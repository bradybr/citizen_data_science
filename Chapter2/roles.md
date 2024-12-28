# Roles

Now that we have a bit of an understanding about what data science is and what we do, it's time to dig a bit deeper into the personas and roles that make up a mature advanced analytics team.  Every company and team is different, and their investments into tools and technologies will play a large part in what a team is capable of doing and what roles are required.

Job titles matter.  They matter to an individual's self identity, their reward for years of study and experience, and for aided comprehension and understanding of the expectations of the resposibilities tied to a position.  Unfortunately titles do not guarantee any kind of standardization across industries, so we get often get the same confusion we ran into with trying to define what data science is.

This course will focus mostly on the capabilities of a citizen data scientist and being self sufficient, but it's a good idea to discuss all of the peripheral roles one would encounter in the real world.  Again, there's significant overlap so it'll be a good idea to undertand what "common" looks like.  Titles, roles, and responsibitliies are constantly evolving with new technologies and business expectations, but what follows are fairly well established at this time in the industry no matter where you find yourself.

```{figure} ../images/data_science_roles.png
---
width: 900px
name: data_science_roles-fig
---
Common roles and workflow in an advanced data analytics team
```

This list could get out of hand if we're not careful, so let's try to keep it simple and high-level at this stage.  From {numref}`data_science_roles-fig`, below are some of the common roles and personas you might run across in the field.  We'll tackle them one by one and highlight what you could expect to see.

 - Business/Data Analyst
 - Business Architect
 - Data Engineer
 - Machine Learning Engineer/Machine Learning Ops Engineer
 - Data Scientist

**<h3>Business/Data Analyst</h3>**

We start here because these associates are generally the front lines of analytics in any business, and not so coincidentally, the persona which aligns the closest with a citizen data scientist: Business/Data Analyst.  These associates are often generalist and experience varies across industries.  The title Business Analyst can be a catch all for hiring entry level associates without specialized expertise, beyond general business knowledge.  Of course this depends on the specifics of the role and sector.  For example, an analyst working in a goverment post is typically a highly educated, skilled, and specialized resource.  So again, expect differences and your mileage may vary.

Business analysts are embedded within a specific business function, i.e. Supply Chain, Sales, Marketing, Consumer Insights, and their primary responsibilities are to support that function.  When leadership needs to understand their business, these resources get the phone call to help provide the insights needed.  Value and speed (i.e. time-to-insights, or how quickly the analysis can be completed) are generally of paramount importance here.  Their analytics typically do not need to be pretty or complicated.  What matters is getting to the insights quickly.  

Get the data, run some simple descriptive statistics that shed light on what's happened, then share the information quickly.  Rinse and repeat.  After you enter into the corporate workforce, you'll learn the dirty little secret that even multi-billion dollar companies essentially run on Microsoft Excel and PowerPoint.  This is a time tested workflow for analytics that works.

```{tip}
Value can be found by anyone in an organization, and not everything requires complicated methods from specialists.  If you can find value by running a report, dumping it in Excel, running some simple descriptive statistics or visual methods, then that's nothing to sneeze at.  Things do not have to be complicated.
```

```{figure} ../images/xls_screen.png
---
width: 800px
name: xls-screen-fig
---
Simple Excel analytics
```

These resources are very common in business circles.  They're leaned on heavily and spend a signficant amount of time pulling data, compiling summary statistics, and ultimately publish their findings and recommendations in easily consumable ways (hopefully).  Our course is largely centered around upskilling these associates and enhancing their analytical skills and capabilities to provide even greater value to their organization.

**<h3>Business Architect</h3>**

With Business Architects we begin to move towards a specialty within analytics, however mainly from the _business_ side.  These associates tend to be much more knowledgeable about the broad field of analytics though.  This covers a technical understanding of what other roles and personas are doing, as well as the technology and methodolgies involved.  With analysts in general you tend to get a lack of understanding of what data science resources can do, and with data science resources you tend to get a lack of understanding of how the business works.  The Business Architect role typically fills this gap between business strategy and technical execution, and will play in between these parties.

These associates are generally not the ones performing analytics themselves, but more so work in business or program management, organizational communicatory, and consultancy capacities.  This is also a role is often missing with companies that are farily immature in their analytics journey, since these responsibilities can be assigned to and performed by other resources (arguably not as well though).  

**<h3>Data Engineer</h3>**

Now we get to someone you should definitely run into in any organization actually taking advanced analytics seriously.  Data Engineers are a critical member of any data science team.  These associates tend to be heavy on the CS/IS/IT backgrounds, and often less specialized in the advanced mathematics we employ, machine learning, and basic data science methodologies.  This is actually not such a bad thing though, seeing as your prototypical data scientist will not be as proficient in the skills that a data engineer brings to the table.

So what do they do?

- Data acquisition & storage
- Data ETL (Extract, Transform, Load), wrangling, munging, and aggregation
- Database management
- Create and maintain pipleine architectures
- Data governance, security, and compliance

