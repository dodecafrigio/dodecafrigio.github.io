---
layout: page
title: "Chi sono"
permalink: /chi-sono/
current: chi-sono
navigation: true

# campi “author‐style”
cover:   /assets/images/cover4.jpg
logo:    /assets/images/ghost.png
name:    "Luca Scala"
location: "Wrocław, Polonia; Napoli, Italia"
bio: >-
  Dottorando in geometria generalizzata e approcci di double field theory
  alle dualità nella teoria delle stringhe. Supervisori:
  Jerzy Kowalski-Glikman e Falk Hassler.
assets:  /assets/images/luca.jpg
url:     "fhassler.de"
url_full: "https://www.fhassler.de/group"
---

<style>
/* 1) nasconde l’header “normale” incluso da layout:page */
header.main-header:not(.author-head) {
  display: none !important;
}

/* 2) imposta altezza, sfondo e posizionamento per l’author‐header */
header.main-header.author-head {
  height: 300px;
  background: url('{{ page.cover | relative_url }}') center/cover no-repeat;
  position: relative;
  margin-bottom: 80px; /* spazio per la propic */
}

/* 3) logo e menu già gestiti dal tema, non serve cambiarli */

/* 4) propic centrata e “galleggiante” */
header.main-header.author-head::after {
  content: "";
  position: absolute;
  bottom: -60px;      /* metà altezza avatar */
  left: 50%;
  width: 120px;
  height: 120px;
  margin-left: -60px; /* metà larghezza avatar */
  background: url('{{ page.assets | relative_url }}') center/cover no-repeat;
  border-radius: 50%;
  border: 4px solid #fff;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}

/* 5) sposta in basso la sezione profilo e centra testo */
.section-wrapper {
  max-width: 600px;
  margin: 0 auto 2rem;
  text-align: center;
}
.author-profile.inner {
  padding-top: 80px; /* per non sovrapporsi all’avatar */
}
.author-title {
  margin-top: 0;
  font-size: 1.8rem;
}
.author-bio {
  margin: 1rem 0;
  color: #555;
  line-height: 1.6;
}
.author-meta {
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  color: #666;
  font-size: .95rem;
}
.author-meta span,
.author-meta a {
  display: flex;
  align-items: center;
  gap: .4rem;
  text-decoration: none;
  color: inherit;
}
.auth-icon {
  font-size: 1.2rem;
  color: #999;
}
</style>

<!-- === featured header (solo author‐head) === -->
<header
  class="main-header author-head has-cover"
  aria-label="Header Chi sono">
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

<!-- === author profile section === -->
<section class="author-profile inner section-wrapper">
  <h1 class="author-title">{{ page.name }}</h1>
  <div>
    <h2 class="author-bio">{{ page.bio }}</h2>
  </div>
  <div class="author-meta">
    <span><i class="auth-icon fas fa-map-marker-alt"></i>{{ page.location }}</span>
    <span>
      <i class="auth-icon fas fa-link"></i>
      <a href="{{ page.url_full }}">{{ page.url }}</a>
    </span>
  </div>
</section>

<!-- === loop dei post dell’autore === -->
<main id="content" class="content" role="main">
  {% assign my_posts = site.posts | where: "author", "chi-sono" %}
  {% for post in my_posts %}
    <article class="post">
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d %B %Y" }}</time>
      {{ post.excerpt }}
    </article>
  {% endfor %}
</main>

