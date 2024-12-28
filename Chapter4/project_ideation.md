# Project Ideation

_"I want to use AI to..."_ <br>
_"I'd like you to build me a prediction model to..."_ <br>
_"I need an optimization and simulation tool for..."._

With this section I'm going to share one of the biggest challenges we face in this field.  Far too often we start at the end.  We lead with our assumption of what the final solution should be.  That is, someone at the point of origin for the business use case will lead with telling a technical practitioner how they want them to solve their problem.
```{image} ../images/frustrated_man.png
:alt: frustrated man
:class: bg-primary mb-1
:width: 400px
:align: right
```
Hopefully this strikes you as putting the cart before the horse.  Instead, ideally we'd hear:

_"My problem is today we do **this**, but tomorrow I'd like to be able to do..."._

While it may be obvious that we're going to deliver a model to forecast sales, or maybe we're going to build a model to predict late shipments, and so on, but it's an infinitely better approach to let multiple people, all with different skills and specialties, come to the table and start from the beginning with the problem.  Let the business domain owner do what they do, and that is understand and explain the business problem and context, and let the analytics practitioner do what they do, which is understand how to solve business problems with math.  A marriage made in heaven.

It's critical to be able to work with your business domain experts to generate a large backlog of project ideas.  It's the simple idea of common brainstorming.  Generating a large and unfiltered list of blue sky ideas without trying to qualify or solve the problems at the same time, is a far more valuable exercise than starting with just one idea and jumping in.  Most of the ideas will go nowhere, but having a long list to talk about will allow you to rank, prioritize, and choose what to work on based on a number of factors.

**<h3>Project Ideas & Funnel</h3>**

Let's start with how you might go about the exercise of working with the business to get their creative juices flowing.  Instead of trying to start at the end with solutions to ill-defined problems, how do we get people talking freely and easily getting all of their specialized knowledge out on the table?

The best way to approach these ideation sessions is to have the data science team play facilitator, moderator, and consultancy roles up front.  Let the busines experts do what they do best, which is talk about what they know - the business.  This is where the projects come from, not from the data science domain.  This point can't be oversold.

```{tip}
The data science projects should originate from the business domains, not the analytics team.
```

What this means is the data science resources are not the project sponsors.  The project problem should always come from some other function within the organziation, or at least with them having a seat at the table when flushing out the idea.  Remember, we're the skilled problem solvers armed with advanced methodologies, but most likely know very little about what the business teams care about.  There's no point in us working on something that a business team doesn't care about just because _we_ think it's important.  Believe it or not, this point is overlooked far too often and we try to push our solutions without support from the functional business owners.  It rarely works.

Now for a simple framework that makes it simple and organic to extract the important information from the key resources who will likely not understand, or have the interest to hear all of the technical math speak we might try to use.  

Take a look at {numref}`ideation-ex-fig`.  It's a simple and logical progression that gently guides us to arrive at a currated list of ideas ranked by sponsor interest and potential value.  The key is to move from one question to the next flushing out each topic that comes from your business subject matter experts.

```{figure} ../images/ideation_ex.png
---
width: 900px
name: ideation-ex-fig
---
Example of an ideation session with a project sponsor
```

<h4>Responsibilities</h4>

Recall our Senior Financial Analyst job description example from Chapter 2?  Well, this is the same idea.  There's naturally a set of primary duties and **Responsibilities** that every associate cares about.  People care about what they're incentivized to care about, and Jim's responsibilities are what he's going to want to focus on.  In this case, there's no point in talking about ideas to do with supply chain, marketing, or some other function since he's in sales.

To get us started, we ask Jim to start spit balling all of the things he's responsible for.  

> _What are all of the high-level and big bucket things you're **Responsible** for?_

Everything.  Stream of conciousness stuff here with no value judgements.  We don't worry about the quality of the information we're compiling just yet.  We're simply trying to list out everything Jim cares about to get all of the _potential_ out on the table for further discussion later.

<h4>Decisions/Tasks</h4>

Next, we go through his responsibilities list we just created one by one, and ask the same question for each:

> _What are all the **Decisions** you make and Tasks you have, related to this Responsibility?_

