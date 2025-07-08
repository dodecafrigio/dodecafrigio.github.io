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

<style>
/* 1) Header con cover e overflow visibile */
header.main-header {
  position: relative;
  height: 300px;
  background: url('{{ page.cover | relative_url }}') center/cover no-repeat;
  overflow: visible;
}

/* 2) Cerchio avatar sovrapposto (diametro 120px) */
.cover-avatar {
  position: absolute;
  bottom: -60px;                   /* metà del diametro esce fuori */
  left: 50%;
  transform: translateX(-50%);
  width: 120px;
  height: 120px;
  background: url('{{ page.assets | relative_url }}')
              center/cover no-repeat;
  border-radius: 50%;
  border: 4px solid #fff;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  z-index: 10;
}

/* 3) Titolo centrato appena sotto il cerchio */
.profile-title {
  margin-top: 80px;    /* spazio per non sovrapporsi all’avatar */
  text-align: center;
  font-size: 1.75rem;
  font-weight: bold;
  color: #333;
}
</style>

<!-- === featured header (cover + nav generico del tema) === -->
<header class="main-header has-cover" aria-label="Header Chi sono">
  {% if page.navigation %}
    <a class="menu-button icon-menu" href="#"><span class="word">Menu</span></a>
  {% endif %}

  <!-- Avatar inserito dentro l’header -->
  <div class="cover-avatar"></div>
</header>

<!-- === nome autore centrato sotto l’avatar === -->
<h1 class="profile-title">{{ page.name }}</h1>

<!-- === bio === -->
<section class="author-bio inner">
  {{ page.bio }}
</section>
