# Introduction

As I sit down to write this Introduction, I'm returning from a one-day conference regarding _AI-Centric Factories of the Future_.  If I would have written this prior to, I'm pretty sure it would read differently than it's about to.  It's funny how your thinking can shift so easily sometimes.

```{image} ../images/ai_singularity.png
:alt: AI singularity
:class: bg-primary mb-1
:width: 400px
:align: right
```

Ever since ChatGPT blew the the public's blinders off as to the possibilities with what we do, the AI hype train has gone off the rails.  Despite this hype, not much has actually changed.  To the average person who didn't know anything about us before, it may seem like this all came out of nowhere and we've hit some kind of AI singularity milestone.  The reality is, we're still doing pretty much what we were doing before, just with more data, more computing power, and we've solved some of the limitations with the math we've been using since the 1950's.  So in effect, it's really just a newer and better natural language prediction model than we've ever had before.

The user interface over these generative pretrained models like ChatGPT which have been exposed to the general public is pretty cool though I have to admit.  And it's this user interface layer and prompt engineering which really is what's enabled the explosion of oppportunies, not what's behind the curtain with the math.  The advancements in the math are pretty amazing for sure, but without exposing and enabling its use via an easy to use wrapper for the public to consume, we would never be where we are today.

I see and hear comments every day like _"I used AI to..."_ something or other, and the technician in me can't help but want to educate or correct people when I hear misunderstandings of the methodologies and with what they believe is happening.  I'm fully aware my opinion doesn't matter and is just that, my opinion, and I have no desire to be the word police.  It has nothing to do with wanting to sound smart or placing value judgements on the activities of others either, and everything to do with battling a simple misconception which causes endless confusion.  The term "AI" has been co-opted and hijacked by the public to represent just one single use case, specifically "generative AI".

AI is actually an extremely broad umbrella term which as you can see below in {numref}`ai-umbrella-fig`, is not so constrained.  Working in the arena of AI could mean you're doing research to understand the ethical implications of the collective advancements we've made.  It could also mean you're involved in designing a new type of fluidless hydraulic system for a quadruped robot.  There's no end to the disciplines involved in the work going on under this umbrella of AI.  Saying you're going to solve a statistical inference problem with "AI", while understanding "AI" to mean a generative AI large language model makes little sense and wastes tons of energy in communication encoding/decoding.

```{figure} ../images/ai_umbrella.png
---
width: 900px
name: ai-umbrella-fig
---
AI fields of study, and Data Science use cases coupled with classes of mathematics
```

Generally speaking from the public and business perspectives, most often the usage of the term AI is intended to represent applied data science or machine learning.  Ok, so who cares if they misuse or misunderstand these words you might be asking, since data science and machine learning are actually under the umbrella of AI.  Well, this confounding of terminology is problematic for a number of reasons.  Primarily because large language models are a very specific class of mathematics for a specific purpose, and do not do what most people likely believe they do.  Technically, models such as ChatGPT are prediction models, but not in the same way a Classification model will predict an event or occurrence of something happening.  Large language models are predicting something called tokens, which can be thought of as simply which words have the highest probability of being strung together in some order that reflects how humans communicate and which will answer the query.  That's it.  It is not a replacement for the other types of solution classes.

If you can find value in these new tools, great.  Use them!  I think they're awesome and useful, I really do.  My feeling is entirely to do with I believe we've grown a massive chasm between how value is _actually_ created with these tools and methodologies, versus the _perception_ of how and where it happens.  This gap is causing us to focus on and talk about the wrong things, which only serves to confuse and make finding value more difficult than it already is.  Honestly at the stage we're in now, it feels a bit like two people coming to a table with two buttons on it, one red and one blue.  The first person wants to hear the details of the opportunities and then align which button to push based on how that problem should be solved, but the second person keeps saying _"just push the blue button!_".  

