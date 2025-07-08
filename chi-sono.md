---
layout: page
title: "Chi Sono"
permalink: /chi-sono/
current: chi-sono
navigation: true
cover:  /assets/images/cover4.jpg
logo:   /assets/images/nahui-logo.png
location: "Wrocław, Polonia; Napoli, Italia"
assets: /assets/images/luca.jpg
---

<style>
header.main-header.post-head {
  position: relative !important;
  overflow: visible !important;
  padding-bottom: 80px;              /* spazio in basso per mostrare metà cerchio */
}  
header.main-header.post-head::after {
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

@media only screen and (max-width: 900px) {
  header.main-header.post-head {
    padding-bottom: 60px;
  }
  header.main-header.post-head::after {
    width: 90px;
    height: 90px;
    bottom: -45px;
  }
}

/* 4) Mobile e schermi stretti */
@media only screen and (max-width: 500px) {
  header.main-header.post-head {
    padding-bottom: 60px;
  }
  header.main-header.post-head::after {
    width: 70px;
    height: 70px;
    bottom: -35px;
  }
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
<h1 class="profile-title">Luca Scala</h1>

<div style="text-align:center">
  <div class="profile-location">
    <i class="fas fa-map-marker-alt"></i>{{ page.location }}
  </div>
</div>

Ciao! Se sei finito su questa pagina ti chiederai chi io sia. Piacere, sono Luca, nato a Napoli nel 1997 e ora dottorando in fisica teorica a Wrocław, in Polonia. Lavoro a parte, mi interesso di filosofia, mitologia e scrittura e adoro viaggiare. Ultimamente mi sto divertendo a scrivere un po’ di cosette che puoi trovare listate su [pubblicazioni](/pubblicazioni/).
  
La ragione che mi ha portato a passare notti insonni a combattere contro GitHub (sì, mi dispiace ma non mi piace programmare) e aprire questo sito è il desiderio di creare connessioni interessanti con nuove persone.
  
Il nome “Cosmologie Digitali” nasce innanzitutto da un desiderio di pretenziosità che sarebbe stupido negare. Ma poi, al di là di questo, c’è una motivazione più profonda. La cultura accademica, quella definita “alta”, e la cultura popolare, “bassa”, sono spesso considerate elementi in contrapposizione, e difficilmente conciliabili. Questo divario crea una sfiducia dei consumatori di contenuti “pop” verso gli accademici, e degli accademici verso la “pop”-olarizzazione delle loro discipline. Questa sfiducia rallenta e frena l’originalità, e crea un sentore di malcontento, dove artisti e spettatori si sentono continuamente sotto il giudizio gli uni degli altri. Il significato di Cosmologie Digitali sta proprio in questo: un desiderio di mescolare questi aspetti, fare coesistere e autoalimentare la mitopoietica con il meme, la ricerca con il nonsense. Perché abbiamo preso la vita troppo sul serio per millenni; è ora di divertirci a contaminare.
  
Se ti interessa sapere di più sui miei progetti di ricerca, sia in campo scientifico che artistico, salta pure su [progetti](/progetti/).
  
Se hai domande, idee interessanti per collaborare o suggerimenti di sorta, contattami pure pigiando sulle iconcine che trovi in fondo al menù!
