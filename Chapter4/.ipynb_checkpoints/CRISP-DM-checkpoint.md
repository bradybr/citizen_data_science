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

# CRISP-DM

Now that you understand how we get to the point of undertaking a project, let's turn the page to see what the actual process of working through one looks like.

Picutre this: You've just been tapped to jump into a meeting to help with some vague notion of a business problem one of your teams is talking about.  Now what?  Do you sit back and let them all flush out the idea, and then you swoop in at the end with your fancy math and solve the problem they've come up with?  You could, but I'd be willing to be you the project will get off the rails and miss the mark somewhere along the lines if you do.

Ok then, is there a better way?  Glad you asked.  Yes there is.  There's no reason to reinvent the wheel.  Some really smart people came before us a long time ago and gave us a pretty well thought out end-to-end process for data mining/science projects.  Enter CRISP-DM.

**<h3>Cross Industry Standard Process for Data Mining</h3>**

Have you heard of deductive or inductive reasoning?  With deductive reasoning, we begin with a few basic axioms - simple true statements regarding how the world around us works.  Inductive is exactly the opposite where uncovering simple truths about some phenomenon is the _goal_ of the investigation, not the _starting_ point.  Out of inductive reasoning we get the scientific method we briefly touched on in Chapter 2.  

```{note}
The process cycle we follow is a combination of the deductive mathematical methods in data mining, and experimentation and testing steps from the inductive scientific method {cite}`NIS_2009`.
```

The most widely used framework in the industry for data mining and analytics is called **CRISP-DM** (Cross Industry Standard Process for Data Mining), below in {numref}`CRISP-DM-fig`.  There have been proposed extensions and adaptations over time to address deficiencies in the model, but it is still regarded as the dominant guide which many teams follow.  You may also find it's common to add in a layer of project management via either an agile or scrum methodology (e.g. IBM's Analytics Solutions Unified Method {cite}`IBM_WP_2016`).

```{figure} ../images/CRISP-DM.png
---
width: 400px
name: CRISP-DM-fig
---
CRISP-DM phases as the industry standard workflow process for data mining and analytics
```

<h4>Business Understanding</h4>

Starting from the beginning with Business Understanding.  We need to understand the business context, sure of course, you're probably saying.  Saying it and doing it well are two different things in practice though.  This one is deceivingly simple.  What could go wrong?  Well, first of all, do you think the business sponsor you're working with understands what your specialty is?  What you could do to help them?  What kinds of information you need to know?  Hopefully you answered "no" to all of these questions because I would bet they do not.  Unfortunately what this means is it's up to you, or at least someone on the team that understands the bridge between the business and data science, to be sure to ask all of the right questions and collect the relevant information you'll need to know.  And there's a long open-ended list of questions that will vary for each project.

We can cover a few common ones that will be good starter questions regardless of the project specifics.

- What is the current process you have now?
- What's the current level of performance (KPI's, metrics, etc.)?  Do you understand why it's not good enough?
- Are there special exceptions and considerations?
- What are the objectives for the project?  What are we trying to solve for?
- What are the deliverables?  A one time study?  A re-useable production solution?
- Who are the end users and what are their needs?
- And so many more...

You'll need to become comfortable with general fact-finding and surveying your business domain experts.  Asking one question and getting an answer is generally not the end of it.  Follow up questions will be required, new questions and clarifications will spring from their answers, and you'll need to observe the loop from Data Understanding back to Business Understanding in {numref}`CRISP-DM-fig` as new information becomes available.

This understanding of the business context is so critical to the success of a project that we devote the next section {doc}`../Chapter4/project_charters` to it as well.  We will really drive home this idea of finding value through the citizen data scientist being embedded within a business unit in the coming sections.

<h4>Data Understanding</h4>

All of our high-powered methods rely on data.  This one is also extremely vital to the success of the project (as they all are really), but there's a few plot twists to consider when we start thinking about data.  The first is the data generation process, followed by access and acquisition, and lastly data quality and understanding.

