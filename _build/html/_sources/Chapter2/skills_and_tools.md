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

# Skills & Tools

Coming on the heels of learning which fields of study are involved in the application of data science, is the just as important topic of what Skills and Tools one would be expected to use.  Don't worry though, it's about to start getting fun.  At this stage we start introducing practical tools you'll be able to start playing around with instead of just more theory and conceptual topics.

The landscape of tools and technology looks so radically different today than it did just 10 years ago, that I'm constantly reminded how quickly we move in this space. 
 Years ago, practioners would have most likely come up through a mathematics, engineering, or science department at university and learned theory, methodology, and how to use some commercial software tool during that time (whichever was paid for by your university).  Post graduation, you would have found a company looking for a practioner capable of using the software program you learned in school, and then you would have been all set for a career.

Open source technologies have seriously changed the game since these old days.  Open source essentially means the source code of the program, which allows it to do what it does, is available for you tp see, modify, and/or distribute under its license, all for free.  This is in stark contrast to commercial applications which cost money to use, usually not an insignificant amount I might add, and you're generally not allowed to view or modify how it works.  There are communities of users who maintain these open source code repositories with a rigorous testing and comittal process, but the general idea is to leverage the synergy of active users contributing to the functionality of the language or tool.  The benefits and the ways these communities have changed the world around us cannot be overstated.

Today, you have an amazingly deep pool of powerful tools to choose from at your disposal, generally supported by an active community of users willing to help you learn.  Definitely take advantage, and hopefully give back where you can.

Now finally, let's get to the landscape of tools and technologies that allow us to do what we do.  The majority of what you'll need to start making an impact falls under the following buckets:

1. Analytics Platform
   - Programming Languages
   - Integrated Development Environment (IDE)
   - Low/No Code Applications
2. Code Management
3. User Interface/User Experience (UI/UX)
   - Front-End Application

**<h3>Analytics Platform</h3>**

Data science and machine learning doesn't just come out of nowhere.  This is the _where_ and _how_.

Whether you code it yourself or an application does the heavy lifting for you, our work involves math, code, and some kind of development platform.  This is where all of the magic happens.  Our focus here is of course the Citizen Data Scientist and not the professional Data Scientist; however, I would be remiss if I didn't lead with the following suggestion.

```{tip}
Learning to code and becoming proficient in any number of programming languages will pay huge dividends in your ability to be productive and effective in this space, regardless of the application or tools you choose to use in practice.
```

<h4>Programming Languages</h4>

Let's start with what the majority and professionals are actually using.  If we're talking about pure developer programming languages overall, you can see from the Stack Overflow 2024 Survey {cite}`SO_2024` in {numref}`so-langs-fig` that the top spots are geared towards web development with Javascript and HTML/CSS.  The 3rd spot however is where we come in with over 50% of the respondents citing python (PY), in response to the question **"Which programming, scripting, and markup languages have you done extensive development work in over the past year?"**

```{figure} ../images/so_langs.png
---
width: 1000px
name: so-langs-fig
---
Source: https://survey.stackoverflow.co/2024/technology/
```

Python is an extremely flexible general purpose coding language, which has been extended with a super robust library of add-on functionality to make it the undisputed king of the hill for professional machine learning practitioners, as well as novices and hobbyists alike.  If you plan to become more of a full fledged programmer or data scientist, then you can't go wrong learning python.  Visit <a href="https://www.python.org/">Python.org</a> to learn more. 

I would also suggest you get started using python through an <a href="https://docs.anaconda.com/">Anaconda</a> distribution though if you're going this route.  You can read up in the docs, or you'll come to understand the benefits of its package manager and add-ons if you get into actual coding.

Additionally, there are a handful of other languages you may be interested in familiarizing yourself with if you plan to go the coding route.  These recommendations will cover basic general purpose scripting, math and statistics, data science and machine learning, database connectivity, as well as more advanced operations dealing with cloud computing, and distributed and parallel processing.  There are tons of free and paid resources available via books, tutorials, and web courses to learn any of these and others.

1. <a href="https://www.python.org/">Python</a> (<a href="https://docs.anaconda.com/">Anaconda</a>)
   - NumPy
   - Pandas
   - matplotlib/seaborn
   - scikit-Learn
