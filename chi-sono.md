---
layout: page
title: "Chi sono"
permalink: /chi-sono/       # opzionale, per avere URL “/about/”
current: chi-sono           # deve corrispondere al key in navigation.yml
navigation: True
author: chi-sono
cover: /assets/images/cover4.jpg
logo:  /assets/images/ghost.png
---
<!-- === featured header === -->
<header
  class="main-header author-head{% if page.cover %} has-cover{% endif %}"
  {% if page.cover %}
    style="background-image:url({{ page.cover | relative_url }});"
  {% endif %}>
  <nav class="main-nav overlay clearfix">
    {% if page.logo %}
      <a class="blog-logo" href="{{ '/' | relative_url }}">
        <img src="{{ page.logo | relative_url }}" alt="Logo" />
      </a>
    {% endif %}
    {% if page.navigation %}
      <a class="menu-button icon-menu" href="#"><span class="word">Menu</span></a>
    {% endif %}
  </nav>
</header>

<!-- === author profile === -->
<section class="author-profile inner">
  {% for id, a in site.data.authors %}
    {% if a.username == page.author %}
      {% if a.assets %}
        <figure class="author-image">
          <div class="img"
               style="background-image:url({{ a.assets | relative_url }});">
            <span class="hidden">{{ a.name }}'s Picture</span>
          </div>
        </figure>
      {% endif %}
      <h1 class="author-title">{{ a.name }}</h1>
      {% if a.bio %}
        <div style="text-align: justify; text-justify: inter-word;">
          <h2 class="author-bio">{{ a.bio }}</h2>
        </div>
      {% endif %}
      <div class="author-meta">
        {% if a.location %}
          <span class="author-location icon-location">{{ a.location }}</span>
        {% endif %}
        {% if a.url %}
          <span class="author-link icon-link">
            <a href="{{ a.url_full }}">{{ a.url }}</a>
          </span>
        {% endif %}
        <span class="author-stats">
          <i class="icon-stats"></i>
          {% if paginator.total_posts == 0 %}
            No posts
          {% elsif paginator.total_posts == 1 %}
            1 post
          {% else %}
            {{ paginator.total_posts }} posts
          {% endif %}
        </span>
      </div>
    {% endif %}
  {% endfor %}
</section>

<!-- === eventuale loop dei post === -->
<main id="content" class="content" role="main">
  {% include loop.html %}
</main>
