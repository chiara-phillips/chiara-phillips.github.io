---
layout: home
---
<div id="about" style="display: flex; align-items: center; gap: 2rem; margin-bottom: 2rem; width: 100%; max-width: none; flex-wrap: nowrap;">
  <img src="/assets/images/2024-chiara-portrait.png" 
       alt="Chiara portrait" 
       style="max-width: 300px; width: 300px; height: 300px; object-fit: cover; border-radius: 50%; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); flex-shrink: 0;" />
  
  <div style="flex: 1; min-width: 300px; text-align: left; max-width: none;">
    <p style="font-size: 1.1rem; line-height: 1.6; margin-bottom: 1rem; color: #374151; text-align: center;">
      Over the past 6+ years as a Cartographer and Geospatial Software Developer, I have helped countless organizations understand and communicate the hidden stories within spatial data.
    </p>
    
          <p style="font-size: 1.1rem; margin-bottom: 0.5rem; color: #f75f61; text-align: center;">
        Ready to bring your data to life?
      </p>
      <p style="font-size: 1.1rem; font-weight: 600; margin-bottom: 0.5rem; color: #f75f61; text-align: center;">
        <a href="#contact" style="color: #f75f61; text-decoration: none; cursor: pointer;" onclick="document.getElementById('contact').scrollIntoView({behavior: 'smooth'}); return false;">Let's work together!</a>
      </p>
  </div>
</div>

<div id="portfolio" class="md:w-4/5 mx-auto gap-4 md:gap-6 columns-2 md:columns-3 mb-10">
  {% for post in site.posts %}
    {% if post.tags contains 'portfolio' %}
    <div class="md:fadeIn pb-8 mb-8 break-inside-avoid-column ">
      <div class="hover:underline hover:decoration-2 hover:underline-offset-4 transition ease-in-out delay-150 hover:-translate-y-1 hover:scale-104 duration-300">
        <a href="{{ post.url | relative_url }}">
          <img src="{{ post.image | relative_url }}" alt="" class="w-full max-w-screen-sm h-auto shadow-md rounded-lg">
          <h2 class="text-lg md:text-xl lg:text-2xl pt-5 text-ellipsis overflow-hidden">{{post.title}}</h2>
        </a>
      </div>
      <div class="pt-2">
        {% for tag in post.tags limit:3 %}
        <span class="text-xs text-slate-700 dark:text-slate-100/80 align-middle">#{{tag}}</span>
        {% endfor %}
      </div>
    </div>
    {% endif %}
  {% endfor %}
</div>

---

## Notes from the Field

<div id="blog" class="md:w-4/5 mx-auto gap-4 md:gap-6 columns-2 md:columns-3 mb-10">
  {% for post in site.posts %}
    {% unless post.tags contains 'portfolio' %}
    <div class="md:fadeIn pb-8 mb-8 break-inside-avoid-column ">
      <div class="hover:underline hover:decoration-2 hover:underline-offset-4 transition ease-in-out delay-150 hover:-translate-y-1 hover:scale-104 duration-300">
        <a href="{{ post.url | relative_url }}">
          <img src="{{ post.image | relative_url }}" alt="" class="w-full max-w-screen-sm h-auto shadow-md rounded-lg">
          <h2 class="text-lg md:text-xl lg:text-2xl pt-5 text-ellipsis overflow-hidden">{{post.title}}</h2>
        </a>
      </div>
      <div class="pt-2">
        {% for tag in post.tags limit:3 %}
        <span class="text-xs text-slate-700 dark:text-slate-100/80 align-middle">#{{tag}}</span>
        {% endfor %}
      </div>
    </div>
    {% endunless %}
  {% endfor %}
</div>

---

## Let's work together!

Feel free to send a message to inquire about a project, speaking opportunity, or just to say hey!

<div id="contact">
<form action="https://formspree.io/f/mvgklnaj" method="POST" class="mt-6 space-y-4 max-w-md mx-auto">
  <label class="block">
    <span class="text-gray-700 dark:text-gray-300">First & Last Name</span>
    <input type="text" name="name" required class="mt-1 block w-full border rounded-md p-2 bg-white dark:bg-gray-800 border-gray-300 dark:border-gray-600 text-gray-900 dark:text-white">
  </label>

  <label class="block">
    <span class="text-gray-700 dark:text-gray-300">Email</span>
    <input type="email" name="_replyto" required class="mt-1 block w-full border rounded-md p-2 bg-white dark:bg-gray-800 border-gray-300 dark:border-gray-600 text-gray-900 dark:text-white">
  </label>

  <label class="block">
    <span class="text-gray-700 dark:text-gray-300">Message</span>
    <textarea name="message" rows="5" required class="mt-1 block w-full border rounded-md p-2 bg-white dark:bg-gray-800 border-gray-300 dark:border-gray-600 text-gray-900 dark:text-white"></textarea>
  </label>

  <button type="submit" class="w-full px-4 py-2 border rounded text-gray-700 dark:text-white border-gray-300 dark:border-gray-600 hover:bg-gray-200 dark:hover:bg-gray-700 transition-colors duration-200">
    Send Message
  </button>
</form>
</div>