2. SQL
3. PySpark
4. Scala

The majority of the analytics, graphics, and coding images in this book have been created with python, however we'll focus on an analytics platform called KNIME for our Labs and Exercises coming up, just as soon as we cover IDE's in this next section.

<h4>Integrated Development Environment (IDE)</h4>

After you have your favorite language picked out, you'll need a place to do your work.  Enter the text editor or integrated development environment (IDE).  You could actually do all of your work in a plain text file and use the comand prompt if you're one of those kinds of programmers... I am not unfortunately, and am only comfortable there when I need to be.  So for me and many others like me, we need applications with all the bells and whistles that make coding more efficient.  With these applications we'll get awesome utilities and benefits like control over run-time execution, debugging, syntax highlighting, linting, object explorers, etc., that make our lives so much easier.

You'll have a couple of choices here depending on your preferences and needs, and they generally shake out into two camps: 1) Web notebooks and 2) Desktop applications.

**Web Notebooks**

Web notebooks are excellent choices when you're learning, teaching, sharing, in development, or prototyping.  There are plenty of choices and different flavors, but when we talk the most common, you'll probably run across the following.

- <a href="https://jupyter.org/">JupyterLab</a>  (<a href="https://docs.anaconda.com/">Anaconda</a> distribution)
- <a href="https://colab.google/">Google Colab</a>
- <a href="https://www.databricks.com//">Data Bricks</a>

```{figure} ../images/jupyter_ex.png
---
width: 900px
name: jupyter-ex-fig
---
JupyterLab notebook excercise example
```

It's worth mentioning that when you get out into the corporate arena and start seeing end-to-end production infrastructures, you'll likely run into the difference between coding by yourself in isolation and coding designed to scale within a team.  Certain front and back-end environments and platforms will make more or less sense depending on the composition of your team, your financial resources, and what you're trying to accomplish.  

**Desktop IDE's**

If you start getting really serious about building bullet proof applications in a "pythonic" way, you may realize the online notebooks sometimes may make it a little difficult to do so.  Production applications are built and deployed in notebook environments like Jupyter and Data Bricks, but you may find it's often easier to develop and manage your code at certain steps using an IDE.  These tools come with more functionality and a different template compared to the notebook/cell varieties.  In those cases where it may help to move out of a notebook environment, you may want to start looking into local installations.  Below are just a couple of the most popular, and all three come with the Anaconda installation as well.

- <a href="https://www.spyder-ide.org/">Spyder</a>
- <a href="https://code.visualstudio.com/">VS Code</a>
- <a href="https://www.jetbrains.com/pycharm/">PyCharm</a>

I personally love Spyder as my IDE of choice because it comes with a variable explorer natively, which makes is much easier to investigate and monitor your progress.  VS Code and PyCharm are more popular by far, although I personally find them less intuitive and user friendly for some reason.  You aren't locked into choosing just one, and can switch back and forth as you'd like since they're not cloud or web environments, so feel free to play around with any or all.

```{figure} ../images/spyder_ex.png
---
width: 900px
name: spyder-ex-fig
---
Spyder IDE with local .py file example
```
Again, since our objective in this course is the citizen data scientist for quick wins with business analytics, you can actually skip the coding languages and IDE's all together if your intent is to get right down to it and starting returning value quickly.

```{tip}
The detailed explanation of the professional toolkit involving programming languages and tools was for the benefit of comprehensiveness, but make no mistake, you can still provide quick wins with advanced analytics without being a master coder or learning tons of new applications or technology.
```

For the determined analyst and citizen data scientist, our recommended vehicle for getting you in the game quickly is where we go next with Low/No Code Applications.

<h4>Low/No Code Applications</h4>

Now for the fun!  If the idea of opening a text editor to a blank screen and being asked to "go write some code" doesn't sound appealing to you, you're going to love this.  There's a whole host of tools and applications available that allow you to explore and visualize data, build exploratory models, and even deploy your applications, all from a user-friendly drag and drop kind of interface without needing to code.  These kinds of tools and applications are generally referred to as low, or no code applications. 

