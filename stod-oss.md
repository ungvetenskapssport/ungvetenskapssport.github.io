---
layout: page
title: Stöd oss
id: stod-oss
---
Det enklaste sättet att stötta oss är att bli medlem, [ge en gåva](./#ge-en-gava) eller inleda ett samarbete.

### Bli medlem
Ett enkelt sätt att stötta Ung Vetenskapssport är att bli medlem. Våra föreningar får bidrag från MUCF per medlem 6-25 år. Det är helt gratis att bli medlem och tar bara någon minut. [Bli medlem här!](/medlem)

### Engagera dig
Våra engagerade får ingen ekonomisk ersättning för sitt arbete (däremot är det otroligt lärorikt och kul!) Vi har alltid plats för fler engagerade, så om du vill hjälpa till med något, hör av dig till oss! [Kontakta oss här](mailto:styrelsen@ungvetenskapssport.se?subject=Engagemang) eller fyll i [detta formulär](https://forms.gle/ieCyvan5bkeEaa2P6)!


### MUCF
En av Ung Vetenskapssports största finansieringskällor är MUCF - Myndigheten för ungdoms- och civilsamhällesfrågor. MUCF är en statlig myndighet som arbetar för att stärka det civila samhället och öka ungas inflytande i samhället. Ung Vetenskapssport har fått stöd från MUCF för att bilda förbund och vår målsättning är att uppnå kraven för organisationsbidrag i närtid.


<img src="/imgs/MUCF-webb.png" style="width: 100%; position: relative; left: 0px; max-width: 200px;">


### Sponsorer och samarbetspartners
Vi är alltid intresserade av att samarbeta med företag och organisationer som delar våra värderingar och mål. Vi kan erbjuda exponering på vår hemsida, i våra sociala medier och på våra läger. [Kontakta oss](mailto:styrelsen@ungvetenskapssport.se?subject=Samarbete) gärna för att diskutera samarbeten! 

Tack till våra samarbetspartners och sponsorer! Observera att vissa enbart stöttar specifika projekt eller medlemsföreningar.
<!-- Grid of sponsor logos -->
<!-- use jekyll to iterate through the members of "sponsors.yml" and display
their image in a grid with name as alttext and link to their page onklick. Shadow on hover. No border. -->

<div class="row">
{% for sponsor in site.data.sponsors %}
    <div class="col-xs-6 col-sm-4 col-md-3 col-lg-2">
        <div class="sponsor">
            <a href="{{ sponsor.url }}" target="_blank">
                <img src="{{ sponsor.img }}" alt="{{ sponsor.name }}" class="img-responsive" style="width: 100%; position: relative; left: 0px; max-width: 200px;">
            </a>
        </div>
    </div>
{% endfor %}
</div>

<style>
.sponsor img:hover {
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}
</style>


### Ge en gåva som privatperson eller företag {#ge-en-gava}
Vill du stötta vår verksamhet med en allmän gåva? Nästan alla medel vi får är bundna till någon specifik budgetpost. En allmän gåva ger oss friheten att göra vad vi anser är bäst för Ung Vetenskapssport just nu! Det går bra att sätta in valfritt belopp på vårt bankgiro. Donationer är i regel anonyma, men vi publicerar donerat belopp nedan. Om du vill att vi publicerar ditt namn eller företagsnamn i listan nedan tillsammans med donerat belopp, [mejla förbundets kassör](mailto:kassor@ungvetenskapssport.se?subject=Gåva). Detsamma gäller om du önskar en faktura eller ett tackbrev för din gåva, eller har någon annan förfrågan rörande din gåva. Tusen tack för ditt stöd!

**Bankgiro: 392-5492** 

<!-- Sum all donation.amount and display it -->
{% assign total = 0 %}
{% for amount in site.data.donations %}
  {% assign integerAmount = amount.amount | plus: 0 %}
  {% assign total = total | plus: integerAmount %}
{% endfor %}
**Totalt:**  {{ total }} kr


{% for donation in site.data.donations %}
- {{ donation.date }}: {% if donation.name %}{{ donation.name }}{% else %}Någon{% endif %} skänkte {{ donation.amount }} kr. {% if donation.message %} *"{{ donation.message }}"* {% endif %}
{% endfor %}
