---
layout: posts
title: "IBJJF Worlds Team Results by Year"
htmlwidgets: TRUE
classes: wide
header:
  teaser: /assets/images/IBJJF_Mens_Results.jpg
---
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:site" content="@wearejackie">
<meta name="twitter:creator" content="@wearejackie">
<meta name="twitter:title" content="IBJJF Worlds Results by Year">
<meta name="twitter:description" content="Interactive bump charts showing IBJJF team rankings by year">
<meta name="twitter:image" content="https://juliusgo85.github.io/assets/images/IBJJF_Mens_Results.jpg">

## Web scraping and interactive bump charts

<figure>
  <img
    src="/assets/images/IBJJF_Mens_Results.jpg"
     alt="Static image of Men's results">
  <figcaption>Static screenshot, interactive charts shown below.</figcaption>
</figure>

**This site is best viewed on a computer. Viewing on your phone won't allow selecting multiple teams in the charts.**

If you practice Brazilian jiu jitsu (BJJ), you probably notice some teams win consistently but how often do we look at their rankings over the years? Even if you're not participating in or following this very niche sport, it might give you some ideas or tools to do a similar analysis on another subject.

Let's dive in and take a look at how teams have performed at the International Brazilian Jiu Jitsu Federation's (IBJJF) World Championship tournament over the years.

Which teams are "streaky" and place in the top consistently year over year? Are there any "one hit wonder" teams? One thing to keep in mind is the team results are based on athlete rankings within the various belts, not just at the black belt level.

Team rankings are provided for adult males adult female, and juvenile groups.

Team rankings are based on how a team's athletes place in their respective brackets (divided by age group, gender, belt, weight class) in a single elimination tournament. First place gets 9 points, second place gets 3 points, third place gets 1 point. There are two 3rd-place finishers (they're the ones who lost to 1st and 2nd place winners before the finals match, but don't compete aganist each other after being eliminated).

A fair criticism is that the points are the same for each belt level - i.e. 1st place for a blue belt is the same number of points for 1st place for a black belt. So these rankings are best read as an indication of a team's ability to field winning athletes for as many divisions as possible, instead of a measurement of a team's rankings at a given belt.

**How I did it:** To get the data, I did some web scraping from the IBJJF's Championships results page to get the individual year rankings. After cleaning up the data in pandas, I used Altair to plot the results for Men's, Women's, and Juvenile categories.

## Quick notes for navigating:
- **To select multiple teams in the chart, click a team's name in the legend, then `Shift + Click` to add more teams.**
- You can also hover over each point to identify the team plotted.

<br/>

{% include chartmenresults.html %}
The IBJJF only recorded team rankings for the top 3 teams until 2011, then they started showing the top 10.

Some of the powerhouse men's teams over the years: Alliance, Atos, CheckMat, Cicero Costha, GF Team, and Gracie Barra. Some newer teams on the rise: Art of Jiu Jitsu, Dream Art, Unity.

{% include chartwomenresults.html %}
Interestingly, compared to the men's team results, there are more unconnected dots, indicating top teams from one year don't necessarily place in the following year. This seems more prevalent in the earlier years.

Consistently high-performing women's teams: Alliance, Atos, CheckMat, GF Team, Gracie Barra, Gracie Humaita. Some newer teams on the rise: Dream Art, Infight, Unity.

{% include chartjuvenileresults.html %}

Consistent top juvenile teams over the years: Alliance, CheckMat, GF Team, Gracie Barra, Gracie Humaita, Nova Uniao (they had a lot of success in the first few years then placed sporadically). More recent years show Art of Jiu Jitsu, Atos, and Team Lloyd Irvin establishing themselves among the top teams.

For the most part, I tried to consolidate team names for wording or spelling variations. However, I left in nearly identical team names if they both placed within a category for the same year (such as Alliance and Alliance International, or Gracie Humaita and Gracie Humaita Reunion).

 A lot of the same teams show up in the 3 separate categories. These are generally some of the largest schools/associations out there. Certainly, a big factor of the overall points is the number of competitors each team places in each weight class at each belt. The other major factor is how well each of those competitors do, but I don't think there's a complete listing available showing each competitor's win/loss record during each tournament.
 
 Remember: "If you're not first, you're last." To end with some cynicism and some levity, no one will remember if you won or lost if you're not on the podium. If you lost horribly in the first round, the record books won't remember but your opponent's highlight reel might! Joking aside, tournaments are supposed to be a challenge to yourself but should ultimately be fun so just go out there and play your game.

 Thanks for reading through this. I hope this was insightful and easy to digest.

 For those interested in seeing how the sausage is made, please check out the <a href="https://juliusgo85.github.io/IBJJF_Worlds_results_notebook.html">Jupyter notebook</a>. Github Pages does not natively render the Altair interactive charts in Jupyter notebooks, so I'm sharing the notebook as an html file.