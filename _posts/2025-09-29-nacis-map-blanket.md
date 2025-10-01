---
layout: post
title: NACIS Map Tile
image: /assets/ai2html/nacis-map-blanket/MapQuilt_Phillips_editable_text-Artboard_1.jpg
tags:
  - portfolio
  - tutorial
  - qgis
  - adobe
author: By Chiara Phillips
published: true
---

This year, I decided to participate in the NACIS Map Blanket project!
My tile was (North, west, east, south: 45.0, -125.0, -65.0, 25.0).

At first glance, I wasn't sure what to map. I looked at what points of interest were 
within my tile. I noticed that the Louisville Airport was within my tile. I looked
at the airport's news on their website, and saw that they had a huge number of 
people flying out after the Kentucky Derby. I found out that this is consistently
the busiest day of the year for the airport. So, I set out to map the number of flights
out of the Louisville Airport after the Kentucky Derby.

I used the Flight Radar API to get the number of flights out of the Louisville 
Airport after the Kentucky Derby.

Then I used QGIS to map the number of flights out of the Louisville Airport 
after the Kentucky Derby.

I added labels and symbols to the map within Adobe Illustrator and exported the map
using AI2HTML to embed in this post.

<div class="not-prose w-full my-8">
  <iframe
    src="{{ '/assets/ai2html/nacis-map-blanket/MapQuilt_Phillips_editable_text.html' | relative_url }}"
    style="width:100%; border:0; aspect-ratio: 16 / 9;"
    loading="lazy"
  ></iframe>
</div>

### Tools Used
QGIS, Adobe Illustrator, AI2HTML

### Data Source
Flight Radar
