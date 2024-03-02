---
layout: special_event_layout
id: hojdpunkten
header-img: /imgs/hojdpunkten_header.png
permalink: /hojdpunkten/
# content
title: Höjdpunkten
title-size: 7vw,60px
title-color: black
subtitle: En lagtävling i matematisk problemlösning för  högstadiet, gymnasiet och övriga!
subtitle-size: 2.6vw, 27px
subtitle-color: black
---

# Tidigare upplagor av Höjdpunkten

<h3> 2024 </h3>
Mer info kommer snart!

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
