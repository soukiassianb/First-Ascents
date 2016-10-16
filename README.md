# First-Ascents

Visualization of a dataset of the highest mountains in the world, part of the Data Analyst Nanodegree by Udacity.

Chart and accompanying story live here: [https://soukiassianb.github.io/First-Ascents/](https://soukiassianb.github.io/First-Ascents/)

## Summary
Visualization of a dataset of the highest mountains in the world, their first ascents and their "popularity" among climbers.
Chart built with D3 and dimple.js, using a [dataset](https://www.kaggle.com/abcsds/highest-mountains/) scraped from Wikipedia.
I wanted to give a historic perspective on the mountaineering achievements by focusing on the first ascents.

## Design
I choosed to plot the data using a bubble chart with years as the X axis and heights of the peaks as the Y axis. The size of the bubble showcase the sum of successful climbs and attempts before 2004, which gives a good idea of the popularity of the peaks.
The vertical axis of the chart is centered around 8000 meters, also called the death zone because of the lack of oxygen above it.

## Feedback
While showing the first draft of the chart, I got feedback regarding the range of the axis. Plotting the heights of the peaks with a 0-based axis did not fully capture the variability of height between summits, I then got the idea of plotting around the death zone limit which conveniently did not remove any data points.

## Ressources
- http://dimplejs.org/
- https://d3js.org/
- http://wikipedia.com for information about climbers and peaks.
