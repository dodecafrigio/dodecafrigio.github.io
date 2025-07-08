---
layout: page
author: chi-sono
title: "Chi sono"
permalink: /chi-sono/       # opzionale, per avere URL “/about/”
current: chi-sono           # deve corrispondere al key in navigation.yml
navigation: True
---
<!-- 1) CSS inline: nasconde l’header standard e costruisce il tuo -->
<style>
/* nasconde l’header e la nav di default */
header.main-header,
.main-nav { display: none; }

/* nuovo header fullscreen */
.custom-header {
  position: relative;
  background: url('{{ "/assets/images/cover4.jpg" | relative_url }}') center/cover no-repeat;
  height: 300px;
}

/* nav interno con logo + menu -->
.custom-header .custom-nav {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  padding: 1rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.custom-nav .blog-logo img {
  height: 2rem;
}

.custom-nav .menu-button {
  color: #fff;
  font-size: 1.5rem;
  background: transparent;
  border: none;
}

/* se vuoi riprendere la classe icon-menu */
.custom-nav .menu-button.icon-menu::before {
  content: "\f0c9";
  font-family: "Font Awesome 5 Free";
  font-weight: 900;
}

/* profilo autore sotto l’header */
.author-profile {
  max-width: 600px;
  margin: -60px auto 2rem; /* solleva la card sul header */
  background: #fff;
  padding: 2rem;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  text-align: center;
  border-radius: 8px;
}

/* avatar rotonda */
.author-profile .avatar {
  width: 120px;
  height: 120px;
  margin: 0 auto 1rem;
  border-radius: 50%;
  background: url('{{ "/assets/images/luca.jpg" | relative_url }}') center/cover no-repeat;
  border: 4px solid #fff;
}

/* nome e descrizione */
.author-profile h1 {
  margin: 0.5rem 0;
  font-size: 1.75rem;
}
.author-profile p.bio {
  font-size: 1rem;
  color: #555;
  line-height: 1.5;
  margin-bottom: 1.5rem;
}

/* metadati: icona + testo */
.author-meta {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1.5rem;
  font-size: 0.95rem;
  color: #666;
}
.author-meta span,
.author-meta a {
  display: flex;
  align-items: center;
  gap: 0.4rem;
  text-decoration: none;
  color: inherit;
}
.auth-icon {
  font-size: 1.2rem;
  color: #999;
}
</style>

<!-- 2) Header personalizzato -->
<div class="custom-header">
  <div class="custom-nav">
    <a class="blog-logo" href="{{ "/" | relative_url }}">
      <img src="{{ "/assets/images/ghost.png" | relative_url }}" alt="Logo">
    </a>
    {% if page.navigation %}
      <button class="menu-button icon-menu" aria-label="Apri menu"></button>
    {% endif %}
  </div>
</div>

<!-- 3) Sezione profilo autore -->
<section class="author-profile">
  <div class="avatar"></div>
  <h1>Luca Scala</h1>
  <p class="bio">
    Dottorando in geometria generalizzata e approcci di double field theory
    alle dualità nella teoria delle stringhe. Supervisori:
    Jerzy Kowalski-Glikman e Falk Hassler.
  </p>

  <div class="author-meta">
    <span><i class="auth-icon fas fa-map-marker-alt"></i>Wrocław, Polonia</span>
    <a href="https://www.fhassler.de/group" target="_blank" rel="noopener">
      <i class="auth-icon fas fa-link"></i>fhassler.de
    </a>
    <span><i class="auth-icon fas fa-file-alt"></i>18 posts</span>
  </div>
</section>

<!-- 4) Il tuo contenuto aggiuntivo -->
## La mia storia

Scrivi qui la tua bio più estesa: studi, interessi, hobby, progetti in corso…
