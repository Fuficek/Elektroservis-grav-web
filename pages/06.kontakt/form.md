---
title: Kontakt
form:
    name: contact
    fields:
        name:
            label: Name
            placeholder: 'Enter your name'
            autocomplete: 'on'
            type: text
            validate:
                required: true
        email:
            label: Email
            placeholder: 'Enter your email address'
            type: email
            validate:
                required: true
        message:
            label: Message
            placeholder: 'Enter your message'
            type: textarea
            validate:
                required: true
    buttons:
        submit:
            type: submit
            value: Submit
        reset:
            type: reset
            value: Reset
    process:
        save:
            fileprefix: contact-
            dateformat: Ymd-His-u
            extension: txt
            body: '{% include ''forms/data.txt.twig'' %}'
        email:
            from: '{{ form.value.email }}'
            to: matalacek49fuf@gmail.com
            subject: '[Site Contact Form] {{ form.value.name|e }}'
            body: '{% include ''forms/data.html.twig'' %}'
        message: 'Děkujeme, že jste nás kontaktovali. Odpovíme Vám, jakmile to bude možné!'
---

<script>Loader.load()</script>

<div class="grid-container container-inline">
  <div class="grid-item span2 row1"><h1 class="page__heading span-p">Kontaktujte nás</h1></div>
  <div class="grid-item span2 row2 flex-collumn"><p class="span-p">
Zavolejte anebo nám napište... kvalitní komunikace je jeden z pilířů, na kterém stavíme.</p>
</div>
  <div class="grid-item">
  <section class="grid__contact__info">
                <span><p>+420 602 112 719</p></span>
                <span><a href="mailto:hrabal.petr@tiscali.cz">hrabal.petr@tiscali.cz</a></span>
                <span><a target="_blank" href="https://mapy.cz/zakladni?source=firm&id=2508852&ds=2&x=15.3513454&y=50.4254168&z=18">Na výsluní 409, 50601 Jičín - Nové Město, Česko</a></span>
    </section></div>
    <div id="mapa" class="map"></div>

</div>



<script type="text/javascript">
var center = SMap.Coords.fromWGS84(15.3513453, 50.4253758);
var m = new SMap(JAK.gel("mapa"), center, 18);
m.addDefaultLayer(SMap.DEF_BASE).enable();
m.addDefaultControls();

var layer = new SMap.Layer.Marker();
m.addLayer(layer);
layer.enable();

var options = {};
var marker = new SMap.Marker(center, "myMarker", options);
layer.addMarker(marker);
</script>

