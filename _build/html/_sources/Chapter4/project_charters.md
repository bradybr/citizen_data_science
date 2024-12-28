# Project Charters

At this point consider you’ve gone through the ideation stage and you've iteratively whittled down your full list to one stand out idea you want to turn into a project.  You could easily just get started with what you know today; however, I would strongly encourage you to spend a little more time and energy on flushing out key details first.  Projects can and often go sideways very quickly from what you originally set out to accomplish, and you can minimize the risks of getting off course if you take the time to document and get the proper engagement from your stakeholders.
 
This section is all about setting you up for success by being intentional and explicit right from the start.  The person responsible for this step will vary across organizations and may not be the data scientist, but possibly the business analyst, project lead, project sponsor, or project manager, among others.  Regardless of who, and whether or not it's an official Charter, going through the accounting and documentation actitivies that follow will unquestionably be time well spent.

**<h3>What Is a Project Charter?</h3>**

Whether it's an official Charter, Executive Summary, Project Plan, or simply an outline in a Word or PowerPoint doc, the answer is essentially the same.  Primarily what we're talking about is documenting the _Who_, _What_, _When_, _Where_, _Why,_ and _How's_ of a project.  The most formal of the bunch is the Project Charter, which serves as a high-level project overview and commitment from multiple key participants involved in the life of an engagement.

At one level we have the requesting and functional owner of the effort (business sponsor) coming to terms with the working team (analytics team plus business subject matter experts) regarding the details of what they want someone to go off and work on, and their expectations for what that working team needs to deliver at the end of the project to be considered a "success".  At a commonly higher level, there may also be the need for awareness and oversight from a Steering Committee for necessary support or approval (capital, human resources, or change management).  This group of leaders will typically have the power to authorize financial support, communicate expectations, set priorities, and clear any blockers for the working team.

A common set of the details found in a Charter are listed below, with an example in {numref}`project-charter-fig`.

1. Business Context/Need
2. Objectives
3. Scope
4. Deliverables
5. KPI/Performance Metrics
6. Resourcing Requirements
7. Project Plan

```{figure} ../images/project_charter.png
---
width: 900px
name: project-charter-fig
---
Example of a one-page Project Charter template
```

A Project Charter should ideally be kept to a one-page document, highlighting all of the details someone would need to understand your project without requiring any further context.  In general, you can't control what happens to a presentation or document after you publish or hit send in your email, so it's a good habit to get into to assume anything you share will get passed on to someone else that may not have the context or opportunity to hear you speak over the content.  

Anyone should be able to pull up this document and understand the motivation behind the effort, what you're trying to solve for and deliver, why it's valuable for the company, the teams and resources involved, as well as a very high-level timeline of major milestones and stage gates.  This is a living document which may require revisions and updates, but the general idea is to lock in understanding and agreement so there's no ambiguity and slippage in terms of the asks and commitments after the project gets underway.

<h4>Business Need/Context</h4>

The logical place to start is with the _What_ and _Why_.  Think of the Business Need and Context as setting the stage and laying out what's going on in the business environment related to the ask.  

This can be framed as _"The problem is today the business does **this**, but tomorrow they would like to be able to do..."_.

> _What problem does the business have today?_ <br>
> _Why are they seeking a solution of some kind?_ <br>
> _Do they have a method in place today that is falling short of addressing the issue?_

<h4>Objectives</h4>

With the Objectives, we begin to move closer to the idea of the desired future state.  We take what we learned from the Business Need & Context, and continue here by outlining the solve for the problem, or _How_ we're going to address their needs.  

For example, if we heard the business state they have no visibility into their upcoming demand for a specific product, which effects their ability to coordinate resources and plan production schedules for the next quarter, then the Objectives could be to "Provide the business with advanced visibility and insights into future product demand prior to when their plans need to be submittted for resourcing and production scheduling".

