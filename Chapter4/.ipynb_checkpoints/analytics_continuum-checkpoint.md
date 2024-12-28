# Analytics Continuum

Let's start with a view of the analytics continuum.  There's no value judgement below, as significant value can be found anywhere along the continuum; however, there is a natural progression of implied complexity as you move from left to right.  Data scientists mostly _want_ to live on the right side of the graphic, but it's certainly not unusual to progress through the descriptive, visual, and statistical steps during the course of an actual project.
<br>

```{figure} ../images/analytics_craddle.png
---
width: 700px
name: analytics-craddle-fig
---
Analytics Continuum
```

These lists are non mutually exclusive, and we'll often say "generally" because there are few hard and fast rules here.  It's not unusual for a data scientist to be working on a project using only traditional statistical methods.  Again, it's not important that we're super strict with definitions and classifications, but more so that we gain a better understanding of what's commonly considered to be included under the umbrella of Data Science.

**<h3>Descriptive Statistics</h3>**

If we look at {numref}`analytics-craddle-fig`, we can understand that the majority of the traditional analytics produced today falls into the first bucket of trying to explain _what happened_ (Descriptive Analytics).  Why?  Because it's the most accessible and requires the least amount of specialized knowledge.  Nearly every entry level business associate should be able to take some historical data and summarize it in some interesting way.

 - What's the percentage of sales for this quarter by region?
 - Which late shipment reason code was applied most often last month?
 - Which customers are paying their invoices late, ranked as a percentage of total sales?

<br>

How about highlighting your findings with a simple barplot?

Is there any evidence of chivalry based on the survial rates from the famous Titanic disaster?  Turns out... maybe.  In the plot below we can see that over 80% of men perished that fateful night, whereas only 26% of the women on board died.  Very interesting.   _Women and children first_ possibly?

```{figure} ../images/titanic_survival_by_sex.png
---
width: 500px
name: titanic-survival-by-sex-fig
---
Titanic Survival Rates by Sex
```

This is all the domain of Descriptive Analytics.  Overall, pretty intuitive questions you might think of when interrogating a data set, which is why it's the most frequently employed; however, don't be fooled into thinking analytics has to overly complex or elaborate to be valuable.

```{tip}
Analytics does not have to be complicated.  Sometimes all that's needed to make a massive impact is simply a clear understanding of what's happening.
```

**<h3>Diagnostic Analytics</h3>**

Moving on to trying to understanding _why_ something happend.  Diagnostic Analytics in {numref}`analytics-craddle-fig` shows us this bucket has been the traditional home for the more advanced and mathematically inclined in any organization.  These have historically been engineers, economists, statisticians, research and development (R&D), demand planners, and even MBA's, to name a few.  

What's important to point out here, is that this set is working with higher order mathematics more so than the average analyst.  We'll discuss this further when we get to methodologies, but for now it's enough to know what really sets this group apart is their statistical prowess.  We do see some crossover into the more data science-sy territory with this group because we often use some of the same math and solvers.  Where we usually diverage is in the end-to-end business continuity, the types of problems we solve, the technology and programming languages we use, and the applications we build.  I know it's hard to see the distinctions now, but stay tuned.  It will become more clear as we introduce new topics.

An example for this group wouldn't be complete without mentioning the workhorse of statistics:  Regression.

 - Want to understand the relationship between height and weight?
 - Want to estimate what raising your retail prices will do to sales?
 - Want to understand if a promotion you ran last month influenced your sales?

<br>

Then welcome to statistics and regression my friend.  There are lots of other methodologies being used with diagnostic analysis, but the main distinction is we're essentially stopping short of predictions and instead usually making some sort of statistical inference (i.e. looking at a sample of data and drawing some kind of conclusion from your analysis).

We'll cover these topics again in later chapters, so don't feel like you're missing anything if you don't quite understand the _how_ behind the ways these questions are answered or the details behind these methods.

**<h3>Predictive Analytics</h3>**

Now we get to the fun stuff (IMHO).  Predictive analytics always felt like the "what's new and different" when I was first introduced to the field.  General business assocates are often quite capable of analyzing data with descriptive summaries, and statistics was burned into my brain as a chore from my college years, but now I was being asked to think about how cool it would be if I was able to predict which specific employees were likely quit next month, or which product had the highest probability of running out of inventory next week.  Taken even further with topics that held more personal interest was really exciting as well.  Could I predict the winner of an upcoming MLB baseball game?  Could I predict which stock had the highest probability of going up in price tomorrow?  Super fun stuff!

