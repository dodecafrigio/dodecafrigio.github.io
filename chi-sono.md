---
layout: autore
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
  /* 1) Definisco il diametro avatar via variabile e lo adatto per i breakpoint */
  :root {
    --avatar-diameter: 120px;
  }
  @media (max-width: 900px) {
    :root {
      --avatar-diameter: 90px;
    }
  }
  @media (max-width: 500px) {
    :root {
      --avatar-diameter: 70px;
    }
  }

  /* 2) Blocchetto titolo + location, sempre posizionato sotto l’avatar */
  .profile-block {
    text-align: center;
    /* metà dell’avatar + 1rem di gap */
    margin-top: calc(var(--avatar-diameter) / 2 + 1rem);
    margin-bottom: 2rem;
  }

  .profile-block .profile-title {
    font-size: 4rem;
    margin: 0 0 0.5rem;
    display: block;
  }

  .profile-block .profile-location {
    display: inline-flex;
    align-items: center;
    gap: .5rem;
    color: #555;
    font-size: 1.5rem;
  }
  .profile-block .profile-location .fa-map-marker-alt {
    font-size: 2rem;
  }
</style>

<div class="profile-block">
  <h1 class="profile-title">Luca Scala</h1>
  <div class="profile-location">
    <i class="fas fa-map-marker-alt"></i>{{ page.location }}
  </div>
</div>

Ciao! Se sei finito su questa pagina ti chiederai chi io sia. Piacere, sono Luca, nato a Napoli nel 1997 e ora dottorando in fisica teorica a Wrocław, in Polonia. Lavoro a parte, mi interesso di filosofia, mitologia e scrittura e adoro viaggiare. Ultimamente mi sto divertendo a scrivere un po’ di cosette che puoi trovare listate su [pubblicazioni](/pubblicazioni/).
  
La ragione che mi ha portato a passare notti insonni a combattere contro GitHub (sì, mi dispiace ma non mi piace programmare) e aprire questo sito è il desiderio di creare connessioni interessanti con nuove persone.
  
Il nome “Cosmologie Digitali” nasce innanzitutto da un desiderio di pretenziosità che sarebbe stupido negare. Ma poi, al di là di questo, c’è una motivazione più profonda. La cultura accademica, quella definita “alta”, e la cultura popolare, “bassa”, sono spesso considerate elementi in contrapposizione, e difficilmente conciliabili. Questo divario crea una sfiducia dei consumatori di contenuti “pop” verso gli accademici, e degli accademici verso la “pop”-olarizzazione delle loro discipline. Questa sfiducia rallenta e frena l’originalità, e crea un sentore di malcontento, dove artisti e spettatori si sentono continuamente sotto il giudizio gli uni degli altri. Il significato di Cosmologie Digitali sta proprio in questo: un desiderio di mescolare questi aspetti, fare coesistere e autoalimentare la mitopoietica con il meme, la ricerca con il nonsense. Perché abbiamo preso la vita troppo sul serio per millenni; è ora di divertirci a contaminare.
  
Se ti interessa sapere di più sui miei progetti di ricerca, sia in campo scientifico che artistico, salta pure su [progetti](/progetti/).
  
Se hai domande, idee interessanti per collaborare o suggerimenti di sorta, contattami pure pigiando sulle iconcine che trovi in fondo al menù!

P.S. il logo del sito è ispirato al Quinto Sole della mitologia Nahuatl, [Nahui Ollin](https://en.wikipedia.org/wiki/Nahui_Ollin)!
