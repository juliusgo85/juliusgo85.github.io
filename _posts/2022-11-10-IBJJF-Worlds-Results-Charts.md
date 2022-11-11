---
layout: posts
title: "IBJJF Worlds Team Results by Year"
htmlwidgets: TRUE
classes: wide
---
## Making interactive charts with data from a website

![Screenshot of Men's team results](/assets/images/IBJJF_Mens_Results.jpg)

If you practice Brazilian jiu jitsu (BJJ), you probably notice some teams win consistently but how often do we look at their rankings over the years? Even if you're not participating in or following this very niche sport, it might give you some ideas or tools to do a similar analysis on another subject.

Which teams are "streaky" and place in the top consistently year over year? Are there any "one hit wonder" teams who only did well once so far? One thing to keep in mind is the team results are based on athlete rankings within the various belts, not just at the black belt level.

**How I did it:** To get the data, I did some web scraping from the IBJJF's Championships results page to get the individual year rankings. After cleaning up the data in pandas, I used Altair to plot the results for Men's, Women's, and Juvenile categories.

## Quick notes for navigating:
- **This site is best viewed on a desktop.**
- **To select multiple teams in the chart, click a team's name in the legend, then hold `Shift + Left-mouse-button` to add more teams.**
- You can also hover over each point to identify the team plotted.


{% include chartmenresults.html %}
The IBJJF only recorded team rankings for the top 3 teams until 2011, then they started showing the top 10.

{% include chartwomenresults.html %}
Interestingly, compared to the men's team results, there are more unconnected dots, indicating top teams from one year don't necessarily place in the following year. This seems more prevalent in the earlier years.

{% include chartjuvenileresults.html %}