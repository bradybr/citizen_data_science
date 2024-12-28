# How They Add Value

In any business, associates are hired to perform specific work, typically embedded within a business function.  In these domains it's not uncommon to find roles such as analysts, account executives, team leaders, and directors, to name a few.  These associates could be practically anywhere, from Consumer Insights, Marketing, and Sales, to Manufacturing, Transportation, and Supply Chain.  All of these business functions have domain specific elements of their operations that require specialized knowledge, training, and experience.

Each associate, no matter the domain or title, is responsible for tasks in line with whatever their business function delivers for the company.  My work as a data scientist, you guessed it, is to do data science work.  The thing is though, data scientists typically work in a support capacity.  We seldom own the domain or business function we work in.  We support whichever business function owns the use case, be it Supply Chain, Sales, Marketing, Manufacturing, etc.  My strengths are expertise are in math and machine learning, but these skills are essentially useless unless paired with some area of focus, as within a specific area of business.

Citizen data scientists are first and foremost something else.  They're hired as analysts or associates to work within a business function.  Maybe it's a transportation scheduler, human resource manager, marketing associate, category analyst, procurement specialist, business analyst, etc.  These associates will all have core responsibilities and duties within their business functions they were hired to perform, such as coordinating and scheduling inbound shipments, managing employee retention, allocating marketing spend, and so on.

In {numref}`data-scientist-expertise-fig` we can see the secret that makes this idea of the citizen data science so potentially valuable.  On the left side of the graphic, notice that a professional and full time data scientist will spend all their time accumulating skill and expertise in the practical elements of data science methodologies.  There's a significant amount of effort and time to work up the pyramid through all of the elements of their core capabilities before getting to the top, where we'd begin to gain any understanding of a specific domain.  And once you consider that we often work in analytical centers of competency, meaning we support across a variety of business functions, it's fairly unreasonable to expect these resources to become experts or self sufficient in multiple domains in any sort of expedient time frame.

```{figure} ../images/cds_expertise_pyramid.png
---
width: 900px
name: data-scientist-expertise-fig
---
Professional vs. Citizen Data Scientist knowledge & expertise pyramid
```

Now consider the citizen data scientist pyramid of expertise on the right side of {numref}`data-scientist-expertise-fig`.  It's simply an inverted image of the professional data scientist.  Because their first priorities are the business, these associates spend all of their time accumulating expertise within their domain.  They possess an understanding of the challenges of their environments, have intimate knowledge of the decisions and actions required in their space, possess a detailed grasp of the idiosynchries, rules, and constraints that need to be considered, and finally they sit at the origin of any potential uses cases or projects that may be valuable to the business.

Hopefully the benefit is starting to become clear.  It's simply a longer path for someone to get all the way through to the top of the pyramid on the left than it is for a business analyst, or citizen data scientist, to just get to the second rung of their capability pyramid.  They already know everything they need to know about the potential project use case and the value potential for solving the problem.  All they need now is to get to the next level of Computer Science to begin using the low/no code analytics platforms, such as we've discussed with KNIME.

Please don't misunderstand the message though.  While someone could turn themselves loose straight away using KNIME and start making all kinds of predictions and analytical inferences.  I would strongly advise against it however.  The point it's a quicker and easier path to empower and enhance the _business analyst_ with minimal data science and machine learning knowledge, than it is to try to upskill the full-time professional data scientist in any kind of domain expertise capacity.

**<h3>Financial Analyst Use Case</h3>**

To solidify our understanding with an example, consider the following job description in {numref}`financial-analyst-job-description-fig` for a Senior Financial Analyst.

We'll learn how to do this in more detail later when we get to project scoping and ideations, but for now, begin with trying to understand that the lowest hanging fruit in terms of our analytical opportunities will always exist within the current scope of an employee's role.  Said another way, each employee is responsible for certain decisions and activites, and effectively, these are the things they care about.  You can't go wrong with starting with current responsibilities if you're looking for advanced analytics opportunities.   

In {numref}`financial-analyst-job-description-fig` we see a bulleted list of the primary responsibilities and tasks for this associate.

```{figure} ../images/financial_analyst_job_description.png
---
width: 700px
name: financial-analyst-job-description-fig
---
Job description outlining the tasks and responsibilities for a typical Financial Analyst position
```

After you get a few more pieces of the puzzle under your belt, here's what you'd be able to do with just this information.  Given any list of responsibilities like the one this analyst will care about, you could ask a series of _what if I could..._ questions that might be of interest to them.  And the cool part... you know that the questions you're asking are all tied to one of those 3 things we covered in {ref}`problems_we_solve`, where we either 1) Predict something, 2) Uncover hidden patterns or relationships, or 3) Prescribe something, but you've phrased the question in context and words they understand, which avoided all of the complicated AI and math speak that might confuse them!

Let's see how it works.

