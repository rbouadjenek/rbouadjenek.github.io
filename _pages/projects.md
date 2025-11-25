---
layout: page
title: research
permalink: /research/
description: 
nav: true
nav_order: 2
---

## Research Overview: From Data to Decision-making for Better Services
### Introduction

With the emergence of the social Web in the mid-2000s, the Web has evolved from a static Web, where users were only able to consume information, to a Web where users are also able to interact and produce information. This
evolution which is commonly known as Social Web or Web 2.0, has introduced new freedoms for the user in his
relation with the Web by facilitating his interactions with other users who have similar tastes or share similar
resources. Examples of Web 2.0 include social platforms and networks (such as MySpace, Facebook, and
LinkedIn), collaborative tagging sites (like delicious, CiteULike, and Flickr), microblogging sites (like Twitter and
Yammer), and even crowdsourced databases (e.g., Bioinformatics sequence databases such as GenBank or
UniProt).
These platforms are commonly used as means to communicate with other users, exchange messages, share
resources (photos, videos, or bioinformatics sequences), comment, tag, maintain profiles, interact and
play online games, etc. In addition to dedicated social platforms, traditional content providers like
newspapers, tend to be more social since they provide to users means for sharing, commenting, and linking
documents together, e.g., sharing. These collaborative tasks are among the most important factors
for the increasingly quantity of available social data. Hence, the need to exploit this unprecedented
quantity of data is critical for many companies and their business. This has led to the development of
Data-driven Decision-making techniques to extract valuable knowledge from this data, based on
fast, effective and scalable data analysis and machine learning algorithms, which are at the heart of
my research interests focusing on descriptive, predictive, and prescriptive analytics of large-scale
data.
Specifically, my research addresses data and information quality in crowdsourced databases, as well as the crucial
problem of enabling users to consume relevant information with respect to their interests and needs. This
task is commonly realized through content recommendation (such as movie Netflix, books on Kobo
or products on Amazon) or Information Retrieval ( on platforms like Google or Bing). However,
conventional models of recommendation and Information Retrieval don&#8217;t consider this side social
information, and proposing novel extensions are also at the heart of my work. As two exemplars of my
research:
                                                                                                
                                                                                                
<ul>
<li>In Social Information Retrieval <span>[<a 
href="papers/IS-D-14-351.pdf">1</a>]</span>, I have extended conventional Information Retrieval models in
order to incorporate side social information. Specifically, I have introduced a novel ranking function
<span >[<a href="papers/sp086-bouadjenek.pdf">2</a>]</span>, a new Information Retrieval modeling schema <span class="cite">[<a 
href="papers/sp085-bouadjenek.pdf">3</a>,&#x00A0;<a 
href="papers/INS-D-15-2480.pdf">4</a>]</span>, and a query expansion algorithm <span>[<a href="papers/p1113-bouadjenek.pdf">5</a>,&#x00A0;<a 
href="papers/TLDKS-12008.pdf">6</a>]</span> all
based on innovative social features. These contributions have been integrated into a social web search
engine called LAICOS <span>[<a 
href="papers/demo16-bouadjenek.pdf">7</a>]</span>, which represented some of my major contributions to the area of Social
Information Retrieval.
</li>
<li>In data quality for collaborative bioinformatics databases (e.g., <span class="cite">[<a 
href="papers/bax021.pdf">8</a>,&#x00A0;<a 
href="papers/JBI-17-134.pdf">9</a>,&#x00A0;<a 
href="papers/sp0228-bouadjenek.pdf">10</a>,&#x00A0;<a 
href="papers/BINF-D-18-00977.pdf">11</a>]</span>), I have addressed the
problem of identifying low-quality and suspicious records based on literature analysis. These databases
contain  hundreds  of  millions  of  records  derived  from  submissions  by  individual  laboratories,  as
well as from bulk submissions from large-scale sequencing centers. Their diversity and scale means
that they suffer from a range of data quality issues including errors, discrepancies, redundancies,
ambiguities, and incompleteness. In that context, I have combined a set of information retrieval and
machine learning techniques while using the published literature as a background knowledge to detect
literature-inconsistent records.</li>
</ul>

With the increasing level of business competitiveness, investigating more intelligent and faster ways of analyzing,
exploring, using, and mining the data is a key aspect for many businesses. Hence, my objective is to go deep in the
development and the usage of data analytics in different areas from both academic and industry perspectives. To
elaborate in more detail, following is a summary of my ongoing research that enables this large-scale data processing for information retrieval and recommendation.


### Mining Massive Media
Social media sites such as Twitter present a double-edged sword for users. On one hand these sources
contain a vast amount of novel and topical content that challenge traditional news media sources
in terms of their timeliness and diversity. Yet on the other hand they also contain a vast amount
of chatter and otherwise low-value content for most users&#8217; information needs where filtering out
irrelevant content is extremely time-consuming. My previous work on twitter topic classification <span class="cite">[<a 
href="papers/ICWSM2017.pdf">12</a>]</span>
has noted this need for topic-based filtering and has adopted a range of variations on supervised
classification techniques to build effective topic filters. However, there remain many fundamental
research questions that need to be answered on a longitudinal study of the performance of such
supervised topic classifiers. For example, can we identify temporally unstable features? How can we
design a learning algorithm that automatically downweights the influence of temporally unstable
features?