This is separate from the specific metrics and success criteria we will get to shortly.  Here we simply want to define the focus of how we plan to address the issue and solve what the business has said they need.

> _What is the solve or solution we plan to deliver, and how does it address the problem expressed by the business?_

<h4>Scope</h4>

Now for the Scope - What's in and what's out?

Sometimes it'll make sense for you to first test out the idea in your most complicated location instead of the easiest.  Sometimes the business only cares about a specific brand at the moment so you'll only want to consider certain product lines.  Often there's a certain event or condition that needs to be included within the analysis.  The opposite situations exist as well.  There will times we want to limit the analysis to specific locations, products, and events that may skew your results or don't make sense to be included for whatever reason.  We'll need to be sure to carefully pay attention to what's being _included_ and _excluded_ as dictated by the requirements of the project.

> _Are we starting with a limited scope?  If so, what will be included?  Specific locations, products, customers, activities, etc.?_ <br>
> _Are there any specific situations or required conditions that need to be included or excluded?_ <br>
> _What is the plan for future phases and scaling?_

It's pretty much that simple, but know this is the area that has the most potential to cause issues during the course of a project.  It may seem minor at the time.  Add an extra product line to the analysis that we didn't originally talk about...  Allow an additional condition or capability that was not originally agreed to...  Change the method of deployment from a Proof of Value (POV) to now requiring all of the bells and whistles of a customer facing usable Minimum Viable Product (MVP)...  All of these changes are what's known as **scope creep**.

```{note}
_Scope creep_ is any minor or major changes to a plan, compared to what was originally agreed to and approved for working on during the course of a project.
```

Often we don't jump straight away into a full scale deployment so we need to be very clear about what kind of effort we're running.  Part of scoping a project is deciding on what the delivery plan looks like.  Will you be doing phased iterations of testing, learning, and deployment?  Are certain requested deliverables off the table for the first version, or does everything need to be delivered all at once?  Depending on what matters for our project sponors, there are options to manage the project goverened by various constraints at different times, such as time, money, resources, priority, etc., and to deliver the project in phases.

We may want to start first with a smaller scale limited Proof of Concept (POC) to quickly test the idea before worrying about anything else.  Maybe we want to begin with a Proof of Value (POV) to prove the potential benefit truly exists before we'd spend time on any of the end user functionality.  Or we could deliver a bare bones prototype called a Minimum Viable Product (MVP) to quickly realize a return.  It doesn't need to be pretty, but it will work and prove out the concept, as well as allow the business to capture actual value.  Another option is to possibly deploy a full featured Pilot, carefully built out to the full business requirements.  This version is carefully tested in production environments, and ready to scale to a wider scope after an adequate period of time monitoring the solution in real-time.

Some changes to the scope and deliverables are obvious and easy to reject for being out of scope; however, the ones you really need to watch out for are the little changes that seem minor and within acceptable tolerances to let slide.  The additive and cummulative effects of taking people off task, even in short bursts, can have a devastating effect on the overall timeline.  Remember, the original plan did not include for these tasks and more often than not it pays to strictly adhere to the plan.  This is the exact reason we create these kinds of documents so there are no surprises and we stay on track.

<h4>Deliverables</h4>

Under the Success Criteria, we begin with what we've agreed to actually deliver at the end of the project effort.  Think of this as when you turn the keys over to the new owner, what will they be driving away in?  This can be in a range of any number of formats, from code or white papers, to a functioning web application.  

What we want to document here is exactly what we've committed to overall, but also any special conditions or functional requests from the business called out as a requirement.  This may can be anything from the ability to change the level of analysis from Customer to Product by clicking a button before hitting "run", maybe a specific visual, graph, or view, or a requirement to have the ability to export the analysis into Excel, and so on.

> _Is this a one time analytical study or a resuable model?_ <br>
> _Does the delivery include a customer facing application with a user interface?_ <br>
> _Are there any specific capabilities or functions the sponsor has requested?_

<h4>KPI/Performance Metrics</h4>

