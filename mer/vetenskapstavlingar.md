---
layout: page
title: Vetenskapstävlingar
id: vetenskapstavlingar
---
*Denna sida är under konstruktion. <i class="fas fa-wrench"></i>*

Här kan du hitta information om olika vetenskapstävlingar och hur uttagningsprocesserna för dem går till.

<!-- Per competition, compile info and a flowchart -->
{% for comp in site.data.competitions %}
{% if comp.display-details %}
<div>
    <h3>{{ comp.name }} {% if comp.alt-name %} ({{ comp.alt-name}}) {% endif %}  </h3>
        {% if comp.organizer %} <p><b>Arrangör:</b> {{ comp.organizer }}</p> {% endif %}
        {% if comp.participants-qualifiers %} <p><b>Antal deltagare:</b> {{ comp.participants-qualifiers }}</p> {% endif %}
        {% if comp.target %} <p><b>Huvudsaklig målgrupp:</b> {{ comp.target }}</p> {% endif %}
        {% if comp.international-name %} <p><b>Internationell tävling:</b> {{ comp.international-name }}</p> {% endif %}
        {% if comp.participated-since %} <p><b>Deltagit sedan:</b> {{ comp.participated-since }}</p> {% endif %}
        {% if comp.description %} <p>{{ comp.description }}</p> {% endif %}
        {% if comp.url %} <p><a href="{{ comp.url }}">Läs mer om tävlingen här</a></p> {% endif %}
        {% if comp.flowchart %}
        <object data="{{ comp.flowchart }}" type="image/svg+xml" width="90%" height="90%">
            Your browser does not support SVG
        </object>
        {% endif %}
        <br>
        <br>
        <br>
</div>
{% endif %}
{% endfor %}



<!--
## Fysikolympiaden (Wallenbergs fysikpris)
**Tävlingens namn:** Fysikolympiaden


<object data="../imgs/vetenskapstavlingar/flowchart-fysik.svg" type="image/svg+xml" width="100%" height="100%">
    Your browser does not support SVG
</object> -->
