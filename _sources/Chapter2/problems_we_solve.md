---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

(problems_we_solve)=
# Problems We Solve

You're going to be introduced to a whole bunch of new fancy technical words if you want to learn about using data science.  Unfortunately there's not much I can do about that.  What I can do though is try and make it as simple as possible for you to get that _ah-ha_ light bulb to go off.  There's always a simple explanation to convey complicated matters, and this is where the skill of your tutor comes in.  Hopefully I won't let you down.

We'll talk about this more soon, but one of the biggest challenges we have in this field is not figuring out how to solve a problem, understanding complicated math, or the tools and technology.  The truth is, the single largest barrier to solving a problem with data science is _business understanding_.  From our point of view, understanding the challenges, situations, and nuances of the environment we're being asked to work with.  From the business sponsor point of view, understanding what special skills we bring to the table, and the what's and how's behind all of the ways we can solve their problems.

To avoid that confusion, let's forget about all the fancy words like AI, data science, machine learning, ChatGPT, neural networks, or any others you've come across for the moment.  We'll get there.  But for now, let's make it crystal clear before we complicate things with new terms.  At the end of the day, it's actually pretty simple what we do.  All of the problems we solve can be categorized into just a few buckets.

```{note}
Everything we do can be reduced to the following:

1. Predicting something
2. Uncovering hidden patterns or relationships
3. Prescribing something
```

<br>

Hard to believe I know, but that's pretty much it.  There of course edge and specialty cases that don't fit so neatly into these categorizations, but easily 95% of our projects will fall into these buckets.  

Let's learn a bit more about each, starting with Predictions.


**<h3>Predictions</h3>**

This is the area I associated the most with data science and machine learning when I began getting into the field.  It seemed the next logical jump from what an advanced analyst could tell you about historical trends and relative frequencies, to being able to actually make a mathematical prediction about what was going to happen in the future.  

```{image} ../images/pred_event_cal.png
:alt: prediction event calendar
:class: bg-primary mb-1
:width: 300px
:align: right
```

There are tons of ways you can make predictions, and all sorts of methodologies you could employ from simple to complex, but they all boil down to two simple ideas; you're either trying to predict an event/occurrence or class (group) of some sort, or you're trying to predict a number.  

Generally you have visibility into some kind of past behavior or results, and you'd like to project that insight into the future by converting it into an estimate, or prediction, for what is going to happen.  These predictions frequently have a timing element baked in as well, e.g. you need to make a prediction today about what will happen 3 weeks from now.

<h4>Predicting An Occurrence or Class</h4>

Can you think of an event or class you might care about?  Maybe it's predicting the upcoming MLB World Series winner.  Or maybe you might want to predict the direction of the stock market tomorrow, whether it will be higher or lower than it was today.  How about predicting which baby names will be the most popular next year?  There are endless possibilities to what you could predict.  Whether or not you could do any of these successfully or accurately is however another matter for a later discussion...

In the business world, you might be interested in predicting if potential customers will respond to a sales promotion or not.  You might also like to know if any of your customer shipments are going to arrive late past their due dates.  Or maybe, what if you wanted to raise an alert in your factory if a piece of machinery has over an 80% chance of breaking down in the next week.  Wouldn't that be of interest and save your company lost down time and sales if you could preemptively service the machine before any type of catastrophic failure occurs?  You bet it would.

```{image} ../images/equipment_failure.png
:alt: equipment failure
:class: bg-primary mb-1
:width: 500px
:align: center
```

<br>

When we're predicting events or occurrences, it's pretty straight forward and easy to understand.  It's typically a binary, either yes or no prediction declaring whether or not it's going to happen.  Predicting classes, or groupings, can take on more descriptive meanings, such as happy/disgruntled, late/on time, benign/malignant, normal/abnormal.  It's essentially the same thing as with events and occurrences though - binary predictions, typically one in the affirmative and one in the negative, depending on which class or group you actually care about and are trying to predict.  Predicting occurrences and classes can actually be more than two groups, but binary two class predictions are by far the most common.