There are lots you could choose from, but we're going to recommend <a href="https://www.knime.com/">KNIME</a> for it's ease of use, open source community, and end-to-end capabilities.  Below in {numref}`KNIME-fig` you can see what's known as a workflow in the KNIME application.  This is your home base for building a model or analytical study, via connected "nodes", or steps, of the end-to-end process.

```{figure} ../images/KNIME.png
---
width: 900px
name: KNIME-fig
---
KNIME Analytics platform workflow
```

The idea with these kinds of model building tools, is for you to spend the majority of your time thinking about the business problem and the value in quick analytics, versus spending all of your time enmeshed in the nitty gritty behind the scenes details of model building.  Don't get me wrong, these behind the scenes details are extremely important; however, what these applications have done is abstracted away the complicated and nuanced decisions we have to make, by using intelligent automation and exposing the places where you can make selections via simple drag and drop screens.  

All of our Labs and Exercises will be built using KNIME, so we'll postpone getting into the details until then.  There's plenty of hands-on exposure coming soon.

**<h3>Code Management</h3>**

Next we discuss code management.  This section will be more applicable to the professional data scientist vs. the citizen, but we will cover it briefly in an attempt to be thorough in outlining the complete toolkit in the data science space.

So what are we really talking about?  Code management involves the notion of keeping master files separate from developmental files.  It allows a team to edit offline, track changes, implement tight version control, revert to a previous copy if needed, and enables multiple people to work on the same project at the same time.  Pretty cool stuff.

There are a couple of extremely common tools here that nearly everyone you'll run into uses.  First is Git, which is the actual version control system used under the hood.  Next is Github, which is essentially built on top of Git and gives you the UI tools and framework to create repositories of code and notebooks.  Feel free to start reading the user docs to get a sense of the basic functionalities they offer.

- <a href="https://git-scm.com/">Git</a>
- <a href="https://github.com/">GitHub</a>

```{figure} ../images/git_workflow.png
---
width: 900px
name: git-workflow-fig
---
Git workflow example staying in sync between Github and local files
```
We won't go into further details in this course, but you should be able to get the idea from {numref}`git-workflow-fig`.  There's a master repository, called a "repo", where everything is either being pulled from, or pushed to.  You can pull down the current version, work on making updates and changes to the code, and then send it back to be approved for inclusion into the main repository.  All of these updates and changes are annotated, tracked, and capable of being reversed if needed. 

Imagine a simple example of a production model saved to our main repository.  This model, code, and notebook have been tested and approved by the team, and committed as the current version.

$$
y\hat{} = \alpha + \beta_1(x_1)
$$

Now, let's say you work on this team and had the bright idea that we should add the effects of a second feature to make better predictions, like so,

$$
y\hat{} = \alpha + \beta_1(x_1) + \beta_2(x_2)
$$

You would simple pull down the current version of the code to your local files, make the change and validate your idea, and then finally "push" your changes back to the admin for approval and committal of your updates so they become part of the new version of the main code.  Of course it gets much more complicated in real life, but hopefully you get the idea.

At the end of the day, this code management process allows a team to work more efficiently on the same project at the same time.  It also ensures everyone is working on the most current version, avoiding unnecessary conflicts, and there's also a clear process for testing and allowing updates to be made safely without the dangers of losing the last known working copy.


**<h3>User Interface/User Experience (UI/UX)</h3>**

Now we get to the user interface (UI) and user experience (UX).  Far too often these ideas are left until the end of a project, which is a mistake in my opinion.  You should have a clear understanding up front of how the end users expect to be able to access and work with your solution.  They likely will not be comfortable reading code, working in any of the technologies we've discussed thus far, and therefore will need a much more business friendly GUI and front-end to interact with your program.

The basic idea here is that when you're all done solving the business problem, users will likely need some way to upload new data, select dynamic inputs, or to simply run your program on demand.  Not every project in the real world will need a front-end like this, but in cases requiring interactivity from your end users, your application will need to be "live" and deployed to the user in some way.  There are tons of ways this can be done, in technologies and applications ranging from simple to complex.  

Let's start with the first consideration though: The User Experience.

