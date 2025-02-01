---
layout: page
title: Bli medlem i UVS
id: medlem

---

<div class="row">
    {% for member in site.data.medlemsforeningar %} {% if member.current == true %}

    <div class="col-xs-6 col-sm-4 col-md-3 col-lg-3">
        <div class="thumbnail" style="padding: 0px;">
            {% if member.img %}
            <img class="contact-image-no-border" src="{{ member.img }}" alt="{{ member.name }}" style="padding: 5px;" onclick="redirectToLink('{{ member.form }}')">
            {% endif %}
            <div class="caption">
                {% if member.form %}
                <script src="/scripts/redirectOnClick.js"></script>
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
                <div class="button-container">
                    <div class="buttonInfo" onclick="redirectToLink('{{ member.info_ebas }}')">
                    Mer info <i class="fa fa-info-circle"></i>
                    </div>
                    {% if member.email %}
                     <a href="mailto:{{ member.email }}" class="buttonInfo" style="max-width: 3em; margin-left: 0.5em;" role="button" aria-pressed="true"><i class="fa fa-envelope-square"></i></a>
                    {% endif %}
                </div> 
                {% endif %}

                <details>
                    <summary style="display:list-item; font-size:8pt;">Om {{ member.name }}</summary>
                    <p>{{ member.description }}</p>
                </details>
                
                
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

<div style="width: 100%; max-width: 800px; margin: 0 auto;">
    <iframe 
        src="https://clickable-file-magic.lovable.app/" 
        width="100%" 
        height="300px" 
        style="border: none; overflow: hidden;"
        title="Olympic Rings Interactive Component"
    ></iframe>
</div>

***Att bli medlem är helt gratis!*** UVS är ett förbund av medlemsföreningar. Som medlem i en medlemsförening blir du automatiskt också medlem i förbundet Ung Vetenskapssport. Förbundets viktigaste beståndsdel är dess medlemmar. Det är medlemmarna som är delaktiga i förbundets verksamhet, och det är för medlemmarna som förbundet finns. Fler medlemmar för föreningen är bara bra: vi får bidrag och fler personer får en möjlighet att ta del av vår verksamhet!

Att bli medlem är helt gratis. Som medlem får du ta del av vår verksamhet, rösta på årsmöten och vi kommer även skicka utskick till dig om våra aktiviteter.

Vi får bidrag för personer som är upp till 25 år gamla. Självfallet är du välkommen som medlem även om du är äldre än 25 år! 

## Jag är medlem! Vad gör jag nu?
Grattis! Du som är medlem kan ta del av våra aktiviteter. Du kommer att få medlemsbrev med information om planerade aktiviteter och andra nyheter. Utöver detta kan du:
- [Gå med i vår discordserver](https://discord.gg/GDfJKkTaqb)! Här diskuteras tävlingsproblem och möjligheter.
- Gå på något av våra läger! Information skickas ut i våra medlemsbrev och andra kanaler.
- Om du gillar UVS får du gärna sätta upp en av våra affischer!
- Engagera dig! Läs mer nedan.
<div class="buttonInfo" style="max-width: 250px;" onclick="redirectToLink('../affisch/pdfs/uvs-poster-vit-pussel.pdf')">
    Skriv ut UVS-affisch <i class="fa fa-print"></i>
</div>
<script src="/scripts/redirectOnClick.js"></script>

### Engagera dig

Att engagera sig ideellt är bland det roligaste och mest givande man kan göra! Vill du hjälpa dig själv och UVS att utvecklas? Grunda ett nytt läger? Ge fler unga chansen att delta i våra aktiviteter? Engagera dig i Ung Vetenskapssport och/eller någon av våra medlemsföreningar! Maila mer än gärna styrelsen om du är intresserad, eller fyll i [detta formulär](https://forms.gle/ieCyvan5bkeEaa2P6)!

### Förbundet Ung Vetenskapssport -- ett projekt med stöd av MUCF
Ung Vetenskapssport har beviljats projektbidrag från Myndigheten för ungdoms- och civilsamhällesfrågor (MUCF) för att utveckla verksamheten. Detta projekt pågår höst 2023- vår 2024. Projektet syftar till att utveckla förbundet och dess medlemsföreningar till att uppnå kraven för organisationsbidrag för barn och ungdomsorganisationer. Förhoppningen är att förbundet ska kunna söka organisationsbidrag från MUCF redan med 2023 års underlag och behöver för detta bland annat uppnå totalt 1000 medlemmar i medlemsföreningarna - ett mål vi med glädje tar oss an! Att få organisationsbidrag vore ett stort steg i riktningen mot att göra vetenskapssport till ett etablerat koncept i Sverige. Det är även ett steg mot att göra förbundet mer hållbart och långsiktigt när vi växer!

Projektet syftar även till att öka antalet medlemmar i förbundet och dess medlemsföreningar. Projektet finansieras med hjälp av projektbidrag från Myndigheten för Ungdoms- och Civilsamhällesfrågor.




<img src="/imgs/MUCF-webb.png" style="width: 100%; position: relative; left: 0px; max-width: 200px;">


### Andra föreningar
Om du gillar Ung Vetenskapssport så finns det många fler föreningar du kanske skulle gilla! Dessa och många fler tips finns på [vår resurssida](../resurser/#organisationer-och-f%C3%B6reningar)!


<img src="/imgs/medlemsforeningar/uvs-medlemsforeningar-website.gif" style="width: 100%; position: relative; left: 0px; max-width: 800px;">