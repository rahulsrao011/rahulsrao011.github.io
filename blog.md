---
layout: default
title: Blog
permalink: /blog/
---

<h1 class="page-title">Blog</h1>

{% if site.posts.size > 0 %}
{% include post-list.html posts=site.posts %}
{% else %}
<p class="muted">No posts yet — check back soon.</p>
{% endif %}