- **Prepare Financial Plans:**  _What if I could automate forecasting sales and improve your accuracy from 80% to 95%?_
- **Partner with Business Leaders:**  _What if I could preemptively alert you to abnormal consumer shopping behaviors, prolonged negative sales trends on the horizon, or competitor activities creating risk for your business, all before they happen?_
- **Develop Ad-Hoc Analysis:**  _What if I could prescribe the best course of action for a given scenario you're considering, which will maximize your return (e.g. merger/acquisition/divestiture, staffing changes, new product introductions)?_
- **Work Cross Functionally:**  _What if I could give you a scenario planning and simulation tool that allows you to test the financial impacts of various ideas and strategies, and will optimize your budget and spend across multiple departments?_

<br>

So just from the couple of bullet points in a job description, in a field, industry, and company I am personally unfamiliar with, I'm able to come up with 4 or 5 use case ideas I guarantee you this company would be falling over themselves to have.

Now let's look at this through the lens of a professional full-time data scientist solving the challenge vs. a citizen data scientist, and see how the effort might play out for each.  We'll select the easiest use case idea to motivate our example - Sales Forecasting.

<h4>Professional Data Scientist</h4>

On the face of it, this request seems simple enough, right? Give me some sales data and I'll figure out the fancy math, build some forecasting models, and finally tell you how good they are.  Sadly, it's not going to be that easy.  Consider the following questions I can tell you from experience you should be asking, and will need to know before getting started.

- What am I forecasting (_target_)?  Is it Retail Point of Sales, Customer Sales/Shipments, Net Sales, Gross Sales, Revenue?
- What's the _level of analysis_ you need the forecast at, e.g. Sales, by Division, by Region, by Product, by Day/Month/Quarter?
- What's the forecast _horizon_ window, or how far out do I need to forecast, e.g. the end of the Week, Month, Quarter, Half-Year, Year-End?
- When does the forecast need to be produced, e.g. on the first day of the current month, 3 days before month end, daily?
- Are there any skus, brands, product lines or divisional categories that should be excluded from the data history?
- How many years of data are available?
- Why are there missing time periods in the data history?
- What does success look like?  Are there any accuracy or error benchmarks that I need to outperform?
- and many more...

After weeks and weeks of waiting, and finally receiving answers to all of my questions above, guess what I'm going to do next?  I'm going to open my favorite coding IDE and get to work coding from scratch.  And because I'm so smart and knowledgeable, I'm going to code up exploratory data analysis summaries, plots, and data quality reports to understand what's in my data.  Next, I'm going to investigate the statistical properties of the data target I'm trying to forecast.  Does it have serial correlation?  Is it stationary?  Does it have heteroskedasticity, or non constant variance?  What about any seasonal or cyclical components?  Does it look like additive or multiplicative effects?  And on, and on...

Next up, I'm going to think through some transformations to the data that may help clean up the distribution a bit.  Maybe forecasting the log values would be better?  Or maybe I should try a Box Cox transformation to induce normality?  And then after that, I'll try a million different types of mathematical modeling approaches to see what works best to give me the smallest error on a rolling back test.  Maybe it's a drift model?  Or maybe a state-space model?  Or possibly holt-winters?  And more...

Hopefully at the end of the 4 weeks, and all of these tests and iterations I've carried out, I've built you the absolute _best_ forecasting model on the planet!  And wouldn't you know it?  I was able to get the mean absolute percentage error down to only 5% for my final model!  Not too shabby.  

<h4>Citizen Data Scientist</h4>

Now, for the Financial Analyst (aka citizen data scientist) we've upskilled and trained on how to build a forecasting model.  Guess what?  They already know all of the answers to those questions above!  So instead of scheduling meetings, asking questions, waiting for someone to send data, and then needing time to investigate that data, and all of the back and forth communications that take weeks to accomplish, the citizen data scientist can actually jump right in today!

So far so good, but how about all of those complicated math tests and statistical questions they need to know about, understand, and investigate?  Well, here's where we rely on our low/no code platform.  What if you only had to learn a few basic concepts, like which math and modeling methodologies pair up with each of the 3 types of things we do (predictions, uncovering patterns, prescription/optimization)?, and how to know if your results are stable or untrustworthy?  No need to be an expert in the math or methods, instead learn just enough to be able to work through a minimum number of steps, ask questions, and know when something looks wrong.  That's it! 

For example, if you understood we solve the business case of predicting numbers using time series forecasting math, knew how to navigate the KNIME template which outlined all of the steps and questions you need to work through, could understand the documentation for what "good" looks like, and could follow the steps for things to try if your results _don't_ look so "good".  Hopefully that doesn't sound too scary.





Let's say I'm right and all of that is possible!

**<h3>What Did We Learn?</h3>**




The fact is, I don't work in Sales.  The request for a solution to this problem did not originate with me.  I can guess what I think the answers are to my questions, but the truth is, it doesn't matter what I think.  what matters is I deliver what my business sponsor wants, and only they will be able to answers these questions because they can.  They're the ones who understand the Sales function, and they're the ones who will use what I build.


Hopefully the light bulb and bells of excitement are starting to go off and ring in your head, and you're seeing the potential of what we're talking about!