This set of analytics is generally where we begin to see separation from what a traditional "math" persona or statistician might be comfortable doing.  We also start throwing around words like "algorithm" and "model" far more frequently at this stage.  You can definitely build diagnostic models, but when we get to the predictive stage we're likely talking about building end-to-end, deployable, and resuable models.  Essentially this means we're no longer talking about just answering a one-time question or a one-off study.  Here we may want to frequently run new data through our model and have it continuously spit out new predictions at regular intervals. 

You'll be introduced to all kinds of new topics when we begin discussing the methodologies and mathematics from this set in future chapters, but for now try to wrap your head around this idea: We start with data as inputs, then we build models to learn patterns and relationships between the subjects of interest, next we project those learned patterns onto new data inputs, which finally produces a prediction of some kind.

 - Predicting which consumers have the highest likely of responding to a promotional offer
 - Predicting which piece of manufacturing equipment is likely to break down within the next month
 - Forecasting sales for next quarter
 - Grouping products and consumers together to reveal hidden similarities or preferences
 - Detecting foreign objects and ingredient contaminants in food manufacturing

<br>

For another example, imagine how an anti-theft detection program might "see" crowds of people in a small shopping corridor and predict unusual behvior.  Computers do not see things the same ways our human eyes and brains do so we need to somehow encode our data into a format our program can understand.  For now, just understand that public places like this often have software running analyzing video feeds for our facial expressions, body movements, and other indicators of specific behaviors.  From a technical point of view it's very cool, however kind of scary to think about from a personal privacy perspective, right?

```{figure} ../images/crowd_id2.png
---
width: 700px
name: crowd-id-fig
---
Anti-theft detection program
```

**<h3>Prescriptive Analytics</h3>**

Now we've arrived at the final, and typically the most complex type of analytics: Prescriptive.

Prescriptive Analytics is another set similar to Diagnostic Analytics, in that it has historically received plenty of attention, albeit from highly specialized practitioners.  These resources tend to be masters or Ph.D. level associates highly skilled in applied statistics, linear algebra, and calculus.  Practically speaking, the field of Operations Research, alternatively known as Management Science, has been the applied faction in business traditionally focused on linear modeling and optimization.

Generally, the idea of this set is focused on steering an organization towards better, hopefully optimal, decision making, by using specialized mathematics and analytical techniques.  We want to _prescribe_, or direct our business stakeholders with information telling them what they should do.  The techniques we use can be anything from simple algebra and linear programs, stochastic optimization, to extremely complex non linear functional solvers.  Regardless of the type or industry, these optimization problems will nearly always have the same components, i.e. input variables, decision variables, an objective function, and optionally, constraints if applicable.  

Lots of new terms here we'll explain in greater detail later, but think of optimization simply as taking in some information (input variables), telling it what answer you would like to get back (decision variables), describing what you would like the solution to minimize or maximize (objective function), and possibly giving it some rules the solution must respect (constraints).

This type of optimization lends itself well to manufacturing and industries where there are complex operations with many possibilities for the choices or decisions one could make. 

 - Resource shift scheduling
 - Transporation route planning
 - Production sequencing and scheduling

<br>

Taken even further to a more complex degree, a field of study known as Reinforcement Learning (RL) is often in the public eye due to high profile companies such as Tesla.  Any guess as to how those fancy autonomous driving vehicles are learning how to avoid pedestrians and other obstacles?  You guessed it, reinforcement learning (among many other types of math and models).  RL is a type of complex specialized program that learns how to make sequential decisions that lead to the best cumulative benefit over a longer time horizon.  An easy way to think of RL is as decision making under uncertainty, or in uncertain conditions.

In manufacturing, these learned state-action policies are often used to automatically control extremely complex pieces of machinery without requiring human intervention.

```{figure} ../images/manif_process.png
---
width: 700px
name: manif-process-fig
---
A complex manufacturing operation with parallel and sequential tasks
```

Whew... that was a lot.  Sorry, had to get it out of the way.

At this stage you've been introduced to some fundamental data science methodologies and project types at a very high level.  There's so much more to expound on and we'll begin to discuss in more detail in the upcoming sections.

Let's pivot now to discuss what makes Data Science so exciting by looking at the kinds of problems we solve.