On a practical level, do you know how the data was actually created?  I mean the actual physical process making the data available.  Is someone manually entering data into a spreadsheet?  Is it system generated?  Which systems?  When is it updated?  Are there revisions or restatements that you need to account for?  And many more questions.  Next, from a statistical point of view, do you have any understanding of the **data generation process**, or _DGP_, which is the phenomenon or mechanism that actually creates the data we're observing.  If you can build a mathematical model that accurately reflects this process which created your data, then you've hit a home run.  You can now do all sorts of interesting things with your model, like investigating how changes to specific parameters will affect the system, simulate new data to study, make predictions, and run scenario planning queries.

Now let's talk about actually getting your hands on the data.  Do we have access to all of the technical environments that house the data?  Are we going to import offline manual files, open up an API (application programming interface) connection, or get it from the source?  Will the proof of concept method of ingesting data be the same as when we get to the production version, or do we need to create a new process?  If so, who will maintain the process after deployment?  Do we have any legal or contractual restrictions with what we're allowed to do with the data?  Are there security and compliance considerations if we're using private personal information (PPI) data?  You definitely do not want to be the reason your company gets splashed into the news with some kind of data breach that exposed sensitive consumer data into the public domain.

Ok now we have our data, but do we understand it?  Are there special codes or idiosyncrasies we need to ask the domain experts to explain?  Do we understand the time intervals or frequencies being pulled?  Are there hierarchies or aggregated levels in the data?  Is anything being filtered out or omitted?  How are missing values handled, e.g. empty, nulls, NA's, 9999 placeholders.  This step also includes a descriptive exploratory analyses step known as exploratory data analysis (EDA).  Numerical summaries and distributions, mode frequencies and counts for categorical features, and descriptive plots will be one of the first things you want to do when you get started.  We'll discuss all of this later in {doc}`../Chapter5/EDA`.

You'll often hear the phrase "garbage in, garbage out".  Please believe it.  You can't expect to be able to predict sales accurately if the historical data you collect to inform your models is completely untrustworthy and inaccurate or you don't understand it.  Or don't expect to be able to predict when a piece of machinery is going to break down if you can't get your hands on data without missing time windows.

<h4>Data Preparation</h4>

Notice there are two sections associated with data in the {numref}`CRISP-DM-fig` framework?  That's because we spend the majority of our time working with data.  It was a bit surprising to me when I found out how much.  General estimates are that we spend ~70-80% of our time dealing with data.  I came into the field thinking it was all math and modeling, to find out it's really only a small perentage of our time.  By far, we spend most of our time acquiring, understanding, transforming, restructuring, enhancing, and prepping the data _for_ the modeling work.        

Data preparation may not be the most talked about steps in the cycle, but it is one of the coolest in my opinion.  Why?  Because it allows you to be creative and solve a problem in a way that maybe no one else thought of.  This is where the magic really happens and will make or break your ability to get good results.  

```{tip}
The world has plenty of algorithms.  What it can always use more of is creative associates and analysts capable of thinking critically and being imaginative with how they present data to those algorithms. 
```

This is the stuff of data preparation.  We'll cover all of these in greater detail in the {doc}`../Chapter5/wrangling` and {doc}`../Chapter5/feat_engineering` sections, but below is just a taste.  Again, at this stage it's more about conceptual understanding than anything else.

When you start working with data, you'll learn about data distributions and what are called statistical moments.  Some distributions are especially desireable, like the standard normal distribution; whereas some like a non theoretical multimodal ones will give your algorithms fits and make your results untrustworthy if you don't recognize what you're working with.  Most of the machine learning algorithms we deal with will perform better if your data is normally distributed.  So when we get into learning about Feature Engineering transformations, you see that we often want to try and induce normality when we come across a skewed distribution, like the exponential one below.