<h4>Predicting A Number</h4>

Now, the other type of prediction - predicting a number.  This one generally can be thought of as forecasting; however, you may also hear it referred to as regression, or estimation.  Personally I prefer not to use regression to mean predicting a number, because 1) regression is a method and statistical tool, and 2) not all forecasting methods are regression based.  While regression can predict numbers, it's probably more commonly used for statistical inference, where the primary objective is coeficient estimation and not predictions.  We're getting a bit ahead ourselves here, I just want you to be aware you may see or hear this one referred to in a few different ways.

```{image} ../images/sales_forecast_graph.png
:alt: sales forecasting
:class: bg-primary mb-1
:width: 300px
:align: right
```

This one is probably an idea you're already familiar with.  Maybe you're a sports fan and would like to try and predict NFL scores each week?  I'm thinking Chicago - 30/ Detroit - 27.  How about forecasting what the chance of rain will be tomorrow (you probably don't need to go through the trouble if you live in San Diego, but maybe useful elsewhere)?  You never know what you're going to get where I live.  And maybe you're thinking of investing in Apple, and you want to forecast their annual sales for next year to decide if they'd be a good investment today?  I'm not even going to hazard a guess on this one...

So predicting a number, or forecasting, is hopefully pretty easy to wrap your head around.  You should have some past history to draw insight from, and you're then able to make some sort of educated prediction about what some value will be in the future.  Whether that's sales dollars for the next year, someone's weight (lbs/kg) based on their height, or even what the population of honey bees will be in South America 10 years from now.


**<h3>Uncovering Hidden Patterns & Relationships</h3>**

Next up is the exploratory side of what we do.  You'll often hear this group referred to as data mining or exploratory modeling.  We typically do not have a "target", or specific output of interest like we do with predictions.  We're still likely interested in improving some target like sales, response rates, equipment failures, etc., but the main bjective is to learn something useful about our data under study.

For example, with sales forecasting, you're explicitly asking to know what the next sales dollar amount will be so you can take some action before it's too late if the forecast comes in lower than expected.  With these exploratory methods, increasing sales may still be the overall objective too, but here our aim is to look through the data and learn some statistical relationship we may not have known about or understood.  With these new insights, we'll then go to the next step and develop plans to be discriminate and targeted with our actions, which hopefully will give us better results.

```{tip}
I'm intentionally blurring the lines a bit under this bucket between the more common understanding of methodologies (i.e. supervised and unsupervised learning), that you will hopefully come to realize later, but for now understand that we're grouping things by objective (the _what_ we're trying accomplish) instead of mathematical approaches.
```

<br>

There's a tremendous amount of examples that should fall under this section, however the goal of this introduction is simply to introduce a few examples, not an exhaustive list.  Understand that a large number of statistical and machine learning methodologies are centered on this idea of pattern identification.  Similarity/dissimilarity scoring, causality modeling, graph networks, latent class analysis, structural equation modeling, dimensionality reduction techniques, to name just a few.  

Enough confusing words.  Back to the simple examples.

<h4>Clustering</h4>

First up is clustering.  You may not have heard of the word, but no doubt you're familiar with the simple idea.  Imagine you have a customer list with 10,000 people who have patronized your business.  It includes demographic and socioeconomic details, such as gender, age, race/ethnicity, education, income, marital status, email, address, household dynamics, etc., and their lifetime value to you as a customer.

Now what could you do with this data?

A great place to start is to see if you have any natural groupings (clusters) that people fall into.  Everyone grouped together will be more similar than dissimilar, and they should look different somehow than those placed in other clusters.  If we could do this in some meaningful way, we'd be able to direct our efforts and tailor our approaches based on what's going to work best to ellicit the responses we want from each group!

```{image} ../images/customer_segmentation.png
:alt: customer segmentation
:class: bg-primary mb-1
:width: 400px
:align: right
```

