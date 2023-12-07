---
layout: page
title: Evenemang
id: events
---

## Kommande evenemang
<ul>
{% for event in site.data.events %} {% if event.upcoming == true %}
<li>
    <h3> {{ event.name }} </h3>
    <p> {{ event.startdate }} {% if event.enddate %} - {{ event.enddate }} {% endif %} </p>
    {% if event.location %}
    <p> Plats: {{ event.location }} </p>
    {% endif %}
    {% if event.inbjudan %}
    <p><a href="{{ event.inbjudan }}" >Läs mer...</a></p>
    {% endif %}
</li>
{% endif %}{% endfor %}
</ul>


## Återkommande evenemang
Ung Vetenskapssport är ett levande förbund med många olika evenemang, och vi tror på att du som har en bra idé ska få möjlighet att genomföra den! Det innebär att nya evenemang ofta dyker upp, och ibland försvinner gamla. Ett par evenemang brukar dock återkomma varje år. Klicka på bilderna för att läsa mer om respektive evenemang.

<!-- Idea: make it similar to styrelsen (grid) but an event-image and title only -->
<div class="row">
    {% for event in site.data.recurringevents %} {% if event.current == true %}

    <div class="col-xs-6 col-sm-4 col-md-3 col-lg-3">
    
        <div class="thumbnail" onclick="redirectToLink('{{ event.url }}')">
            {% if event.img %}
            <!-- <a href="{{ event.url }}"><img class="contact-image" src="{{ event.img }}" alt="{{ event.name }}"></a> -->
            <img class="contact-image" style="border:0px" src="{{ event.img }}" alt="{{ event.name }}">
            {% else %} 
            <img class="contact-image" style="border:0px" src="/imgs/other-eventicons/default-eventicon.png" alt="{{ event.name }}">
            {% endif %}


            <div class="caption">
                <h4>{{ event.name }}</h4>
            </div>
        </div>
        <script src="/scripts/redirectOnClick.js"></script>
    </div>
    {% assign mod4 = forloop.index | modulo:4 %}
    {% assign mod3 = forloop.index | modulo:3 %}
    {% assign mod2 = forloop.index | modulo:2 %}
    {% if mod2 == 0 %}
    <div class="clearfix visible-xs-block"></div>
    {% endif %}
    {% if mod3 == 0 %}
    <div class="clearfix visible-sm-block"></div>
    {% endif %}
    {% if mod4 == 0 %}
    <div class="clearfix visible-md-block"></div>
    <div class="clearfix visible-lg-block"></div>
    {% endif %}

    {% endif %}{% endfor %}
</div>


## Tidigare Evenemang
<ul>
{% for event in site.data.events %} {% if event.upcoming != true %}
<li>
    <h3> {{ event.name }} </h3>
    <p> {{ event.startdate }} - {{ event.enddate }} </p>
    <p> Antal deltagare: {{ event.no_participants }} </p>
    <p> Plats: {{ event.location }} </p>
    {% if event.inbjudan %}
    <p><a href="{{ event.inbjudan }}" >Läs mer...</a></p>
    {% endif %}
    {% if event.media %}
    <p><a href="{{ event.media }}" >Om evenemanget i media...</a></p>
    {% endif %}
    {% if event.resultat_och_problem %}
    <p> Resultat och problem hittar du <a href="{{ event.resultat_och_problem }}" >här</a>.</p>
    {% endif %}
</li>
{% endif %}{% endfor %}
</ul>
