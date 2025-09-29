---
layout: post
title: North Atlantic Spring Phytoplankton Bloom
image: /assets/images/plankton-portrait.gif
tags:
  - portfolio
  - tutorial
  - qgis
  - adobe
  - animation
author: By Chiara Phillips
---
Mercator Ocean supports the E.U. Copernicus Marine Service in making ocean data freely available and accessible to the public. Although the Copernicus Marine Service offers a vast catalog of open datasets, its primary audience has historically been scientists. The team wanted to reach the data visualization community, showing that in addition to being scientific, ocean data can beautiful and creative.


# 02 Objective

My goal was to create an engaging, visually striking map that transformed Copernicus Marine Service data into something data visualization professionals would be excited to explore and learn about (and perhaps even re-create themselves).



# 03 Process – Using the AED Framework

Whenever I begin making a map, I follow what I call "the AED Framework". You may have heard of a device called "AEDs" before, which deliver a shock to someone's heart when their heart isn't beating effectively. In the same way, we can use "AED" in cartography to get our maps back on track and make them useful for the people that need them.



The framework is mainly designed around questions to ask yourself iteratively throughout your cartography process, starting with...


Audience!



When I think about my audience, questions I ask myself include:





Who is the audience for this map?



What background do they have?



What additional info might they need?



How will they be viewing it?



Why are they using this map?



What tone makes sense?



In this case, I knew my audience would be (geospatial) data visualization professionals, so they'd likely have backgrounds in QGIS or similar softwares. I assumed they would need more context on ocean science and export automation, and that I'd have to show my visualization in a slide format and on social media (Instagram). This led me to create two versions, one for each of the layout dimensions. My goal was to make the Spring Phytoplankton Bloom visually engaging, interesting, or inspiring to map.



The next part of the AED framework is E, for Ethics! Some of the questions in this stage include:





Do I understand the phenomenon that I am mapping?



Am I representing the data accurately and fairly?



Would other professionals approve of what I'm doing?



Is my work reproducible?


I don't come from an ocean science background, so I had to do a lot of research on phytoplankton blooms before I felt comfortable mapping it. 



I did research on:





What the definition of a bloom was (is it a certain concentration threshold that has to be met? A sudden spike of a certain magnitude? etc).



What causes phytoplankton blooms, and the North Atlantic Spring Bloom in particular? (Is it human-caused? Is it natural? Why do they happen? Is it bad? Good? Neutral?)



When does the North Atlantic Spring Bloom typically happen? When and where did it happen during my time period?



Typical ranges of phytoplankton with this phenomenon?



I also met with an ocean scientist at Mercator Ocean who studies this phenomenon.


<iframe title="2024 Chlorophyll-a concentration in the North Atlantic" aria-label="Line chart" id="datawrapper-chart-lzCHl" src="https://datawrapper.dwcdn.net/lzCHl/4/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="461" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r,i=0;r=e[i];i++)if(r.contentWindow===a.source){var d=a.data["datawrapper-height"][t]+"px";r.style.height=d}}})}();
</script>




This information helped me make better informed decisions on what region, time period, legend scale, legend colors, and tone to give my map piece. I learned that phytoplankton bloom definitions are still debated by scientists, but we can generally say that they are a rapid expansion in population, as highlighted in gray in the chart above. The North Atlantic Spring Bloom is largely a natural process that happens every year after nutrients from the deep sea stirred up to the surface from winter storms finally get the spring sunlight they need to photosynthesize, until they are eaten or run out of nutrients again. The ocean scientist let me know that the typical values of this bloom are between 0-2 mg per cubic meter of water, which aligned with the data I was seeing in the latitudes of the North Atlantic, where this phenomenon occurs.



The last letter in our AED framework, D, stands for Design. The two concepts I explore in the design stage are:





Does my map communicate clearly and intentionally with visual hierarchy in mind?



Is my map accessible?



The colors from my legend were sampled from pictures of Aurora borealis, since I thought satellite imagery I had seen of Plankton blooms really looked like the green northern lights, and inspired the same awe and wonder in me. This technique is one that I picked up from a webinar from Greg Fiske, of Woodwell Climate Research Center. I ran these color ramps through several accessibility checkers such as Coblis. 



The atmospheric effects I created in Adobe Illustrator were inspired by John Nelson, who had originally done these techniques in ArcGIS Pro. I thought these atmospheric effects draw the viewer deeper into the map and help put the focus on the globe and increase the contrast of the globe against the dark background.



I removed elements I thought distracted from the main message, and got feedback from both my new ocean scientist friend and general audiences and iteratively improved the design.



There is a whole world of accessibility that I still want to learn about from font sizes on screens to contrast, animation accessibility (avoiding flashes), internet speed accessibility, and supporting multi-language formats. If you have tips on these, do share!



# 04 Results





Slide layout shown in the webinar

The final animated map presented a daily view of phytoplankton bloom distribution between March and June 2024, revealing seasonal changes in a way that was both visually engaging and scientifically sound. It encouraged the data visualization community to explore Copernicus Marine Service datasets beyond purely scientific use cases, and they were kind enough to share that feedback back to me!


Awesome feedback!

# 06 Learnings

I find animated maps extremely engaging (and fun to make), but in webinar contexts, the lag between the sharer/viewer of videos can prevent the viewer from seeing all of the intended frames. This can make designs look less smooth. While animated maps can be nice for social media to draw in people's attention, for live webinars, static maps could make more sense. You can keep these learnings in mind for your next map!



# 07 Next Steps

Speaking of which, if you're interested in creating your own plankton map, you can check out the resources I created as part of this project:

Jupyter Notebook tutorials I created for exporting data from the Copernicus Marine Service

Youtube video tutorial covering QGIS and Illustrator styling, export automations, and Premiere animation

<iframe width="560" height="315" src="https://www.youtube.com/embed/A_0wvyBF3I0?si=rj2DAWOD4jHt7cJ9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


0:00 Intro

0:03 Globe Builder Plugin in QGIS

0:36 Graticule Symbology

1:04 Creating a QGIS Print Layout

1:13 Raster Symbology

3:33 Automating QGIS Print Layout Export

4:10 Setting up Adobe Illustrator Export Script

4:37 Creating Illustrator Layout

4:47 Illustrator Background Styling

5:22 Creating Globe Atmospheric Effects in Illustrator

6:14 Creating Title, Text Boxes & Legend

7:12 Automating Illustrator Layout Export

7:29 Animating in Adobe Premiere


If you do try this out for yourself (or run into any bugs along the way), let me know! I'm excited to see your plankton maps in the wild! ✨