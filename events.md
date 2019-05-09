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
    <p> {{ event.startdate }} - {{ event.enddate }} </p>
    <p> Plats: {{ event.location }} </p>
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
</li>
{% endif %}{% endfor %}
</ul>

