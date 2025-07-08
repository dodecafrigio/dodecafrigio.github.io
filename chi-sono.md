---
layout: page
title: "Chi sono"
permalink: /chi-sono/
current: chi-sono
navigation: true
cover:  /assets/images/cover4.jpg
logo:   /assets/images/nahui-logo.png
name:   "Luca Scala"
location: "Wrocław, Polonia; Napoli, Italia"
bio: >-
  A paranormal expert and his daughter bunk in an abandoned house
  populated by 3 mischievous ghosts and a friendly one, Casper.
assets: /assets/images/luca.jpg
---

<!-- Featured header -->
<header
  class="main-header author-head{% if page.cover %} has-cover{% endif %}"
  {% if page.cover %}
    style="background-image:url({{ page.cover | relative_url }});"
  {% endif %}>
  <nav class="main-nav overlay clearfix">
    {% if page.logo %}
      <a class="blog-logo" href="{{ "/" | relative_url }}">
        <img src="{{ page.logo | relative_url }}" alt="Logo" />
      </a>
    {% endif %}
    {% if page.navigation %}
      <a class="menu-button icon-menu" href="#"><span class="word">Menu</span></a>
    {% endif %}
  </nav>
</header>

<!-- Author profile -->
<section class="author-profile inner">
  {% if page.assets %}
    <figure class="author-image">
      <div
        class="img"
        style="background-image:url({{ page.assets | relative_url }});">
        <span class="hidden">{{ page.name }}'s Picture</span>
      </div>
    </figure>
  {% endif %}
  <h1 class="author-title">{{ page.name }}</h1>
  {% if page.bio %}
    <div style="text-align: justify; text-justify: inter-word;">
      <h2 class="author-bio">{{ page.bio }}</h2>
    </div>
  {% endif %}
  <div class="author-meta">
    {% if page.location %}
      <span class="author-location icon-location">{{ page.location }}</span>
    {% endif %}
    {% if page.url %}
      <span class="author-link icon-link">
        <a href="{{ page.url_full }}">{{ page.url }}</a>
      </span>
    {% endif %}
  </div>
</section>
