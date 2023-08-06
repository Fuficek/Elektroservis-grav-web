---
title: Fotogalerie
process:
    markdown: true
    twig: true
media_order: 'montaz01.JPG,montaz02.JPG,montaz03.JPG,montaz04.JPG,montaz05.JPG,montaz06.JPG,montaz07.JPG,montaz08.jpg,montaz09.jpg,montaz10.jpg,montaz11.jpg,montaz12.jpg,montaz13.jpg,montaz14.jpg,montaz15.jpg,montaz16.jpg,montaz17.jpg,montaz18.jpg,montaz19.jpg,plosina01.jpg,plosina02.jpg,plosina03.jpg,plosina04.jpg,plosina05.jpg,plosina06.jpg,plosina07.jpg,plosina08.jpg,plosina09.jpg,plosina10.jpg,plosina11.jpg,plosina12.jpg,plosina13.jpg'
---
<div class="grid-item span2 row1"><h1 class="page__heading span-p">FOTOGALERIE</h1></div>
<div class="gallery--box">
    <div id="lightgallery" class="gallery--list">
        {% for image in page.media.images %}
            <div class="image--item" data-src="{{ image.url }}" data-sub-html="<h4>{{ image.filename|e }}</h4>">
                <a href="">
                    <img class="image--preview" src="{{ image.cropZoom(400, 300).url }}" alt="{{ image.filename|e }}">
                </a>
            </div>
        {% endfor %}
    </div>
</div>