Also under the header of Success Criteria, we want to be very clear on what is an acceptable level of performance.  There should be no ambiguity when we get to this stage after completing a project.  We should know at the onset what outcome will be considered acceptable, and what result would cause our solution to be rejected at the conclusion.

There are typically units of measures and standard Key Performance Indicators (KPI), or functional business metrics, which are already top of mind for the business.  In sales forecasting this might be mean absolute percentage error (MAPE), in manufacturing production it might be critical failures, and in human resources it might be employee retention.  

> _What are the key metrics used to measure the impact of the solution?_ <br>
> _What are the specific attainment levels of the KPI that need to be achieved (benchmarks or improvements)?_

It's unlikely you'll have to search too hard to uncover the metrics the business cares about.  Where it gets a little tricky is trying to uncover what "good enough" looks like.  Is it a 5% reduction in error?  Maybe 7%?  Or just anything better than what their current process achieves today?  Maybe it's some combination of performance being at least on par with the current method, but also the time savings that come with the automation of the activities?  And so on.

The recommendation is to focus less on specific target improvement values, but instead on any improvement over the benchmark of the existing process in place today. 
 For example, if today 10% of our shipments are considered "late" by our customers and the cause of \$5MM in late fees, our KPI measure of success could be to reduce the percentage of late trucks to less than 10% by any margin over the next 12 months.  In other words, we build our predictive model that identifies shipments which have a high probability of being late, task someone in transportation to take some preemptive actions designed to keep them from actually being late, and then at the end of the year if our percentage of late trucks is less than 10% by any amount, BINGO!  We've succeeded!  By virtue of simply beating the current KPI rate, we should naturally see the \$5MM chargeback value be reduced.

```{tip}
The simple value in advanced analytics is to give the business something better than what they have today.  That's it, and it doesn't need to be any more complicated than that.
```

<h4>Resource Requirements</h4>

Work gets completed through people and teams.  Often resources are pulled and shared across functional business units and managerial lines, so we regularly have to deal with complications arising from conflicting priorities and time allocation, i.e. what associates are expected to spend effort working on for some period of time.  Managers are always fighting for, and to protect, their resources.  First, we want to make sure someone is not over allocated and being asked to do too much since there are only so many hours in a day.  Secondly, we need to make sure that if we plan for someone to be on a project, that we can trust and depend on a certain number of hours each week to be dedicated towards that project, which allows us to manage our timelines effectively.

With a chartered project, we have a formal allocation of resources and an expectation of committment.  If an associate is added to a charter as a project team member, then I know their supervisor has approved their allocation of time to my project.  In addition, we want to assign roles and responsiblities to each team member so we're clear as to who's doing what.  A nice encompassing approach is to use what's know as a RACI (Responsible, Accountable, Consult, Inform) framework.  RACIs clearly delinate the various personas on a project and make it easier to understand expectations for their involvement.

<h4>Project Plan</h4>

Lastly, you will need to be able to build out at least a high-level time line for the work.  For the audience we're communicating to with a Project Charter, we're generally only concerned with major milestones or stage gates.  These are the places in your project where you will have completed some major piece of effort, are advancing to a new bucket or section of work, or want to set hard go/no go checks and balances in the plan that require certain conditions to be met before advancing to the next action items.

These line items will of course vary by project, but often they will share many of the same high-level steps regardless of the specifics.  It can be a good idea to start with the following, and then tailor to the specifics as needed.

1. Kick-Off (milestone)
2. Design & Build
3. Stakeholder Approval (stage gate)
4. Deployment
5. Hypercare
6. Results Share Out (milestone)

You will likely need a much more detailed plan behind the scenes to manage the day-to-day activities for the team, but something along the lines of above will give your stakeholders enough information to understand the time associated with your expected progess.  Any changes, or potential risks, to the plan should be communicated swiftly and transparently as appropriate.  

**<h3>What Did We Learn?</h3>**