### Visualizing large-scale Data for Information Retrieval
In many applications that involve searching geo-temporal data, results are often displayed on a map or other
interactive visual interfaces. However, in many settings of interactive visual search, it is time-consuming to
individually examine all matching results. This suggests the need to aggregate results, for example, via an
                                                                                                
                                                                                                
unsupervised clustering method like K-means. These ideas build on the <span 
class="cmti-10x-x-109">&#8220;cluster hypothesis&#8221; </span>of information
retrieval, which posits that documents in the same cluster are likely to address similar relevance needs for the
search task. Unfortunately, the use of unsupervised methods does not necessarily guarantee that the
clusters themselves are relevant. Therefore, it is critical to develop relevance-driven clustering methods
for Visual Information Displays (VIDs) that are capable of displaying highly relevant clusters for
queries.
Since &#8220;retrieved&#8221; information elements are not individually selected, but rather clustered using the relevance
signal of each element, the problem is clearly an optimization problem of how to restrict cluster settings to show
the user the most relevant information to his query. While this notably diverges from the standard information
retrieval setting where ranked documents are chosen individually, these additional constraints do not change the
overall objective to select relevant information given the user&#8217;s information need as represented by
the given relevance measure. In this work, I intend to provide a unified framework that abstracts
presentation-specific details of different information clusters for VIDs and facilitates an optimization perspective
of clustering w.r.t. a provided relevance measure. I also intend to define a new specific objective
function for optimization that is suitable for this visualization task. Finally, I aim to propose new, fast,
effective and scalable algorithms that optimize the objective function that I define for this visualization
task.

### Machine Learning and Social Media Analysis for Financial Analytics
Social media platforms such as Twitter or StockTwits are widely used for sharing advice between investors,
traders, and entrepreneurs. The popularity of these platforms, the vast amount of information generated by active
members, and their usage by influential people imply that this social media content is often predictive of financial
markets.
In this project, I plan to develop novel algorithms to model the influence of social media on stock
market performance. These novel methods are based on machine learning principles that will provide
financial analysts with powerful tools for summarizing social media sentiment and opinion regarding
individual stocks as well as providing quantitative predictions for use in investment and trading
decisions.
Specifically, the research questions I intend to answer in this project are: how can we model and capture the
influence of users, brand and industry mentions over time? How can we deal with varying reliability of users for
different stocks, or users with non-stationary (i.e., fluctuating) influence over time? How can we automatically
identify brands that may be relevant to a stock ticker to reduce the number of features in our prediction models
and improve the quality of fit (i.e., it is easier to learn accurate parameters in smaller models since it is harder to
overfit in these cases)?

### Future Research Directions 
While my work has made contributions to large-scale data processing and retrieval, there still remains a vast
amount of research to improve data processing, retrieval and recommendation technologies in an online
                                                                                                
                                                                                                
framework. To this end, following are a few key areas where my future research will help close the loop between
data and decisions:

<ol  class="enumerate1" >
<li class="enumerate" id="x1-5002x1"><b>Combining diverse side information for recommendation and IR: </b>users are interacting on
diverse online services such as social network platforms, collaborative tagging sites, microblogging
sites,  and  online  game  platforms.  These  services  provide  valuable  information  to  enhance
recommendation  and  IR.  A  critical  question  is  how  to  extend  existing  solutions  into  a  unified
framework that considers multiple and diverse data sources? I have attempted to answer this question
for recommendation using a co-matrix factorization approach of multiple data sources <span class="cite">[<a 
href="papers/DBKDA2018_v2.0.pdf">13</a>]</span>.
</li>
<li class="enumerate" id="x1-5004x2"><b>Real-time analysis of large-scale data: </b>considering stream data analysis is important for most
existing data mining techniques. But how to do it? Although it&#8217;s a significant challenge in data
mining, different options are possible. One direction consists of exploring the possibility of updating
models without their complete re-computation (incremental learning).
</li>
<li class="enumerate" id="x1-5006x3"> <b>Large-scale data visualization: </b> many applications such as real-time monitoring of social network
activities or urban traffic congestion reports involve high information and cognitive load tasks. In this
context, it is common to have large-scale information visualization interfaces to concurrently display
system status, alerts, and events. However, displaying all information elements simultaneously would
result in a saturated and unreadable display. Thus, the development of novel adaptive user interfaces
(AUIs) are required to help focus the user&#8217;s attention by filtering information relevant to their current
task. How to optimally set the parameters of filters is a problem that I intend to formalize as a
Mixed-integer Linear Programming for which we have optimal solvers.</li></ol>

Overall, my vision for the future is simple: social media is connecting everything, Web services are becoming more
interactive and personalized, and every embedded system that impacts our lives &#8212; from our daily commute to our
consumer needs &#8212; will become increasingly adaptive. This means that we will have to transform immense
quantities of data into valuable knowledge that should be used for decision-making. This is what I aim to do in my
research.  
