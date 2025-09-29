---
layout: post
title: Germany's Population Change
image: /assets/images/germany-population-change.png
tags:
  - portfolio
  - qgis
  - canva
  - human-geography
author: Chiara Phillips
published: false
---

I created this map in the 2023 #30daymapchallenge for the themes "minimal," "black and white," and "population".

I've gotten so many questions on how I created it! The short of it is that the data is natively in raster format, but it's presented in vector format. How?!

Well, I created a population change raster by subtracting values from 2020 to 2010 with raster calculator in QGIS. I then created an equal area vector grid of Germany and used that grid to calculate the average population change using zonal statistics. Then, I created a centroid layer from my zonal statistics vector output, which I then visualized proportional by size in QGIS: one for population growth and one for population decline. My last step was beautifying with a legend and title in Canva. :)

## Tools Used
QGIS, Canva

## Data Source
WorldPop