What's so great about these team members in my experience is that they tend to compensate for the lack of skills held by the more mathematically inclined on the team.  This goes back to the idea that it's much easier to find a data scientist that has expert achievements in one or two of the three (math & statistics, CS, and domain expertise) main skillsets.  So for me personally with my background in business operations supplmented by advanced mathematics - New technology, hardware, networking, and architecture can be difficult for me since I'm not a CS person by any stretch of the imagination.  Having someone on my team with these skills is worth its weight in gold.

Data Engineers historically were the CS folks coming with advanced skills in SQL and probably some of the older languages like COBOL, Pascal, or Fortran.  Today, SQL is still the dominant structured language, and Python has taken over the world as the most used general purpose language.  These are probably the most common of what you'll see in the wild now.  With all of the new era/big data technologies evolving, be prepared to hear about new languages at a pretty constant rate (e.g. MQL, NoSQL, Spark, Scala), and these associates are key to working with them effectively.

**<h3>Machine Learning Engineer/Machine Learning Ops Engineer</h3>**

Those in-the-know out there may have some words for me for lumping these two together, but bare with me.  It's simply easier to explain how these two are similar and where they differ all at once.  It is unfortunate though that these two are so similarly named since it does creates some confusion we have to deal with, but like everything else up to this point you'll get differences depending on the industry and company anyway.

```{figure} ../images/ml_ete.png
---
alt: ML roles
name: ml-roles-fig
class: bg-primary mb-1
width: 500px
align: right
---
End-to-end ML roles and responsibilities
```

First let's talk about the overlap here.  ML Engineers actually have more overlap and in common with data scientists than MLOps Engineers if you ask me.  The main difference is that the Engineers are much more capable and focused on the _productionized optimization_ of the models we build, seen more on the center-right side of {numref}`ml-roles-fig`.  These resources tend to be a bit more in the CS circle of our Venn diagram vs. the Math & Statistics set.  In my experience, we see less of them on the upfront business collaboration side of projects vs. the building, iterating, and deploying solutions, but they are definitely capable of owning a project from inception.  They understand how the models should work in the tech stack and architecture we're dealing with, but better still, how our models and data should work most efficiently and effectively in these environments.  This is their sweet spot.

MLOps Engineers have their main overlap with the ML Engineers focusing on the same productionization of their models and their deployment.  We can think of these resources as hyper-focused on deployment after the model development, monitoring/maintenance, and iteration cycle of tuning and optimization of the system architecture at scale.  The main points of distinction between ML Engineers and MLOps Engineers is that ML Engineers will tend to be much more involved in the model development cycle or handover from the Data Scientist, vs. the MLOps Engineer who cares mostly about the complete back end deployment.

**<h3>Data Scientist</h3>**

And finally, we arrive at the Data Scientist on the team.  This title is slowly falling out of favor for more specialized versions that take more of the technology and systems architecture into account, like what we see with the rise of ML Engineers.  Data Scientists were the main expansion out of the traditional math set of folks doing this work roughly 15-20 years ago, and were generally the first ones solving business problems using these new machine learning methodologies (outside of highly specialized and isolated pockets).  These resources quickly proved concepts and value with prototypes without overly worrying about how it was going to be deployed, or whether or not the model was optimized to scale.  

At that time, the end-to-end process and landscape looked very different than it does today.  Today we have new cloud architecture, innovation sandboxes, CI/CD processes, data movement pipelines, federated data, and so on.  All of this has created the need for the Data Scientist to evolve.  It's no longer enough to just be able to build a simple machine learning model on your laptop.

So where does that leave the Data Scientist today?  Titles come and go, and this one will probably fall by the wayside at some point not so far into the distant future, but the intent of this persona is still going strong in my opinion.  What companies desperately need are resources that can interpret the problem context from the functional business person, propose solutions, and then quickly mock up a minimum viable product (MVP) or prototype model to prove the value of a concept (POC).  They need knowledgeable advanced analytics resources that are able to translate complex topics like math and computer algorithms into simple business layman's terms.  All of these things are still the primary strengths of a data scientist and are not in danger of disppearing anytime soon.

A frequent scenario was for the data scientist to fill this up front space working with the business sponsor all the way to building a POC prototype, and then handing of their work and models to the ML Engineers to package it up for production deployment.  Today this still fits nicely with the emergence of these new specialized roles on the back end, but I do believe there's been a shift to an expectation of being much more knowledgeable and capable with the technology and architecture further down the workflow chain than we've seen historically.

Of course all of this is fluid and only broad generalizations of what I've experienced or have read about in the industry for the last 10 years up until now.  There's certainly no reason that an ML/Ops engineer couldn't or isn't working up front with the business, or that an ML engineer doesn't work on prototype developments, or that a data scientist can't build a production ready model and see it through deployment at scale, etc.  

```{tip}
The only thing I can guarantee you is that change is the only constant in this field.  Be as open to refreshing your mental models and understanding as possible.
```

To close the loop on this section, remember that the intent of this course is to take some of the specialized knowledge from these advanced analytics associates, pare down their expertise and methodologies to just the essentials in an easy to understand manner, while simulatenosuly elevating the front-line business analyst to that minimum level.


