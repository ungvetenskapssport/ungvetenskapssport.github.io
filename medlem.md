---
layout: page
title: Bli medlem i UVS
id: medlem

---

Ung Vetenskapssport är ett förbund av medlemsföreningar. Som medlem i en medlemsförening blir du automatiskt också medlem i förbundet Ung Vetenskapssport! Läs nedan om de ämnen som intresserar dig och välj alla du vill bli medlem i genom att fylla i respektive formulär. ***Det är helt gratis!***

<br>

<div class="row">
    {% for member in site.data.medlemsforeningar %} {% if member.current == true %}

    <div class="col-xs-5 col-sm-4 col-md-3 col-lg-3">
        <div class="thumbnail">
            {% if member.img %}
            <img class="contact-image-no-border" src="{{ member.img }}" alt="{{ member.name }}" style="padding: 5px;">
            {% endif %}
            <div class="caption">
                {% if member.form %}
                <script src="../scripts/redirectOnClick.js"></script>
                <div class="buttonMedlem" onclick="redirectToLink('{{ member.form }}')">
                Bli medlem <i class="fa fa-sign-in"></i>
                </div>
                {% endif %}

                {% if member.sampleproblem %}
                    <!-- <p><a href="{{ member.sampleproblem }}" >Exempelproblem</a></p> -->
                    <div class="buttonInfo" onclick="redirectToLink('{{ member.sampleproblem }}')">
                Exempel<wbr>problem <i class="fa fa-puzzle-piece"></i>
                </div>
                {% endif %}

                {% if member.info_ebas %}
                <div class="buttonInfo" onclick="redirectToLink('{{ member.info_ebas }}')">
                Mer info <i class="fa fa-info-circle"></i>
                </div>
                {% endif %}

                <details>
                    <summary style="display:list-item">Om {{ member.name }}</summary>
                    <p>{{ member.description }}</p>
                </details>
                
                {% if member.city %}
                <p> {{member.city}} </p>
                {% endif %}
                <h3>
                {% if member.github %}
                <a href="https://github.com/{{ member.github }}" target="_blank"><i class="fa fa-github-square"></i></a>
                {% endif %}
                {% if member.website %}
                <a href="https://{{ member.website }}" target="_blank"><i class="fa fa-home"></i></a>
                {% endif %}
                </h3>
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

## Jag är medlem! Vad gör jag nu?
Grattis! Du som är medlem kan ta del av våra aktiviteter. Du kommer att få medlemsbrev med information om planerade aktiviteter och andra nyheter. Utöver detta kan du:
- [Gå med i vår discordserver](https://discord.gg/GDfJKkTaqb)! Här diskuteras tävlingsproblem och möjligheter.
- Gå på något av våra läger! Information skickas ut i våra medlemsbrev och andra kanaler.
- Engagera dig! Läs mer nedan.

### Engagera dig

Att engagera sig ideellt är bland det roligaste och mest givande man kan göra! Vill du hjälpa dig själv och UVS att utvecklas? Grunda ett nytt läger? Ge fler unga chansen att delta i våra aktiviteter? Engagera dig i Ung Vetenskapssport och/eller någon av våra medlemsföreningar! Maila mer än gärna styrelsen om du är intresserad, eller fyll i [detta formulär](https://forms.gle/ieCyvan5bkeEaa2P6)!


### Andra föreningar
Om du gillar Ung Vetenskapssport så finns det många fler föreningar du kanske skulle gilla! Dessa och många fler tips finns på [vår resurssida](../resurser/#organisationer-och-f%C3%B6reningar)!




<img src="/imgs/medlemsforeningar/uvs-medlemsforeningar-website.gif" style="width: 100%; position: relative; left: 0px; max-width: 800px;">