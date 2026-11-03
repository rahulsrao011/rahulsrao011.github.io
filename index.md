---
layout: default
---

<section class="hero">
  <h1 class="hero-name">{{ site.title }}</h1>
  <p class="hero-tagline">{{ site.tagline }}</p>
</section>

<section class="about" markdown="1">

Hi, I'm Rahul. I build software and write about what I learn along the way. I'm currently looking for new opportunities — feel free to reach out.

</section>

  <p class="contact-line">Find me on <a href="https://github.com/{{ site.github }}" target="_blank" rel="noopener">GitHub&nbsp;&#x2197;</a> and <a href="https://www.linkedin.com/in/{{ site.linkedin }}" target="_blank" rel="noopener">LinkedIn&nbsp;&#x2197;</a>.</p>


{% if site.posts.size > 0 %}
<section class="recent">
  <h2 class="section-title">Recent writing</h2>
  {% include post-list.html posts=site.posts max=5 %}
  {% if site.posts.size > 5 %}<p class="more-link"><a href="{{ '/blog/' | relative_url }}">All posts &rarr;</a></p>{% endif %}
</section>
{% endif %}
