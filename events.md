---
layout: page
title: Evenemang
id: events
---

# Kommande Evenemang

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

# Tidigare Evenemang

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
