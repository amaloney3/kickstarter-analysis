# Kickstarting With Excel: An Analysis of Crowdfunding in the Arts

## Overview of Project
This project involves the organization and analysis of eight years (2009-2017) of data from the crowdfunding 
service Kickstarter, which features campaigns for music and entertainment, and food, games and technology, among others.

### Purpose
The purpose of this project was to gain insight about crowdfunded projects in the arts and help the client better
understand which endeavors tend to get support. Specifically, I sought to answer how launch dates and initial funding goals
on Kickstarter affect whether theatrical plays are ultimately subsidized. 

## Analysis and Challenges
The analysis involved sorting and extracting the most relevant data for the client -- data on campaigns for theatrical 
productions, when they were launched and whether or not they were successful. It also required filtering 
data based on funding totals and converting outcomes into percentages. Among other challenges, 
using Excel commands such as 

```
=COUNTIFS(Kickstarter!F:F,"Successful",Kickstarter!$D:$D,"<1000",Kickstarter!R:R,"plays")
```

to stratify the appropriate categories across worksheets took several troubleshooting maneuvers and multiple iterations
of fact-checking. One fact-check, for instance, involved using both 


```
=SUM
```

and

```
=COUNTIFS
```
to verify the total number of successful and failed projects aligned between methods (see below):

![image](https://user-images.githubusercontent.com/1015285/116834299-018cc400-ab83-11eb-8b46-7660f5e0fcd9.png)

Although not difficult, per se, creating intuitive color schemes on the finished graphs also required extra thought and attention to detail.


### Analysis of Outcomes Based on Launch Date

The graph below depicts the number of successful, failed and canceled campaigns related to theatrical productions, based on the months they were launched. Although further analysis would be helpful, it's fair to say the data here suggest:

1. Theatrical campaigns are relatively successful overall, with the number of failures never quite matching the number of successes.
2. The spring and summer -- particularly May and June -- appear to be optimal months for successful theatrical campaigns

![image](https://user-images.githubusercontent.com/1015285/116834644-a6f46780-ab84-11eb-8ead-8c271991f2d7.png)

Again, more data analysis would be required to tease out those relationships and draw further conclusions about causality.

### Analysis of Outcomes Based on Goals

Because the client was interested specifically in plays, it was useful to do further analysis on how those particular projects fared. Accordingly, I stratified the success of crowdfunding campaigns for plays based on their funding targets -- from projects that sought less than $1,000 to those that sought more than $50,000. The relationship isn't perfect, but I think it's fair to conclude that more modest funding targets tend to have more success in this particular domain. Projects in the $35,000 to $40,000 appear to be an interesting exception to that rule-of-thumb. But again, more analyses is required.

![image](https://user-images.githubusercontent.com/1015285/116834806-5af5f280-ab85-11eb-8fb3-6f3c895c8059.png)

### Limitations, Conclusions And Further Areas For Study
The Kickstarter data analyzed here is only current through 2017, so it's unclear whether trends observed over the last four years converge or diverge with the rest of the set.  Additionally, more granular data would be required to explain exactly why there seems to be a correlation between the middle months of the year and successful theatrical crowdfunding efforts, or why exactly certain campaigns end up canceled. Additionally, while Kickstarter is arguably one of, if not, the biggest name in crowdfunding, it's certainly not the only one. Perhaps data culled from other services (e.g. GoFundMe or Patreon) would paint different pictures.

Besides the analyses completed here, it could be helpful to stratify successes and failures based on country of origin. Such an analysis could show us whether there are signficiant differences in support for plays/theater across artistic cultures. Pie charts depicting the percentage of crowdfunding goals achieved could also help give us a more granular sense of success and failure. 

Ultimately, this analysis suggests a modest funding target for plays. One that can preferably launch in the middle of the year, too, would seem to have a reasonable chance of success. Further study could ultimately help the client make a more informed decision.
