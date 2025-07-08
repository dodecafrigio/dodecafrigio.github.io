---
layout: page
title: "Luca Scala"
permalink: /chi-sono/
current: chi-sono
navigation: true
cover:  /assets/images/cover4.jpg
logo:   /assets/images/nahui-logo.png
location: "Wrocław, Polonia; Napoli, Italia"
bio: >-
  A paranormal expert and his daughter bunk in an abandoned house
  populated by 3 mischievous ghosts and a friendly one, Casper.
assets: /assets/images/luca.jpg
---

<style>
header.post-header .post-title,
header.post-header .page-title {
  display: none !important;
}
  
header.main-header {
  position: relative;
  overflow: visible;    
}

header.main-header.has-cover {
  background: url('{{ page.cover | relative_url }}') center/cover no-repeat;
}

header.main-header.has-cover::after {
  content: "";
  position: absolute;
  bottom: -60px;         
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

.profile-title {
  display: block;
  margin: 2rem auto 1rem;  /* distanza sopra e sotto */
  text-align: center;
  font-size: 2.5rem;       /* ingrandisci il font */
  font-weight: bold;
  color: #333;
  line-height: 1.2;
}

  /* icona + testo della location, centrati e color bio */
.profile-location {
  display: inline-flex;      /* raggruppa icona+testo */
  align-items: center;
  gap: .5rem;
  color: #555;
  font-size: 1.5rem;
  margin: 0 auto 2rem;       /* top=0, bottom=2rem, auto orizz. */
  text-align: center;
}

/* la classe .fas di Font Awesome già contiene font-family;
   nel caso servisse puoi aggiustare la dimensione dell’icona: */
.profile-location .fa-map-marker-alt {
  font-size: 2rem;
}
</style>

<!-- 5) Titolo centrato subito dopo il default-header -->
<h1 class="profile-title">{{ page.title }}</h1>

<div style="text-align:center">
  <div class="profile-location">
    <i class="fas fa-map-marker-alt"></i>{{ page.location }}
  </div>
</div>

<!-- 6) Bio -->
<section class="author-bio inner">
  {{ page.bio }}
</section>
