---
layout: post
title: Charting Skill and Chance in the NBA Draft
date: 2013/05/22 17:59 
categories: [numballs, pro]
---
We are big fans of NY Times'' data team. After reading [Charting Skill and Chance in the N.F.L. Draft](http://chartsnthings.tumblr.com/post/49236510636/charting-skill-and-chance-in-the-n-f-l-draft) we wondered if we could do something similar for the NBA draft. We wanted to see the position where best players are drafted each year.

So we did it. 
 
We collected data from [basketball-reference.com](http://www.basketball-reference.com/play-index/draft_finder.cgi?request=1&year_min=1992&year_max=2012&round_min=&round_max=&pick_overall_min=&pick_overall_max=&franch_id=&college_id=0&is_active=&is_hof=&c1stat=&c1comp=gt&c1val=&c2stat=&c2comp=gt&c2val=&c3stat=&c3comp=gt&c3val=&c4stat=&c4comp=gt&c4val=&order_by=ws&order_by_asc=&offset=1000#stats::none ). And then we used all players drafted on the NBA draft from 1992 to 2012 and [Win Shares](http://www.basketball-reference.com/about/ws.html) as a performance indicator.

As NYTimes crew did, we first started plotting players. As it was too noisy we simplified it calculating the mean for each draft position, and that''s the result. As the NBA has less picks than NFL we got a cleanest image. Colors show draft round.

![% Mean for every position](/img/201305_nbadfrat_meanpick.png)

After this first approach to the data, we wanted to see where the 5 most productive players. They are compared to others who were drafted in the same edition. Athletes like [Manu Ginobili](http://numballs.com/athlete/manu-ginobili) o [Marc Gasol](http://numballs.com/athlete/marc-gasol) were picked, but they started playing in the NBA some seasons later. 

Some interested stuff in this graph:

- Not so easy. 13/21 **#1 pick** are among five best players on each draft, 4/5 last five years.  
- It''s better to pick **third** than **second**. 06/21 **#2 pick** are on the top 5. 11/21 **#3 pick** are on the top 5.  
- Most of best players are picked on top 10.  

![% The 5 most productive players from each draft since 1992, and where they were selected](/img/201305_nbadraft_plot.png)

As bonus-track. We wanted to see when all the best NBA players were drafted. We draw a heatmap where blue intensity is the player performance (darkest blue = best performance). 

![% When the best NBA players were drafted](/img/201305_nbadraft_heatmap.png)

All these charts were made with R and Inkscape. Our goal is to get practice on data visualization, and learn imitating from the best.