Why are we asking?  Because this is often what we can help with.  My data science solution can either somehow help him make a better decision than he can do on his own, or it might actually fully automate the decision entirely freeing Jim up to work on other things.  Decisions and Tasks are generally the "things" an associate will care about on a day-to-day basis.  This is where we should be mining for gold looking for opportunities.

<h4>Inputs/Data</h4>

Tied to each Decision Jim makes should also be considerations for what **Inputs**, or data, he uses when working with each of those decisions.  Maybe we won't end up making his ultimate decision for him, but we might be able to supply him superior data or inputs that he can then use to make a better decision than he could without us.  

Maybe there's a sales data report published monthly after each month closes that Jim uses to shape his action plans for the next 2-3 months.  It might be valuable if we could provide earlier insights as to what sales are likely to be _before_ the actual sales are known.

For each Decision he makes and Task he accomplishes, we now go through and ask about what data or inputs he uses when considering what to do.

> _What are all of the **Inputs** and data you consider and use to make this Decision or complete the Task?_

Coupled with what we learned from the Descisions & Tasks questions, collecting detail around Inputs & Data should give us all we need to build up a solid list of opportunties to consider. 

<h4>Value</h4>

After the Decisions and Inputs, we're on to one of the most important ideas:  **Value** estimates.  

Just as important as being able to build a robust backlog of potential project ideas, is to be able to quantify the estimated return on investment (ROI) and value of a project, which ultimately allows us to prioritize the list of projects so we can select which ones we're going to work on.

Unfortunately you may find that this value estimation step can be a royal pain in your behind.  It's just never as not as easy as it sounds.  Often what happens is everyone just intuitively understands and agrees that having this "thing" you're going to build is valuable, but when pressed to actually quantify or define that value, _crickets..._  No one may question what we want is a positive and good idea, but we need to be able to compare opportunities based on effort versus reward.  Just because it's obviously a nice "thing" to have, it doesn't mean it makes sense to work on right now.

We need to consider resourcing and available capacity to work on new projects, the payback window (how long will it take to start seeing a return on the work), do we have leadership support since it's much more difficult to get engagement if no one is being told they should care about it, and so on.  It really boils down to large effort and small reward versus small effort and large reward.  If you have the resources and investments already in place and it's a quick turnaround with expected adoption plus a huge qualified dollar return for that effort, these types of projects should be your priority.  

> _What's the estimated **Value** of an incremental improvement in the Decision or Task?_

This may all sound obvious, but let me assure you companies waste thousands of hours each year talking about and working on projects that probably should have been passed over.  Again, this is a tough one, but we've got to try.  My suggestion is to come up with simple ways to attach ballpark estimates.  We don't need to be perfect here.  Just values we can use to compare and rank each idea.  So if it's a time savings kind of project, use a simple formula like

$$
total\:annual\:$\:savings = avg\:hrs\:saved\:\times\:avg\:$\:per\:hr\:\times\:2080\:annual\:hrs
$$

<h4>What If...</h4>

Ok great, we hopefully have a long list of potential **Decisions** and **Inputs/Data** we could predict, forecast, or optimize in some way with **Value** estimates attached for each. Now what? Now we get to the fun stuff.  We get to start doing what _we_ do!  We get to start asking a whole bunch of **What if** questions for the ideas that filtered to the top based on the value and ROI potential estimates we compiled in the previous step.

> _What if we could predict...?_ <br>
> _Would it be helpful if we could tell you...?_ <br>
> _What resources, human, capital, or otherwise, would you allocate differently if I could...?_

The key details to get out of this line of questioning is if the business sponsor truly cares about the proposed solution.  They've told us there's expected value in the idea, but now they should be able to articulate the how's and why's behind why they care.  How are they going to us it?  Why would it be helpful to them if we delivered some solution?  The main thing to get alignment on here is if they would actually do something different tomorrow, than they do today.

```{tip}
The main value Advanced Analytics delivers is enabling better decision making, which allows for a more informed and analytically driven allocation of resources (human, capital, or otherwise).
```

If the business cannot think of how a solution will change what they do in some way, then it's not worth the time and effort. Period.  This is how companies can avoid working on the wrong things at the wrong times.  

At this point you should be starting to see some serious potential for a good idea to work up a proof of concept with.  Hopefully this is resonating and you're beginning to visualize and see how this might work in the real world or within your domain.

Next up we go to scoping and outlining the details needed before beginning any project.

