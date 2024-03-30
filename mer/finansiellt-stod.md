---
layout: page
id: finansiellt-stod
title: Finansiellt stöd
# permalink: /finansiellt-stod/
---

Har du inte råd att delta i någon vetenskapssports-aktivitet? Då kan du potentiellt söka finansiellt stöd från Ung Vetenskapssport. Vårt mål är att ingen ska hindras från att delta i våra aktiviteter av ekonomiska skäl. Läs mer nedan.

## Vad kan jag söka stöd för?
Finansiellt stöd kan beviljas för bland annat:
- Deltagaravgifter
- Resor till och från aktiviteter

Aktiviteten du söker för måste verka i linje med Ung Vetenskapssports syfte och mål. Deltagande i alla Ung Vetenskapssports aktiviteter är generellt sett öppna för ansökan om finansiellt stöd. Det går även att söka för liknande aktiviteter som inte arrangeras av UVS. Vid bedömningen tar vi hänsyn till andra möjligheter att få stöd, till exempel från din skola, eller från andra organisationer om evenemanget inte arrangeras av UVS. Resekostnader ska vara skäliga i förhållande till resans längd och syfte. Vid beviljande ges ersättning mot kvitto.

Vi försöker att vara så flexibla som möjligt, så tveka inte att kontakta oss om du är osäker på om din aktivitet kan vara berättigad till stöd. Vi ser gärna att du som ansöker om stöd är medlem i Ung Vetenskapssport. Du kan bli medlem gratis [här](/medlem).

## Hur ansöker jag?
För att ansöka om finansiellt stöd, fyll i ansökningsformuläret nedan. Ansökan behandlas löpande och du får besked så snart som möjligt. Om du har frågor eller funderingar, tveka inte att kontakta oss. Observera att ansökningar måste skickas in i god tid före aktiviteten. Fler detaljer finns i ansökningsformuläret.
<!-- Button with a link to the questionnaire -->

<a href="https://docs.google.com/forms/d/e/1FAIpQLSdh0aJxxRBZdEBbk72K2Jdhi-msMSUSYS6jMdapw89waOMUrQ/viewform?usp=sf_link" class="btn btn-primary">Ansökningsformulär</a>

## Kontakt
Vid frågor om finansiellt stöd, kontakta oss på [stod@ungvetenskapssport.se](mailto:stod@ungvetenskapssport.se).


## Tack
Vi vill rikta ett stort tack till våra sponsorer som gör det möjligt för oss att erbjuda finansiellt stöd till våra deltagare. Ett särskilt tack till Beijerstiftelsen som generöst stöttade pilotprojektet med finansiellt stöd redan 2023.

*Totalt har Ung Vetenskapssport kunnat fördela över 35 000 kr i finansiellt stöd till ungdomar som annars inte hade haft möjlighet att delta i våra aktiviteter. Vi är tacksamma för allt stöd vi får och hoppas kunna fortsätta erbjuda finansiellt stöd till fler deltagare i framtiden.* 

*Fonden för finansiellt stöd är beroende av donationer och sponsorer. Vill du stötta detta arbete? Läs mer under [**Stöd oss**](/stod-oss).*

<!-- Visa sponsorers logga -->
<div class="row">
{% for sponsor in site.data.sponsors %}
{% if sponsor.finansiellt-stod %}
    <div class="col-xs-6 col-sm-4 col-md-3 col-lg-2">
        <div class="sponsor">
            <a href="{{ sponsor.url }}" target="_blank">
                <img src="{{ sponsor.img }}" alt="{{ sponsor.name }}" class="img-responsive" style="width: 100%; position: relative; left: 0px; max-width: 200px;">
            </a>
        </div>
    </div>
{% endif %}
{% endfor %}
</div>

<style>
.sponsor img:hover {
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}
</style>