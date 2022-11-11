---
layout: posts
title: "IBJJF Worlds Team Results by Year"
htmlwidgets: TRUE
classes: wide
---
## Making interactive charts with data from a website

![Screenshot of Men's team results](/assets/images/IBJJF_Mens_Results.jpg)

If you practice BJJ, you probably notice some teams win consistently but how often do we look at their rankings over the years? Even if you're not participating in or following this very niche sport, it might give you some ideas or tools to do a similar analysis on another subject.

How I did it: To get the data, I did some web scraping from the IBJJF's Championships results page to get the individual year rankings. After cleaning up the data in pandas, I used Altair to plot the results for Men's, Women's, and Juvenile categories.

<b>This site is best viewed on a desktop.
To select multiple teams in the chart, click a team's name in the legend, then hold `Shift + Left-mouse-button` to add more teams.</b>

{% include chartmenresults.html %}