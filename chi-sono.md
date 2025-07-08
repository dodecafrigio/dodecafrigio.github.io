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

/* 1) Rendo il header di default “spazioso” e posizionato */
header.main-header {
  position: relative;
  overflow: visible;    /* importante: consente al cerchio di uscire dal box */
}

/* 2) Sovrascrivo il background se ho page.cover */
header.main-header.has-cover {
  background: url('{{ page.cover | relative_url }}') center/cover no-repeat;
}

/* 3) Creo il cerchio sovrapposto con ::after */
header.main-header.has-cover::after {
  content: "";
  position: absolute;
  bottom: -60px;         /* metà del diametro, così esce per metà */
  left: 50%;
  transform: translateX(-50%);
  width: 120px;          /* diametro del cerchio */
  height: 120px;
  background: url('{{ page.assets | relative_url }}')
              center/cover no-repeat;
  border-radius: 50%;
  border: 4px solid #fff;        /* bordo bianco */
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  z-index: 10;
}

/* 4) Spazio per il titolo appena sotto il cerchio */
.profile-title {
  margin-top: 80px;      /* pari all’altezza che sporge */
  text-align: center;
  font-size: 1.75rem;
  font-weight: bold;
}
</style>

<!-- NON reinserisco un <header> qui: uso quello di default -->

<!-- 5) Titolo centrato subito dopo il default-header -->
<h1 class="profile-title">{{ page.name }}</h1>

<!-- 6) Bio -->
<section class="author-bio inner">
  {{ page.bio }}
</section>
