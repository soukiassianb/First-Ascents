# First-Ascents

Visualization of a dataset of the highest mountains in the world, part of the Data Analyst Nanodegree by Udacity.

Chart and accompanying story live here: [https://soukiassianb.github.io/First-Ascents/](https://soukiassianb.github.io/First-Ascents/)

## Summary
Visualization of a dataset of the highest mountains in the world, their first ascents and their "popularity" among climbers.
Chart built with D3 and dimple.js, using a [dataset](https://www.kaggle.com/abcsds/highest-mountains/) scraped from Wikipedia.
I wanted to give a historic perspective on the mountaineering achievements by focusing on the first ascents.
Among the main findings of this work, I discovered that:
- Most of the >7000 meters peaks were climbed between 1930 and 1996
- No peaks among the highest were climbed during WWII
- The highest peaks are also the most popular, the most popular of all being Mount Everest
- There is a significant popularity boost for peaks above the death zone limit

## Design
I choosed to plot the data using a bubble chart with years as the X axis and heights of the peaks as the Y axis. The size of the bubble showcase the sum of successful climbs and attempts before 2004, which gives a good idea of the popularity of the peaks.
The vertical axis of the chart is centered around 8000 meters, also called the death zone because of the lack of oxygen above it.

## Feedback

### Yoel
My friend Yoel gave me feedback regarding the range of the axis.
Plotting the heights of the peaks with a 0-based axis did not fully capture the variability of height between summits.
I then decided to plot the x axis between 7000 and 9000 meters, which put the 8000 meters mark (death zone limit) at the center of the chart.

### Mickael
My friend Mickael gave me similar remarks regarding the axis, and also told me that the lack of a legend made the color and bubble size encoding not clear.
I added a legend and a dashed line to show the death zone limit.

### Udacity Reviewer
The reviewer from Udacity gave me feedback about how the sizing method I used for bubbles was non-linear, potentially misrepresenting the scale of popularity between different peaks. I implemented his recommendation of square-rooting values used for the radius of the circles.

## Ressources
- http://dimplejs.org/
- https://d3js.org/
- http://wikipedia.com for information about climbers and peaks.
