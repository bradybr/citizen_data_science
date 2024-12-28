# Fields of Study

Next up, we'll take a look at the knowledge bases and fields of study involved with data science.  {numref}`ds-venn-fig` below is a very common Venn diagram illustrating the composition of a data scientist.  This little graphic will take us a long way towards understanding what we're talking about, so let's jump in.

```{figure} ../images/data_science_venn.png
---
width: 400px
name: ds-venn-fig
---
Data Science Venn Diagram
```

Consider these as the building blocks of knowledge that allow us to solve business problems in creative and impactful ways.  The challenges that obscure an easy definition here are the overlapping fields.  If you hear someone say they fix car engines, then it's easy enough to guess they'd be a mechinic.  There may be many variations of specialties as a mechanic, but essentially you can draw a mental picture of what someone who fixes car engines does.  Same goes for if I told you I teach English.  I may provide English lessons via a web course for non English speaking refugees, but I'm still a teacher in the simplest terms.  For data scientists, there are several overlapping fields front and center so unfortunately it's a bit more convoluded.

**<h3>Math & Statistics</h3>**

Firstly, _Math & Statistics_ are paramount, as you're hopefully starting to pick up from the examples thus far.  There are many flavors of mathematical specialties involved, which in my opinion is one of the main points that make us distinct from other analytics practitioners.  Data scientists are expected to be able to work across a large number of disciplines, whereas others may specialize in just one, or maybe two, fields of study.

There are a few core sets of mathematics which underlie a great deal of the methodologies you would come across in the field.  You certainly could get away with being pretty dangerous by simply using packaged functions and algorithms _without_ understanding what's going on under the hood; however, if you really want to do your best to protect from making untrustworthy assertions, you would be well served to become at least somewhat comfortable with the following:

 - Probability Theory
 - Information Theory
 - Frequentist/Bayesian Statistics
 - Linear Algebra
 - Calculus

The early pioneers and practitioners of the field primiarly came from this set born out of academia, and were mostly mathematicians and scientists.  They were doing this work by hand and with early generation computers that could only do a tiny fraction of the computations that we take for granted today.

If you talk to a 20 year veteran of engineering or statistics, you may hear them say they were doing data science work before it was the sexiest job of the 21st century, and that's because they very well might have been, by way of supervised learning regressions most likely.  At this current and more developed stage of the field however, there are likely pieces of the puzzle missing from these early traditional practitioners toolkits, which is where we go next.

**<h3>Computer Science</h3>**

For years and years the math was the secret knowledge that made us look like superheros.  We could do things not many had seen before or understood, and we simply hacked together the backend architecture without too much worry.  As long as it worked;  that's all we cared about.  Companies of any significant scale today are past this wild west era.  Today, understanding machine learning is pretty common and considered table stakes.  The real secret knowledge at present time is with those that can keep pace with the never-ending changing technology.

Technology is the conduit by which all of our cool mathematical theory sees the light of day.  There's a high bar of expectations that any data scientist be knowledgeable and capable in a wide range of tech.  Peruse any data scientist job posting today and you'll likely see a laundry list of technologies, architecture ecosystems, and programming languages required.  While not exhaustive, below is an example of what you might run across when searching.

 - Experience within the Microsoft Azure ecosystem (e.g. Data Lake, Delta Tables, Data Factory)
 - Experience with Data Bricks environment
 - Advanced Python, NumPy, Pandas, scikit-Learn, TensorFlow
 - Advanced MLOps capabilities
 - Experience with Snowflake
 - Experience with Kafka
 - Experience with Git/Github code management
 - Experience with DevOps

Kind of scary, isn't it?  Don't worry thogh.  It's actually pretty rare for one person to be extremely proficient in everything.  Technology continues to move at break neck paces, and it takes years of hands on practice to gain experience and expertise.

We'll cover aspects of these details later, but for now, just understand that these CS requirements can generally be broken down into categorical buckets like below.

 1. Programming language
 2. Programming environment
 3. End-to-end architecture/infrastructure/networking systems
 4. Code/Project management systems

**<h3>Domain Knowledge</h3>**

Now the last of the outer ring in {numref}`ds-venn-fig`: Domain Knowledge.  The importance of this contributing set cannot be overstated.  We'll discuss this in detail when we get to project overviews, but understand this is one of the main reasons projects fail.  On one hand you have highly skilled problem solvers armed with advanced methodologies, but most likely fairly ignorant of the domain area in which the problems come from.  On the other hand, you have highly competent functional resources who understand how their operations work, but usually have little insight into how to solve their problems with any of the advanced solutions we use.

It's very common to find one person working in the data science field that's skilled in math & statistics as well as the CS space; however, it's far less common to find an individual extremely capable in math and statistics, CS, _and_ domain expertise.  This of course depends on the type of experience and background of the individual, but as a "jack of all trades" type of generalist data scientist, you'd rely heavily on bringing in domain expertise from the function you're working with where the problem and project originated.

Here's an example to make this more concrete.  A transporation logistics department has a need for an application that can build consolidated shipments from all of the individual orders that come into their system, all with different requested arrival dates and destinations.  This seems simple enough.  You just need to know the the total weight of each individual order, the maximum weight a truck can hold, and then one of those fancy optimization algorithms, right?  Well, not so fast.  Did you know that Customer A orders cannot be grouped on the same truck as Customer B orders?  And did you know certain products cannot be double stacked on the truck, so you'll have to leave dead space above them?  And what about having to pull in orders planned to ship over the weekend to ship on Friday's?  And so on...  If you went ahead and built a solution without taking any of these domain specific condsiderations into account, then I can tell you from experience that your solution will be rejected because it does not meet the needs of your sponsors.

