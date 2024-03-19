---
layout: special_event_layout
id: hojdpunkten
header-img: /imgs/hojdpunkten/hojdpunkten_header_2024.png
permalink: /hojdpunkten/
# content
title: #Höjdpunkten
title-size: 7vw,60px
title-color: black
subtitle: #En lagtävling i matematisk problemlösning för  högstadiet, gymnasiet och övriga!
subtitle-size: 2.6vw, 27px
subtitle-color: black
---

I [inbjudan](ungvetenskapssport.se/assets/event_invets/20240316_inbjudan_hojdpunkten_2024.pdf) kan du läsa mer om årets tävling. Skriv gärna ut förstasidan och sätt upp på din skola!

## Är du intresserad av mattetävlingar i lag?
Höjdpunkten med tre klasser: en för högstadieelever, en för gymnasieelever och en öppen klass. På högstadie- och gymnasieskolor kommer tävlingen äga rum den 8 maj. För de som tävlar i öppen klass eller de som inte haft möjlighet att delta på sina skolor, kommer tävlingen äga rum digitalt den 9 maj.

Joina gärna Ung Vetenskapssports [discordserver](https://discord.gg/GDfJKkTaqb). Den 10 maj kommer vi hålla en läsningsgenomgång för intresserade.

Det kommer finnas fina problem att lösa och fina priser att vinna! Har du frågor kan du mejla [mattetavling@ungvetenskapssport.se](mailto:mattetavling@ungvetenskapssport.se).

Lycka till önskar arrangörsgruppen!




## Tidigare upplagor av Höjdpunkten


<ul>
{% for event in site.data.hojdpunkten %} {% if event.upcoming == false %}
<li>
    <h3> {{ event.year }} </h3>
    <p>Datum: {{ event.date }} </p>
    {% if event.inbjudan %}
    <p><a href="{{ event.inbjudan }}" >Inbjudan</a></p>
    {% endif %}

    {% if event.no_participants %}
    <p>Antal deltagare: {{ event.no_participants }} </p>
    {% endif %}


    <p>Högstadietävling: {% if event.hogstadie_problem_sv %} <a href="{{ event.hogstadie_problem_sv }}" >Svenska</a>{% endif %} {% if event.hogstadie_problem_en %}<a href="{{ event.hogstadie_problem_en }}" >English</a>{% endif %} {% if event.hogstadie_losningar %}<a href="{{ event.hogstadie_losningar }}" >Lösningar</a>{% endif %} {% if event.hogstadie_resultat %}<a href="{{ event.hogstadie_resultat }}" >Resultat</a>{% endif %} </p>

    <p>Gymnasietävling: {% if event.gymnasiet_problem_sv %} <a href="{{ event.gymnasiet_problem_sv }}" >Svenska</a>{% endif %} {% if event.gymnasiet_problem_en %}<a href="{{ event.gymnasiet_problem_en }}" >English</a>{% endif %} {% if event.gymnasiet_losningar %}<a href="{{ event.gymnasiet_losningar }}" >Lösningar</a>{% endif %} {% if event.gymnasiet_resultat %}<a href="{{ event.gymnasiet_resultat }}" >Resultat</a>{% endif %} </p>

    <p>Öppen tävling: {% if event.open_problem_sv %} <a href="{{ event.open_problem_sv }}" >Svenska</a>{% endif %} {% if event.open_problem_en %}<a href="{{ event.open_problem_en }}" >English</a>{% endif %} {% if event.open_losningar %}<a href="{{ event.open_losningar }}" >Solutions</a>{% endif %} {% if event.open_resultat %}<a href="{{ event.open_resultat }}" >Resultat</a>{% endif %} </p>

    <p> {% if event.sources %} <a href="{{ event.sources }}" >Sources</a>{% endif %} and proposers of problems </p>

</li>
{% endif %}{% endfor %}
</ul>
