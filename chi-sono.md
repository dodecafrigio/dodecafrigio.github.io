---
layout: page
author: chi-sono
title: "Chi sono"
permalink: /chi-sono/       # opzionale, per avere URL “/about/”
current: chi-sono           # deve corrispondere al key in navigation.yml
navigation: True
---
<!-- 1) Stili inline per hero e card profilo -->
<style>
/* nascondi l’header standard */
header.main-header { display: none !important; }

/* HERO BANNER */
.hero {
  width: 100%;
  height: 320px;
  background: url('{{ "/assets/images/ghost-bg.jpg" | relative_url }}')
              center/cover no-repeat;
  position: relative;
}
.hero .hero-title {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  color: #fff;
  font-size: 4rem;
  text-transform: uppercase;
  letter-spacing: .5rem;
}

/* PROFILE CARD */
.profile-card {
  max-width: 600px;
  margin: -60px auto 2rem;
  background: #fff;
  padding: 2rem;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  border-radius: 8px;
  text-align: center;
}
.profile-card .avatar {
  width: 120px;
  height: 120px;
  margin: -80px auto 1rem;
  background: url('{{ "/assets/images/luca.jpg" | relative_url }}')
              center/cover no-repeat;
  border-radius: 50%;
  border: 4px solid #fff;
}
.profile-card h1 {
  margin: .5rem 0;
  font-size: 1.75rem;
}
.profile-card p.bio {
  font-size: 1rem;
  color: #555;
  line-height: 1.5;
  margin-bottom: 1.5rem;
}
.profile-card .meta-list {
  list-style: none;
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  font-size: .95rem;
  color: #666;
  padding: 0; margin: 0;
}
.profile-card .meta-list li {
  display: flex;
  align-items: center;
  gap: .4rem;
}
</style>

<!-- 2) HERO SECTION -->
<section class="hero">
  <h1 class="hero-title">ghost</h1>
</section>

<!-- 3) PROFILE CARD -->
<section class="profile-card">
  <div class="avatar"></div>
  <h1>Luca Scala</h1>
  <p class="bio">
    Dottorando in geometria generalizzata e approcci di double field theory
    alle dualità nella teoria delle stringhe. Supervisori:
    Jerzy Kowalski-Glikman e Falk Hassler.
  </p>
  <ul class="meta-list">
    <li><i class="fas fa-map-marker-alt"></i>Wrocław, Polonia</li>
    <li>
      <i class="fas fa-link"></i>
      <a href="https://www.fhassler.de/group" target="_blank" rel="noopener">
        fhassler.de
      </a>
    </li>
    <li><i class="fas fa-file-alt"></i>18 posts</li>
  </ul>
</section>

<!-- 4) Qui puoi continuare con altri paragrafi Markdown -->
