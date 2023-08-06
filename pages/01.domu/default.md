---
title: Domů
body_classes: 'title-center title-h1h2'
process.twig: true
process:
    markdown: true
    twig: true
media_order: 'montaz15.jpg,montaz10.jpg'
---

<div class="grid-container container-inline">
  <div class="grid-item span2 row1"><h1 class="word word-delay page__heading span-p">ELEKTROINSTALACE</h1></div>
  <div class="grid-item span2 row2 flex-collumn"><p class="span-p">
Jsme specializovaný elektroservis, který se zaměřuje na kompletní dodávky a práce v oblasti elektrotechniky. Jsme odborníci na průmyslové montáže, elektroinstalace a opravy. Naše služby zahrnují také domovní a zahradní elektroinstalace, hromosvody, revize, montáže a opravy rozvaděčů.</p>
<a href="{{ base_url_relative }}/kontakt" class="button btn41-43 btn-42">Kontaktujte nás!</a>
</div>
  <div class="grid-item"><img class="" src="{{ url('theme://images/montaz10.jpg') }}" alt="plosina"></div>
  <div class="grid-item"><img class="fl-l" src="{{ url('theme://images/montaz15.jpg') }}" alt="plosina"></div>
</div>

<div class="grid-container reduced-margin">
  <div class="grid-item"><img class="" src="{{ url('theme://images/plosina3.png') }}" alt="plosina"></div>
  <div class="grid-item"><h1 class="page__heading h-line_height">PRÁCE S PLOŠINOU</h1>
  <a href="{{ base_url_relative }}/sluzby/prace-s-plosinou" class="button btn41-43 btn-42">Více informací</a></div>
  <div class="grid-item"><img class="" src="{{ url('theme://images/plosina03.jpg') }}" alt="plosina"></div>
  <div class="grid-item"><p>Nabízíme pronájem vysokozdvižné plošiny MP18 s dosahem 18 metrů a bočním dosahem 9,5 metrů, umístěné na lehkém podvozku Nissan Cabstar, s možností obsluhy přímo z pracovního koše a použití i v uzavřeném prostoru.</p></div>
</div>

<div class="grid-container container-inline bounce-7">
  <div class="grid-item span2 row1 flex-collumn"><p p class="span-p">Využijte naše další specializované služby.</p>
  <a href="{{ base_url_relative }}/sluzby" class="box-glow button btn41-43 btn-42">Ostatní služby</a>
  </div>
</div>

<script src="{{ url('theme://aos.js') }}"></script>
<script>
  AOS.init();
</script>