Let's generate some data from normal and exponential distributions and plot them so we can see what they look like side-by-side.

```{code-cell} ipython3
---
tags: ["remove-input"]
mystnb:
  image:
    align: center
    alt: seaborn tips data
  figure:
    caption: |
      Distributions
    name: test
---

import warnings
import numpy as np
import pandas as pd
from scipy.stats import boxcox
import plotnine as gg
warnings.filterwarnings('ignore')

# Generate normal & exponential distributions
x_norm = np.random.normal(loc = 0, scale = 1, size = 1000)
x_skew = np.random.exponential(size = 1000)

# Create DataFrame
df = pd.DataFrame({"Normal" : x_norm,
                   "Skewed" : x_skew})
df = pd.melt(df)

# Plot
(gg.ggplot(df, gg.aes(x = "value", y = gg.after_stat("density"))) +
     gg.theme_bw() +
     gg.geom_histogram(gg.aes(fill = "variable")) +
     gg.geom_density(color = "black") +
     gg.facet_wrap("variable", scales = "free") +
     gg.scale_fill_discrete(guide = False))
```

See how the "skewed" graph on the right is not at all symmeterical with a clear exponential shape?  Now, what if we try to _transform_ our skewed data and rescale it so it behaves more like a normal distribution instead of an exponential one?  We can do that with what's known as the boxcox method using the `boxcox()` function.  This function will find the optimal parameter to transform our skewed data to be as close as possible to a normal distribution.  Let's see if it works below and then re-plot.

```{code-cell} ipython3
---
tags: ["remove-input"]
mystnb:
  image:
    align: center
    alt: seaborn tips data
  figure:
    caption: |
      Description
    name: test2
---

# Transform skewed distribution to a normal one
trans_skew = boxcox(x_skew)[0]
df = pd.concat([df, pd.DataFrame({"variable" : "Transformed Skewed",
                                  "value" : trans_skew})])

# Plot
(gg.ggplot(df, gg.aes(x = "value", y = gg.after_stat("density"))) +
     gg.theme_bw() +
     gg.geom_histogram(gg.aes(fill = "variable")) +
     gg.geom_density(color = "black") +
     gg.facet_wrap("variable", scales = "free") +
     gg.scale_fill_discrete(guide = False))
```

Success!  See how the "Transformed Skewed" plot looks much more symmetrical like the "Normal" graph than it does like the original data it came from in the "Skewed" graph? Pretty cool.

This is just one example of transforming your data so it sets us up for success down the line in a subsequent step, as with modeling up next.

<h4>Modeling</h4>

Next up is modeling after you've wrangled, transformed, and aggregated your data to the appropriate levels of analysis.  Notice the backwards and forwards link between Data Preparation and Modeling in {numref}`CRISP-DM-fig`.  Iterations are very common for multiple steps, and this one is no exception.  You'll try certain things, test and learn, go back and reformat, and then try modeling again.

First of all, do you know what a model is?  This is one of those "blinking" words that has many definitions across multiple fields, and means something very different depending on who're talking to.  A business person might think you're talking about a conceptual framework like Maslow's Hierarchy of Needs model, a designer/enginner might think you're talking about a physical or even a computer-aided design (CAD) representation, and an informations systems resource might hear the word and think you're talking about a data model for representing the relationships between data and architectural end points.

In our data science world when we hear the word model, we're talking about a mathematical formula.  

```{note}
A data science model is a mathematical formula mapping inputs, an internal algorithmic logic, and outputs, designed to uncover the data generation process of some external phenomenon.
```

Lots of big words I know, but it really is a simple idea.  Remember back when we talked about uncovering the data generation process?  That's what our model is.  It's the simplified mathematical representation of whatever process created our data.  It can be a super simple deterministic model like,

$$
output(c) = input(A + B)
$$

or it can be extremely complicated and non linear, and not approximated by any known theoretical distribution.  At their simplest, these models all have inputs, internal algorithmic operations, and then outputs.