What matters today is the same as it was yesterday.  First, we must be able to articulate a problem or question with enough value in a solution that it warrants effort.  Secondly, we must align our stated use case with the "What do you want to do?" answers in {numref}`ai-umbrella-fig`.  We can do much more in the generative option today than we could before, but at the end of the day, there are still only a handful of buckets everything we deliver falls under.  Lastly, we need to be able to match up the problem with the technical solution and class of mathematics, and deal with all of the nuanced intracies involved in the process.  These are the steps that have always mattered and will continue to matter into the future for some time.

There is no all-knowing tool or methodology for all questions.  The core machine learning methodologies are still how we solve predictive and prescriptive problems.  If you want to forecast your sales for next quarter, _AI_ is not the answer.  If you want to predict if a high risk project will succeed or fail, _AI_ is not the tool for this question.  If you want to optimize your labor staffing and shift scheduling, _AI_ cannot provide the answer.  This will definitely change at some point in the future with the continued developments in Agentic AI, but we are not quite there yet.

Several levels below the term _AI_ is where practioners deliver value as you can see above in {numref}`ai-umbrella-fig`.  ChatGPT didn't change this.  Machine learning methods like classification, clustering, forecasting, and optimization are still very much what we do and where we'll continue to find tremendous value for the foreseeable future.  At some point we'll be able to expose their use in the same way as we've done with ChatGPT and other similar models, but this isn't on the table yet.  

All of this nonsense and jibber jabber about words and terminologies goes away if we focus on what matters - 

> Identifying business opportunities where we can enable better decision making, which allows for a more informed and analytically driven allocation of resources (human, capital, or otherwise)
> 

<h4>The Citizen Data Scientist</h4>

The machine learning methodologies we're going to cover in this course are the foundations of data science in practice.  Traditionally, the only people able to harness their power have been experienced professionals with deep mathematical and CS knowledge.  Today, the playing field has been leveled with advances in data accessibility, techonology infrastructure and processing, and analytical tools available to the general public which abstract away many of the technical complexities.

The intuition behind citizen data science is easy to grasp.  Imagine someone who knows how to count to 10 really well sitting at a desk.  Now imagine a line of 20 people queuing up who need the help of someone who can count to 10 really well.  Seems like a match made in heaven, right?  The first person from the line steps forward to the desk and is greeted with _"hi, how can I help?"_, to which this first in line replies with _"por favor puede contar hasta diez?"_  Oh boy.  Our helper, who just wants to count, is going to need to learn some Spanish first before she can help.  Worse yet, she comes to find out that all 19 of the other people standing in line waiting to ask for help speak 19 other different languages as well.  Better take a number because our counter is going to need some study time...

Instead of having only a few, highly trained and experienced professional data scientists delivering a handful of high-value projects each year, what if you could have 50 highly competent business analysts delivering hundreds of small to mid-value solutions each year?  Right!?!?  Now we're talking about seriously moving the value needle.

```{figure} ../images/citizen_data_science_idea.png
---
width: 900px
name: citizen-data-science-idea-fig
---
Professional vs. Citizen Data Scientist project creation model
```

The notion of a citizen data science community within an organization is going to empower those 20 people standing in line with the skills to solve their own problems!  They already know the details of their business environment.  All they're missing are some new skills and tools.  We're not talking about trying to turn these resources into professional mathematicians or engineers, more so simply upskilling advanced business analysts to answer specific types of questions in new ways.  

None of this replaces the need for full-time data scientists or productionzed analytics at-scale.  What it does is open the door for someone who owns and has responsibilities for a specific piece of a business to perform advanced analytics and deliver value quickly on their own.  Critical, complex, connected, or at-scale opportunities, should continue to be run the same as always, with people from different specialties and domains coming together joining forces to solve the problem.

If any of this introduction feels controversial or surprises you, then I hope you'll give me a chance to show you how _anyone can find value with advanced analytics_.  If we can simply focus on problem statements and use cases instead of walking around with a hammer looking for nails, there's dollar bills on the floor just waiting to be picked up!   

I've never been more convinced that analytics does not have to be complicated, and what follows is my attempt at pointing the way.

This is the theme of the book.
