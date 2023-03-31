---
layout: page
title: Bli medlem i UVS
id: medlem

---

Ung Vetenskapssport är ett förbund av medlemsföreningar. Som medlem i en medlemsförening blir du automatiskt också medlem i förbundet Ung Vetenskapssport! Läs nedan om de ämnen som intresserar dig och välj alla du vill bli medlem i genom att fylla i respektive formulär. Det är helt gratis!

<br>

<div class="row">
    {% for member in site.data.medlemsforeningar %} {% if member.current == true %}

    <div class="col-xs-5 col-sm-4 col-md-3 col-lg-3">
        <div class="thumbnail">
            {% if member.img %}
            <img class="contact-image-no-border" src="{{ member.img }}" alt="{{ member.name }}">
            {% endif %}
            <div class="caption">
                <h4>{{ member.name }}</h4>
                <p> {{ member.description }}</p>
                {% if member.city %}
                <p> {{member.city}} </p>
                {% endif %}
                <h2>
                {% if member.form %}
                <a href="{{ member.form }}" target="_blank" rel="noopener noreferrer">Bli medlem <i class="fa fa-sign-in"></i></a>
                {% endif %}
                {% if member.github %}
                <a href="https://github.com/{{ member.github }}" target="_blank"><i class="fa fa-github-square"></i></a>
                {% endif %}
                {% if member.website %}
                <a href="https://{{ member.website }}" target="_blank"><i class="fa fa-home"></i></a>
                {% endif %}
                </h2>
            </div>
        </div>
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


Förbundets viktigaste beståndsdel är dess medlemmar. Det är medlemmarna som är delaktiga i förbundets verksamhet, och det är för medlemmarna som förbundet finns. Fler medlemmar för föreningen är bara bra: vi får bidrag och fler personer får en möjlighet att ta del av vår verksamhet!

Att bli medlem är helt gratis. Som medlem får du ta del av vår verksamhet, rösta på årsmöten och vi kommer även skicka utskick till dig om våra aktiviteter.

Vi får bidrag för personer som är upp till 25 år gamla. Självfallet är du välkommen som medlem även om du är äldre än 25 år! 

## Engagera dig

Att engagera sig ideellt är bland det roligaste och mest givande man kan göra! Vill du hjälpa dig själv och UVS att utvecklas? Grunda ett nytt läger? Ge fler unga chansen att delta i våra aktiviteter? Engagera dig i Ung Vetenskapssport och/eller någon av våra medlemsföreningar! Maila mer än gärna styrelsen om du är intresserad, eller fyll i [detta formulär](https://forms.gle/ieCyvan5bkeEaa2P6)!


## Andra föreningar
Vi vill även tipsa om en annan förening som på många sätt ligger i linje med UVS verksamhet och mål: [Kodsport Sverige](https://kodsport.se/). Läs mer på deras hemsida.




<img src="/imgs/medlemsforeningar/uvs-medlemsforeningar-website.gif" style="width: 100%; position: relative; left: 0px;">