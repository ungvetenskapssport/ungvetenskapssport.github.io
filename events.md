---
layout: page
title: Evenemang
id: events
---

# Kommande Evenemang

# Tidigare Evenemang

<ul>
{% for event in site.data.events %}
<li>
    <h3> {{ event.name }} </h3>
    <p> {{ event.startdate }} - {{ event.enddate }} </p>
    <p> Antal deltagare: {{ event.no_participants }} </p>
    <p> Plats: {{ event.location }} </p>
</li>
{% endfor %}
</ul>