Hopefully you're realizing this is just the beginning of what you could do.  Any ideas for what you might do next?  How about looking into each cluster to understand _why_ customers in each group are similar, and _why_ they're dissimilar to those in other clusters?  Maybe all of the customers grouped in the first cluster skew disproportionately to families with multiple children, or maybe individuals with higher levels of education, and so on.  

What if you see many people assigned to a high sales value cluster that have disproportionately fewer sales transactions than others in the cluster?  Think you might be leaving sales on the table and should try to figure out why?  Hopefully you're saying yes!

We are now in a position to take what we've learned about the similarities and differences in our customers to help target and direct our plans, strategies, and allocation of human and financial resources more effectively!

<h4>Patterns, Associations, & Correlations</h4>

This one is a broad bucket I'm using to cast a wide net for use cases.  No matter what methodology we're talking about, the general idea is that the objective is to find interesting relationships between events or phenomena in our data.  This can be people, products, activites, and practically anything else that interacts together. 

Whether it was your account or not, I'm willing to bet you've either used Netflix or are at least reasonably familiar with how it works.  Did you know Netflix has sophisticated algorithms running in the background to monitor viewing behaviors so they can make recommendations to each user's account?  Their goal is to keep you interacting with their platform as long as possible.  To do this, they need to continuously serve you with recommendations for what they believe has the highest chance of catching your interest and enticing you to click on the next show.

So how do they know what to recommend?  Easy.  First, they learn what kinds of programs you like to watch, e.g. sports, documentaries, romantic comedies, adult cartoons, or whatever it may be, and a whole bunch of other descriptive meta tags that paint a picture of your interests.  Next, they learn what other viewers watched and rated highly after viewing similar content to yours.  Finally they combine what they know about you with what they know about everyone else, and calculate what has the highest probability of keeping your attention.

```{image} ../images/netflix_recommendations.png
:alt: Netflix recommendation engine
:class: bg-primary mb-1
:width: 600px
:align: center
```

<br>

So the next time you're watching Netflix and see "Because you watched..." recommendations, know they weren't pulled out of thin air but driven by behavioral science and mathematical models designed to increase your engagement with their platform.  This type of methodology and solution is more formally known as a _recommendation engine_.  They've become so commonplace today that we hardly even notice them anymore, but understand they're out there running in ecommerce, news, search engines, and practically anywhere people consume content or make decisions and want to know what to do next.  Remember, the company that makes money off of you will gladly offer you a suggestion, even if you don't ask for it.

How about when you're using your Target Circle Card?  Think there's an opportunity for Target to analyze your purchasing habits to exploit?  Absolutely.  

```{image} ../images/shopping_cart.png
:alt: association rule mining
:class: bg-primary mb-1
:width: 400px
:align: right
```

Imagine if they just looked through every single transaction for the last year and analyzed which items were purchased together.  Don't worry.  It's well known that they do...  It's called _market basket analysis_, and is widely applied in the retail industry.  The idea is to look through each individual transaction and calculate how often items are purchased together, and design statistical tests to decide if the relationships are real and interesting.  

For example, would it surprise you to learn that Lays potato chips have a strong association and correlation with Coca-Cola?  Probably not.  What if I told you there was a relationship between Lays potato chips and Hefty trash bags?  It would be news to me.  We're getting into interesting territory now if Category Managers from the brands and the Buyers at Target find out that 68% of all baskets that contained Lays potato chips also contained Hefty trash bags.  It might even get more practically useful if we look at the times of the year when these frequencies pick up, and further possibly interesting if we layer in our previous clustering methodology.  Just think what we can do now.

How about designing new co-promotions with these two brands at the same time?  What about targeting specific people and demographics with Catalina coupons (those long coupons that print out at the register with your receipt) based on what their cluster grouping reveals about their likelihood to purchase?  How about new in-store merchandising highlighting the two brands on the same end cap shelf?  What about timing the promotional and pricing activities to align with whatever seasonal drivers are at play tied to consumer propensity to purchase, e.g. Superbowl, summer months, holidays, graduation season.  And so much more.

