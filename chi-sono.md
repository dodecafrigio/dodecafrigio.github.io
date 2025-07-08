---
layout: page
title: "Chi sono"
permalink: /chi-sono/
current: chi-sono
navigation: true

# campi autore in front-matter
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
url_full:"https://www.fhassler.de/group"
---

<style>
/* 1) Nascondi l’header standard (non author-head) */
header.main-header:not(.author-head) {
  display: none !important;
}

/* 2) Prepara l’author‐header */
header.main-header.author-head {
  position: relative;
  height: 300px;
  background: url('{{ page.cover | relative_url }}') center/cover no-repeat;
  overflow: visible;    /* <— fondamentale per far uscire l’avatar */
  margin-bottom: 80px;  /* spazio per avatar */
}

/* 3) Avatar dentro header */
.author-avatar {
  position: absolute;
  bottom: -60px;
  left: 50%;
  transform: translateX(-50%);
  width: 120px;
  height: 120px;
  background: url('{{ page.assets | relative_url }}') center/cover no-repeat;
  border-radius: 50%;
  border: 4px solid #fff;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  z-index: 10;
}

/* 4) Allineamento titolo e bio */
.section-wrapper {
  max-width: 600px;
  margin: 0 auto 2rem;
  text-align: center;
}
.author-profile.inner {
  padding-top: 20px;  /* lascia respiro sotto avatar */
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
.auth
