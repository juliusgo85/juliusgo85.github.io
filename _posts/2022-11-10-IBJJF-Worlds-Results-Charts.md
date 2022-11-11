---
layout: posts
title: "IBJJF Worlds Team Results by Year"
htmlwidgets: TRUE
classes: wide
---
## Web scraping and interactive bump charts

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

Some of the powerhouse men's teams over the years are Alliance, Atos, CheckMat, Cicero Costha, GF Team, and Gracie Barra. Some newer teams on the rise: Art of Jiu Jitsu, Dream Art, Unity.

{% include chartwomenresults.html %}
Interestingly, compared to the men's team results, there are more unconnected dots, indicating top teams from one year don't necessarily place in the following year. This seems more prevalent in the earlier years.

Notable exceptions for the women's teams: Alliance, Atos, CheckMat, GF Team, Gracie Barra, Gracie Humaita. Some newer teams on the rise: Dream Art, Infight, Unity.

{% include chartjuvenileresults.html %}

Juvenile teams over the years: Alliance, Atos, Brasa CTA, CheckMat, Cicero Costha, GF Team, Gracie Barra, Gracie Humaita, Nova Uniao (they had a lot of success in the first few years). Too many up and coming teams to name off.

For the most part, I tried to consolidate team names for wording or spelling variations. However, I left in nearly identical team names if they both placed within a category for the same year (such as Alliance and Alliance International, or Gracie Humaita and Gracie Humaita Reunion).

 A lot of the same teams show up in the 3 separate categories. These are generally some of the largest schools/associations out there. Certainly, a big factor of the overall points is the number of competitors each team places in each weight class at each belt. The other big factor is how well each of those competitors do, but I don't think there's a complete listing available showing each competitor's win/loss record during each tournament.
 
 "If you're not first, you're last."