So unless you plan on working in every single department or role for a few years before you build any projects for them, it's extremely unlikely you'll be able to serve as the functional domain expert all of the time.  We need to work alongside of our project sponsors and functional working teams to make sure we consider all of the exceptions, constraints, and rules necessary to solve any problem adequately.

At this point we've covered the outer ring of {numref}`ds-venn-fig`, which are the general fields and knowledge bases.  As we get closer to the center of the diagram we're starting to get more specialized and data science specific.  We won't spend too much time on them here since the remainder of the course is mostly dedicating to covering these topics, but let's at least hit the highlights now because it should help round out our understanding of what we've been building towards.

**<h3>Machine Learning</h3>**

As you'll come to understand further, the application of specialty mathematics is a major part of what we do.  Where math & statistics and computer science overlap gives us what's known as **Machine Learning**.

```{note}
_Machine Learning_ is the application of code, algorithms, and data, giving computers the ability to learn and perform a variety of tasks.
```
<br>

Tightly coupled with the types of analytics we've already covered, you'll learn there are groups of methodologies that allow us to teach our models to learn and find patterns, which ultimately gives us the ability to solve our problems.  For example, to solve a Prediction problem previously discussed, we may choose to employ what's known as a _Classification_ algorithm from the Supervised Learning group of machine learning methods.

Our machine learning methodologies will generally fall into one of the three buckets below.

1. Supervised Learning
2. Unsupervised Learning
3. Optimization/Reinforcement Learning

Supervised Learning is a collection of techinques designed to learn from historical observations where you know the answer.  For example, there's a well known dataset called the Iris set {numref}`iris_table-fig`, which contains the petal and sepal measurements of 150 individual Iris flowers from three different species (Iris setosa, Iris virginica and Iris versicolor).  In addition, there's a column of data called "Species", which gives us our known truth label (what kind of specie the flower sample is).  Our classification algorithm is going to learn the different sizes of each feature which will allow us to separate between each of the three species, which we could subsequently use to make predictions on new examples where we _do not_ know the answer.

```{figure} ../images/iris_data.png
---
width: 700px
name: iris_table-fig
---
a) Fisher's Iris Dataset with known labels (Species), b) New observation example (no known label)
```

Unsupervised Learning is similar, in that our algorithms look for relationships and patterns, however here we do not have a ground truth label to learn from, such as the case with our clustering examples where we wanted to uncover hidden associations.  And lastly, we've already discussed Optimization and Reinforcement Learning briefly when introducing Optimization as one of the problems we can solve.  These are generally about providing the best possible decisions after trying to maximize or minimize some reward or penalty, respectively.  More complex cases involve multi-step decisions made over time, as sequential learning tasks under uncertainty.

More to come on these topics.

**<h3>Research</h3>**

This one was a little foreign to me coming from a business background.  Where math & statistics overlap with domain expertise, we get _Research_.  Now this doesn't mean you're going to be conducting trials and writing research papers, but it does mean you should understand some of the same tests, methods, and rigor that academic and scientific professionals balance.

For example, let's say you're trying to prove a statistical link between smoking and cancer.  Seems pretty obvious to us today, but did you know that it wasn't until 1954 that scientists were able to satisfingly prove the causal releationship {cite}`Mendes_2014`?  It's a high bar to say something _causes_ something else from a statistical point of view.

Since you'll be using a lot of the same statistical methods and making a lot of the same kinds of inferential statements based on your models, there are some well documented steps and protocols you should be aware of and follow as best as you can.  Have you heard of the scientific method?  See {numref}`scientific-method-fig`.

```{figure} ../images/scientific_method.png
---
width: 400px
name: scientific-method-fig
---
The Scientific Method
```

You'll be introduced to a lot of these related topics as we progress through the course - experimental design, controlled testing, small sample size, confounding and lurking variables, counterfactuals, omitted variable bias, overfitting, repeated trials, hypothesis testing, confidence intervals, just to name a few.  I know.  Sounds scary if you've never heard any of this.  Don't worry though.  Baby steps.

**<h3>Software Development</h3>**

Lastly, we get to _Software Development_ where computer science and domain expertise overlap.  What work is involved will of course depend on where you're working, what technology architecture and systems you're working with, how large your team is, the roles and responsibilities for each, and which resource is expected to complete certain tasks.

I personally think "Software Development" is a confusion choice of wording here.  We definitely need to understand software and CS applications; however, in my experience _development_ is a bridge too far.  Few data scientists are relied on heavily for traditional software development or the building of robust web applications.  Certainly there's a flavor of software application development that we deal with, in that our programs can be at the heart of these applications. 

We also need to be involved in how we're going to expose, or make our back-end programs accessible to the end users via some kind of user interface.  So from this angle, absolutely software development is not entirely off our plates.  We'll cover this in greater detail when we get to data science personas and roles, but for now understand that someone will need to own building, testing, deploying, and maintaining the final solution the team has built.  

In my experience, the data scientists on the team are typically expected to be able to build simple prototype web apps, or possibly even the final application given it's in a well structured environment.  Outside of this, the responsibility for production deployment typically falls to someone more aligned with with what's known as MLOps or Data Engineering.

Another point worth mentioning is that we often get so caught up in the process of proving we can solve the problem, that we fail to devote enough time to the user experience.  Someone will need to think through some pretty standard questions when you begin talking about using your solution in practice.

 - How will the users interact with our solution?
 - What buttons will they want to push?  Levers they want to pull?
 - Will there need to be any dynamic graphs or visuals?
 - Will it be a web app?
 - Are we deploying in the cloud or on premise?
 - Does it need read/write back functionality?
 - Will it need to be fed a constant stream of new data?
 - And so many more questions. 

This topic will come up again under the Skills and Tools section coming up soon.
