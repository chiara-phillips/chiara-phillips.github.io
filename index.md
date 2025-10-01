---
layout: home
---
<div id="about" style="display: flex; align-items: center; gap: 2rem; margin-bottom: 2rem; width: 100%; max-width: none; flex-wrap: nowrap;">
  <img src="/assets/images/2024-chiara-portrait.png" 
       alt="Chiara portrait" 
       style="max-width: 300px; width: 300px; height: 300px; object-fit: cover; border-radius: 50%; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); flex-shrink: 0;" />
  
  <div style="flex: 1; min-width: 300px; text-align: left; max-width: none;">
    <p style="font-size: 1.1rem; line-height: 1.6; margin-bottom: 1rem; color: #374151; text-align: center;">
      Geographer and designer specializing in cartographic storytelling and programming.
    </p>
    
                         <p style="font-size: 1.1rem; margin-bottom: 0.5rem; color: black; text-align: center;">
                 <a href="mailto:chiara.m.phillips@gmail.com" style="color: black; text-decoration: none; cursor: pointer; font-weight: 900;">Let's work together!</a>
               </p>
  </div>
</div>

<div id="portfolio" class="md:w-4/5 mx-auto mb-10">
  {% assign portfolio_posts = site.posts | where: "tags", "portfolio" %}
  {% for post in portfolio_posts %}
    {% assign is_even = forloop.index | modulo: 2 %}
    <div class="flex flex-col md:flex-row items-center gap-8 mb-16 {% if is_even == 0 %}md:flex-row-reverse{% endif %}">
      <div class="md:w-2/3">
        <a href="{{ post.url | relative_url }}" class="block hover:opacity-90 transition-opacity duration-300">
          <img src="{{ post.image | relative_url }}" 
               alt="{{ post.title }}" 
               class="w-full h-auto shadow-lg rounded-lg">
        </a>
      </div>
      <div class="md:w-1/3 text-center md:text-left">
        <a href="{{ post.url | relative_url }}" class="hover:text-gray-800 transition-colors duration-300">
          <h3 class="text-2xl md:text-3xl font-semibold mb-4">{{ post.title }}</h3>
        </a>
        <p class="text-gray-600 text-lg">{{ post.excerpt | default: post.content | strip_html | truncate: 150 }}</p>
      </div>
    </div>
  {% endfor %}
</div>