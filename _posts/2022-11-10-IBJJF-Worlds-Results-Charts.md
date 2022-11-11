---
layout: posts
title: "IBJJF Worlds Team Results by Year"
---
## Making interactive charts with data from a website
### My first self-directed project to practice data scraping and data visualization skills

![Screenshot of Men's team results](/assets/images/IBJJF_Worlds_Mens_Results.jpg)

Have you ever wanted to see how some of the big Brazilian jiu jitsu teams have ranked at the World Championships every year? Yeah, me neither but I thought it'd be a cool project to practice and learn some new skills. Joking aside, I was genuinely curious if there was a trend of certain teams consistently ranking highly through the years. If you practice BJJ, you probably hear about some competitors and teams winning all the time but how often do we look at their rankings over the years? Even if you're not participating in or following this very niche sport, it might give you some ideas or tools to do a similar analysis on another subject.

I recently completed a module in a Python course I'm taking that covered web scraping. Previously, I had already been doing a bit of data visualization in Python for work, so I wanted to try to put these two together into a bigger project. This has recently snowballed into a larger project to include learning how to create a website on Github Pages since I want to share the results and interactive charts. I also wanted to make it accessible to those who aren't so familiar with Github or other sites where people share code.

How I did it: To get the data, I did some web scraping from the IBJJF's Championships results page to get the individual year rankings. After cleaning up the data in pandas, I used Altair to plot the results for Men's, Women's, and Juvenile categories.

<b>This site is best viewed on a desktop. To select multiple teams in the chart, click a team then hold Shift + Left-click your mouse to add more teams.</b>

