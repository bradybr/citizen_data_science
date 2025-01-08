# Exploratory Analysis

We've finally got our data in hand and now we're getting to the fun stuff!

**Exploratoy Data Analysis (EDA)** is what we're talking about here.  Think of this as _ok, what's going on with what's in my data?_  It's really that simple.  What categorical variables do you have?  How many of them?  Do you have the right periods of time (date ranges)?  Do the numeric values have the statistical tendencies and ranges (min, median, max, etc.) you expect?  Are there any holes in the data (any missing values)?  Are you seeing anything that might give the type of math we're planning to use some problems?  And so on...  And just as critically important, what are you planning to do about any potential issues you're finding?

I can't tell you how many times I've been burned in a project because I didn't take my time exploring the data before jumping into trying to solve the problem.  It's always fun to dive right in as soon as we receive the data, but once you start seeing all of the problematic challenges lurking about that need your attention, it's very easy to get burned out and start looking for any excuse to move on.  Null values are not sexy.  Missing records are not exciting.  Duplicate observations are not fun.  But all of them are important to deal with, trust me.

```{tip}
The devil is in the details as they say, and you can't know what's hidding in plain sight waiting to bite you in the behind if you don't spend the time looking for it.
```

```{figure} ../images/wolf.png
---
width: 600px
name: wolf-fig
---
```

Exploratoy data analysis is a really broad and non standard topic.  Every dataset and problem is different so there's no way to create a one size fits all solution unfortunately.  But again, luckily there's a rough framework we can follow that should hopefully point us in the right direction and help us figure out what actions we need to take.

```{note}
**EDA**, or exploratory data analysis, generally will involve the following:

1. Investigating and understanding the charactersitics of our data (observations & features)
2. Uncovering any potential issues or anamolies that we need to address in some way
```

<br>

You'll come to understand that the separation between this exploratory work and the next topics of data wrangling and feature engineering is not as clear as you may hope for.  Sometimes you'll fix the issues straight away when you find them in the exploratory step, and other times you may choose to defer handling them until after you've reshaped your data in the wrangling step.  Merging multiple datasets together may need to wait until after you've brought one set up to a specific level of analysis, or alternatively maybe the unit of analysis requires that you perform this step before you lose the unique keys.  Creating new features may make sense to perform during an aggregation wrangling step, or possibly it needs to wait until after your data has been separated into training and validation sets.  The answer is always, _it depends..._

There's mostly no right or wrong way to do anything here; however, there is defnitely a loose and orderly way to think through all of these steps in a logical fashion, which is how we intend to present the material.  There are some general best practices on where to start and where to go next with each example we'll show, but of course your specific situation will vary from project to project.

Now back to EDA.  Let me caution you again from being too eager to move on from this stage too quickly.  There are serious penalties for not being diligent here.  Little issues may seem innocuous at the time, but I can assure you they will compound and confuse your models.  Your ability to solve the problem at hand will suffer due to anything less than a thorough examination of your data.

Good luck!