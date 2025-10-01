---
layout: post
title: FlightRadar24, Illustrator, & My 2025 NACIS Map Quilt Tile
image: /assets/images/KentuckyDerbyFlights_NACIS2025_Print.png
tags:
  - portfolio
  - tutorial
  - qgis
  - adobe
author: By Chiara Phillips
published: true
---
<style>
/* Heading 1 styling */
.prose h1 {
  text-align: center !important;
  font-size: 2rem !important;
  padding-top: 2rem !important;
  margin-bottom: 1.5rem !important;
}

/* Heading 2 styling */
.prose h2 {
  text-align: center !important;
  font-size: 1.5rem !important;
  padding-top: 1.5rem !important;
  margin-bottom: 1.5rem !important;
}
</style>
This year, I contributed a tile to the NACIS Map Quilt for the conference in Louisville, KY!

At first, I wasn't sure what I wanted to map. I didn't know much about the city
and upon looking at OpenStreetMap data, my tile seemed largely residential. I tried making a map that just had some colors I liked. 

It didn't feel satisfying to me though— I knew that this place must have a story to tell, I just didn't know it well enough yet.

In exploring the map with the colors I liked, I noticed an area in the top right that was different from the rest of my tile. It was the Louisville Airport! 

<br>
<div style="display: flex; justify-content: center;">
<img src="/assets/images/mapquilt_first_attempt.png" alt="First draft" style="width: 50%; max-width: 400px;">
</div>
<div style="text-align: center; margin-top: 1rem; margin-bottom: 2rem;"><i>Initial research and color play</i></div>

I decided to check out their website and came across a "News" section. There, I found that every year, the busiest day at the airport is 
typically the Sunday after the Kentucky Derby ([article here](https://www.flylouisville.com/louisville-muhammad-ali-international-airport-is-ready-for-kentucky-derby-151/){: style="color: #0066cc; text-decoration: underline;"}). I was fascinated, and set out to figure out where all of those planes were going.

Using [Flight Summary Light](https://fr24api.flightradar24.com/docs/endpoints/flight-summary){: style="color: #0066cc; text-decoration: underline;"} within the FlightRadar24 API, I retrieved all flights out of the Louisville 
Airport after the Kentucky Derby on May 4th, 2025. Then, I removed any flights that were not passenger planes or private jets.

From there, I summarized how many planes were going to each state and used a Streamlit app I created called [Click2Vector](https://www.chiaraphillips.com/#click2vector){: style="color: #0066cc; text-decoration: underline;"} to export a point GeoJSON that contained each state in my dataset.

Then I used "Hub lines" in QGIS to create paths from Louisville to all of the states map the number of flights out of the Louisville Airport 
after the Kentucky Derby. For styling, I intentionally decided to use the [branding](https://www.kentuckyderby.com/)style="color: #0066cc; text-decoration: underline;"" of the Kentucky Derby, both in color and font to give it some visual cohesion. If you look closely, you may see some little easter eggs as well.

After that, I added labels, text, and symbols to the map within Adobe Illustrator.


<br>
<div style="display: flex; justify-content: center;">
<img src="/assets/images/KentuckyDerbyFlights_NACIS2025_Print.png" alt="First draft" style="width: 90%; max-width: 800px;">
</div>
<div style="text-align: center; margin-top: 1rem; margin-bottom: 2rem;"><i>Final draft</i></div>

I'm looking forward to seeing the full Map Quilt!