When you get to this stage you'll have some choices to make.  First up is the class of math you need for the problem at hand.  We'll cover this in depth in subsequent chapters, but for now recall the discussion with the types of machine learning algorithms in the {doc}`../Chapter2/what_is_data_science` section.  If it's a supervised classification problem, then your choices of algorithms will be different from those available if it's an unsupervised clustering type of problem.  Next, you'll need to understand there's no way to know beforehand, or apriori, which type of mathematical model will suit the idiosyncrasies of your data best.  This means that even though you know you need a classification algorithm, which one?  There are tons to choose from.  We'll discuss some best practices and where to start when we get there.  Lastly, understand that no matter which algorithm you choose, there are likely going to be some parameters or arugments that may need to be tuned to get the best result.  For example, if you're working with a neural network model, then you'll need to consider how you settle on the number of layers, the number of nodes for each layer, which activation functions, the learning rate, etc.  Again, don't worry.  We'll get there.

Before we move on to the final evaluation phase, we will be doing lots of model building iterations, scoring of in some way, and comparing between all of the candidate models we have to choose from.  We'll cover topics such as the natural error rate, cross validation, loss functions, and more. 

<h4>Evaluation</h4>

You'll go back and forth between Data Preparation and Modeling for quite some time, but eventually you'll want to move beyond development into evaluation of the best model you've been able to create. Like everything else, there are many ways you can go about it. First of all, it depends on the use case and types of modeling we're working with. If it's a classification model, then it's quite possible we ultimately want to use something called a confusion matrix, or even a step beyond called a cost matrix which considers the total sum of penalties and rewards for the different types of errors and correct predictions. If it's a forecasting project, then you may want something more along the lines of a metric called root mean squared error (RMSE), or a simple mean absolute percentage error (MAPE) to give you an understanding of the average +/- error you can expect from your model.

Our models must be better than chance and stand up to scrutiny from the business domain experts by way of some performance measure they care about. By the time we get here, we either solved the problem and are ready to move into the final Deployment phase where we put the model in actual practice, or rightfully we should go back to the drawing board and the beginning if we failed. We'll discuss soon why you really shouldn't go backwards from this stage back into Modeling due to something known as overfitting.

```{tip}
It's actually common for a model to not go into deployment for a variety of reasons.  Unacceptable results, adoption issues, resource commitments, etc.  The good news is, there's value in simply being able to iterate quickly to learn what shows promise and what doesn't, whether you move into production or not.
```

<h4>Deployment</h4>

Finally, assuming we passed the evaluation phase, then we're moving on to Deployment!  If you've done your job well with the project scoping and Business Understanding phases then we should actually be pretty well set up here with few expected surprises.  

We'll likely need to involve others to enact our plan at his stage.  Were we going to deploy in the cloud with pipeline architecture, or a simple web app with manual excel file uploads?  Whatever it was, it's time to reengage all of those additional team member resources like data engineers and MLOps resources to help make it happen.

What about documentation?  The project should not wither away if you happen to leave the role or company.  Are all of the technical considerations and details outlined?  Are the code files hosted in a networked sharing site like Github?  What about user training and documentation for the business users?  

The final consideration is monitoring and maintenance.  The team should have a standard operating procedure for how this is done and by whom.  All models degrade over time.  The environments in which they were trained change, the inputs change, human behavior changes, etc.  The metrics by which we monitor and decide if model degradation has begun to take place will vary by the project and math type.  We'll cover some of the simple and more common ways this can be done when we get to live examples.

**<h3>What Did We Learn?</h3>**

Hopefully you're starting to see why it's so much easier to just say "throw me an excel file so I can get started!", rather than doing it the right way by asking lots of questions and committing to understanding the process and data before proceeding too far.

I'll caution you again though.  This framework exists for a reason.  I can promise you'll pay for it down the road with wasted time and effort if you skip it or don't give it the attention it deserves.









