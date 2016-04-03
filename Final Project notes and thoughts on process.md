# Final Project notes and thoughts on process

## ["Feeding America" Digitization Project](http://digital.lib.msu.edu/projects/cookbooks/)

To best explain the project I'll use a quote from their home page
> The Feeding America project has created an online collection of some of the most important and influential American cookbooks from the late 18th to early 20th century. The digital archive includes page images of 76 cookbooks from the MSU Library's collection as well as searchable full-text transcriptions. This site also features a glossary of cookery terms and multidimensional images of antique cooking implements from the collections of the MSU Museum.
The Feeding America online collection hopes to highlight an important part of America's cultural heritage for teachers, students, researchers investigating American social history, professional chefs, and lifelong learners of all ages.

The reason I chose to look at cookbooks is two fold.  First the material was accessable.  This is huge for me as I will often choose topics where information is either non existant or limited, and for a project where I wanted to use a lot of data I would need something accassable.  Second, we can learn a lot about our history from our cookbooks.  Food history is a powerful and important part of history and we can learn a lot about changes in technology and social sentements by plotting the topics in a hige collection of cookbooks.

## What I'm doing

What I'm doing with the data is topic modeling.  In an earlier blog post I disscussed Topic modeling and it seemed like a very interesting way to examine data that is to big to read all of.  Initially I was going to use novels from the Victorian era but I decided on cookbooks.   

## Process
### Here I will be writing about what I am doing with my project, as I am doingit.  Issues I encounter will be written down as they are happening as will solutions.  This way when the final results are compiled I can have an accurate account of how I got there.

So to start my analysis I had to download the collection. Then after some discussion with Prof. Graham we decided the best way to analize the data would be to rename the cookbooks' file names to be the date they were published.  This way I'd be able to create charts based on the year and examin historical trends that way.The first issue with this that I have encountered is that some cookbooks were published in the same year.  This means I've had to number them sequentially.  I'm still unsure of what issues this could create in my examination of the data. The second issue I have encountered is tediousness, the actual task of changing all the file names to dates is long and a bit frustrating as the dates are not always where you would expect them to be.  I have found that good music and a fun environment with lots of breaks is the best way to keep on track.

An interesting side note that I've noticed.  Some of the older cookbooks will include the number of years since American Independance with the copyright information

So I;m finding Excel to be pretty frustrating.  Particularily the graphs.  I can't seem to find one that presents my data well.

After discussing my project with a classmate on slack, I have decided to focus on the part that immigration plays in these cookbooks, and any possible cultural influences on American food history I can find.

Alright, so I'm starting to learn more in excel.  I found that if you do a graph of topics and the percentage they appear you can use that to see which topics are the most popular, then I can look at the dates they appear. That should be able to tell me something about the times when those topics were the most popular 

So on Friday I had a really helpful conversation with prof. Graham about my project.  We looked at the data together and decided that the reason one of the opics was as popular as it was, could be because i had not included a list of stop words.  So we went to [Ted Underwood's list of stop words](https://www.ideals.illinois.edu/handle/2142/45709) for topic modeling and re did my topic model of the cook books.  Then fiddled with excel so that the file names were dates again.  Then I explored the [Raw](http://raw.densitydesign.org/) app which creates a whole bunch of really interesting charts to visualize data.  This app has been incredibly useful as it has allowed me to use more data in my charts than I could with excel.  Now when I innitially ran my topc model topic 12 was overwhelmingly popular, which had both myself and prof. Graham questioning the data.  Now, with the exclusion of stop words and the addition of 5 extra topics, topic 24 seems the most popular.  But the percentages topics were appearing went down, this is good because it means I should be able to more acurately see whats happening.  Just to show you the difference here is the 25 topics topic model excluding the stop words ![25 topics, no stop words](file:///C:/Users/catha/Downloads/25%20topics,%20excluding%20stop%20wirds.svg) and here is the 20 topic topic model with the stop words still in there ![20 topics, with stop words](file:///C:/Users/catha/Downloads/20%20topics,%20includes%20stop%20words.svg) The type of chart I used there was a circle packing chart.  Here is Raw's decription of them 
> Nested circles allow to represent hierarchies and compare values. This visualization is particularly effective to show the proportion between elements through their areas and their position inside a hierarchical structure.
Based on http://bl.ocks.org/mbostock/4063530

Now that I see there is a big difference I'm going to look at the most popular topics from both runs of the topic modeling tool and see what they are and what can we learn from the different charts.