<h4>Statistical Inference</h4> 

Remember talking about regression a few sections ago?  Hope so.  Regression is undoubtedly the workhorse of applied statistics and the go-to methodology when we're talking about statistical inference.

Often the point of interest is not the output of the model, but the model itself.  I know we haven't really covered what a model is yet, but hang tight.  We will.  For now, simply understand that a model in this context is a mathematical equation or formula.  These formulas typically have parameters that need to be estimated, which is the point of modeling since we're trying to uncover the equation that explains the data it learned from.  I know... this is a heavy paragraph, but stay with me.

```{tip}
Statistical inference is all about taking a sample of data, learning from what you observe in that sample, and then projecting those learnings onto the unseen part of the data population and hoping what you learned still applies to these new observations.  We call this last part _generalization_.  
```

<br>

Let's crawl with a simple example before we try to run.  Below are the first 5 rows of a real dataset containing customer transactions from a restaurant.  We can see that the dataset contains the total bill amount and also the amount the customer left as a tip, along with additional details about the party.  

```{code-cell} ipython3
---
tags: ["remove-input"]
mystnb:
  image:
    align: center
    alt: seaborn tips data
  figure:
    caption: |
      Seaborn "Tips" dataset
    name: seaborn_tips_data
---

import seaborn as sns

tips = sns.load_dataset("tips")
tips = tips[17:22]
tips.reset_index(drop = True, inplace = True)
tips.style.format({'total_bill':'${:,.2f}',
                   'tip':'${:,.2f}'})
```

If we look at all of the total bill amounts plotted against the tip amounts received on those totals in {numref}`regression_scatterplot`, we get a nice visual of the overall relational pattern.  Clearly there's an upward sloping direction from left to right, indicating tip amounts rise when the bill gets larger.  Makes sense!

```{code-cell} ipython3
---
tags: ["remove-input"]
mystnb:
  image:
    align: center
    alt: regression scatterplot
  figure:
    caption: |
      Scatterplot with overlaid estimated regression line
    name: regression_scatterplot
---

import warnings
import seaborn as sns
import matplotlib.pyplot as plt
import matplotlib.ticker as ticker
warnings.filterwarnings('ignore')

tips = sns.load_dataset("tips")

sns.set_theme()
fig, ax = plt.subplots(figsize = (6,4))
sns.regplot(x = "total_bill", y = "tip", data = tips, line_kws = dict(color = "red"))
ax.set_xlabel( "Total Bill", size = 12)
ax.set_ylabel( "Tip", size = 12)
ax.yaxis.set_major_formatter(ticker.StrMethodFormatter('${x:,.0f}'))
ax.xaxis.set_major_formatter(ticker.StrMethodFormatter('${x:,.0f}'));
```

Now remember all that talk about estimating mathematical equations?  In this example, if we regress `tip` on the `total_bill` amount (estimate the mathematical equation that best approximates this relationship), we arrive at a value which tells us what happens, on the average.  Running a regression on this dataset gives us a beta coefficient of \$0.11, which can be interpreted as the effect the `total_bill` amount has on the amount the server received as a `tip`, holding all else constant.

So in simple terms, for every \$1.00 increase in the total bill amount, the server can expect to receive \$0.11 additional in their tip.  We can see the actual visual representation of our mathematical equation in {numref}`regression_scatterplot`, as illustrated by the red line.  Our \$0.11 coefficient is the effect causing the slope of the red line to point upward \$0.11 per \$1.00 increase in the total bill.  Pretty cool.

This is just the tip of the iceberg with statistical inference.  Often our business sponsors will seek understanding in terms of the effects their actions are having on their results, and there are plenty of different methodolgies and techniques that can answer these types of questions.  There are tons of approaches and methodolgies you could leverage to deliver these insights, but often straight forward statistical analyses and studies may be all that's required.

**<h3>Prescription</h3>**