The **UX** is a wholistic understanding how the users will experience working with your application.  This is a never ending list of questions, but the central idea is trying to understand if you've reduced any friction to using your application as much as possible.  User adoption is a major issue in the real world, and you want to make sure you're doing everything you can to ensure the users _want_ to user your solution.

- Is the app intuitive and easy to understand?
- Is it natural navigating through the app?  Are there multiple tabs or pages?
- What functionality does the user need?  Dropdowns, list boxes, dynamic graphs, multi selection/cascading widgets, etc.?
- Did you create "How To Guides" and User Documentation?
- How will they user request support or report bugs?
- Are there any special security considerations?

The **UI** is the actual front-end the user will see when they use your solution.  There are few rules here beyond beautiful design principles, so whichever method or vehicle serves the end users needs is generally what we do, and these will look different for quick prototypes vs. in production.  You'll need to think about whatever you've built, and what that application requires.  For example, if I'm deploying a sales forecasting model that requires the previous month's sales dollars, then the UI will need a text box which allows the user to type in the dollar amount for the last month, assuming you haven't automated the data pull in the backend somehow.  In addition, if it's an application that's only run on demand when the users wants to use it, then you'll also need a button that activates or runs the program.

Some popular choices for quick and simple are shown below.  These integrate tightly with Python code and Jupyter Notebooks so there's typically little overhead to learning a new language or framework.  As before with the coding suggestions, these options are only necessary if you're going the more robust path of learning to code and needing to build your own web applications from scratch.

- <a href="https://streamlit.io/">Streamlit</a>
- <a href="https://dash.plotly.com/">Dash</a>
- <a href="https://bokeh.org/">Bokeh</a>

```{figure} ../images/streamlit_ex.png
---
width: 900px
name: streamlit-ex-fig
---
Streamlit web app demo example<br />Source: https://echarts.streamlit.app/
```

```{tip}
Good design and usability always start with thinking about the needs of the end user:  What does the user expect, and how will they need to be able to interact with your application to have those expectations met?
```

In our case as the citizen data scientist, you'll be able to provide users access to your application and deploy from the same low/no code environment you built it in, KNIME.  Stay tuned, we'll get there.


**<h3>What Did We Learn?</h3>**

This was again a lot of new ideas and terminology thrown at you without too much detail.  Don't worry if you're still not quite able to see the forest through the trees just yet.  We will get to all of these as we progress through the course.

As long as you understand the following for now, then you're right on track.

<h4>Programming Language</h4>

If you want to dive into the deep end and learn what the professionals use, there are a few core programming languages you'll want under your belt to get started.  Start with **Python/Anaconda** (plus NumPy, Pandas, matplotlib/seaborn, scikit-Learn libraries), then **SQL** as your second foundational language.

If you simply want to quickly power up your analytical skills in whatever domain you work in, then start out with a low/no code analytics platform such as **KNIME**.

<h4>Analytics Platform</h4>

You'll need an environment to build your solutions and programs.  If you're going the full coding route, start with **JupyterLab** for learning, prototyping, and dev work, but you may also consider investigating local IDE's from any number of choices (e.g. **Spyder, VS Code, PyCharm**).

If you're still on the citizen data scientist and quick value track, then stick with a low/no code end-to-end analytics platform like **KNIME**.

<h4>Code Management</h4>

While not completely necessary for the beginner or citizen data scientist, learning the basics of common code management tools could pay off in a number of ways.  If you're ever going to work on a team or with other more seasoned analytics practioners, if you would like to start building a public portfolio of your work, or if you think you may possibly move into more professional data scient work at some point, learning these tools would be a huge benefit.  The most popular are the **Git** and **Github** environments and frameworks.

<h4>UI/UX</h4>

And finally, you'll likely need to learn some ways to publish your solutions to your end users.  If you've built something from scratch in a coding language like python, start exploring and selecting a favorite web app option which allows you to continue in the same language you're comfortable with (e.g. **Streamlit, Dash, Bokeh, Panel**).

If you've gone the end-to-end analytics platform route with **KNIME**, then good news.  You're all set.  KNIME has this capability built in.