Last up is the awesome world of Prescriptive Analytics.  This is definitely on the higher end of the mathematical complexity spectrum, but certainly not out of the reach for anyone willing to put in a little study time.  There are some very math heavy methodologies in this group, but don't be scared off just yet if you don't have your PhD in Quantum Mechanics.  There are also some very accessible and intuitive techniques that are not beyond your comprehension.  I promise.

So what do we actually mean by Prescription?  It simply means we're going to _prescribe_, or tell someone what they _should_ do.  Yep, that's it.  It may be easier to think of this bucket as trying to _optimize_ something.  That is, we're going to take in some data, consider the possible actions we're allowed to take, learn the rules of the environment, and then ultimately make some statements about what the best course of action is that's going to yield the best end result.  Whatever that goal may be.

<h4>Optimization</h4>

A classic example of a simple optimization task is one known as the "Knapsack Optimization Problem".  The setup is you're planning a several night outing in the woods this weekend and need to decide which items to take with you.  Each item has a quantifiable benefit, or value, in terms of a survival scale (higher being more important).  Your constraint making this a challenge, is that your backpack can only carry so much weight, so you'll have to limit what you bring with you and leave the rest behind.

```{image} ../images/knapsack.png
:alt: knapsack optimization problem
:class: bg-primary mb-1
:width: 700px
:align: center
```

<br>

Your task is to maximize the total sum value of the gear and supplies you bring, while keeping the total sum weight below your backpack's max limit of **28 lbs**.  Using one of the many optimization approaches we could choose, you can see below we found an optimal solution that allowed us to pack 6 of the 9 items.  The total weight of the selected items came in at 27 lbs, just one pound shy of our limit, and we maximized our survival points at 69!  

```{code-cell} ipython3
---
tags: ["remove-input"]
mystnb:
  image:
    align: center
    alt: knapsack solution
  figure:
    caption: |
    name: knapsack_solution
---

items = ['coat','knife','water','gloves','sleeping bag','tent','stove','food','snacks']
path = ['food', 'tent', 'gloves', 'water', 'knife', 'coat']

print("The list of gear and supplies that maximizes our survial points is:\n   " + ', '.join(path))
print("\n")
print("The following items did not make the cut and will be staying behind:\n   " + ', '.join([i for i in items if i not in path]))
```

It's interesting to see which items were selected.  Just from a cursory look, you may have noticed the program prioritized the high value items of tent, food, and water, and then seemingly filled in the remaining available weight with the lowest weight items of gloves, knife, and coat because the added value of multiple items would be higher than just being able to add only one more of the mid range weight items.  Very cool stuff!

Image you work for FedEx and were put in charge of planning the shipment territories and determining the route scheduling for each of their 200,000+ trucks that need to deliver over 16 million packages each day {cite}`FedEx_2024`.  Can you imagine the complexities you would have to consider to number one, decide which packages go on each truck, and then number two, give each driver the most efficient ordering of their stops so they don't have to waste time and back track throughout the day?  Well, this is exactly the stuff of optimization.

Give the program all of the addresses and distances, a few rules and constraints it needs to respect, and then tell it you it to find and give you the daily sequences of stops for each driver that will minimize their total mileage traveled for the day, and BAM!  You've just saved your company millions of dollars in gas, equipment costs, overtime, and not to mention the negative costs associated with unhappy customers due to late deliveries.

As with Statistical Inference, this is just the beginning of what's included under the header of Prescriptive Analytics.  There are many more sophisticated areas contained under this heading that are beyond the scope of our learning objectives here.

At the end of the day, we're simply trying to find the best decisions we can make that will minimze or maximize some end result that we care about.  Whether the task is to make a one-time decision from a single list of choices, or learning how to make multi-step sequential decisions as a situation evolves over time, these programs can excel under various conditions of uncertainty.  No matter whether we want to maximize sales, profit, or our time, or maybe we care about minimizing carbon emissions, quality defects, or production scheduling, these are all measureable results we can monitor and compare within our decision sets given the universe of choices we could make.






