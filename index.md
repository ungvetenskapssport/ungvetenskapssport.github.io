---
layout: page
---

Välkommen till Ung Vetenskapssports hemsida!

Ung Vetenskapssport är en ideell förening vars syfte är att skapa mötesplatser och träningsmöjligheter för ungdomar intresserade av problemlösning. Detta görs genom träningsläger inom matematik, programmering, fysik, kemi, biologi och lingvistik samt genom andra problemlösningsinriktade event.

Föreningen har som långsiktigt mål att förbättra svensk skolutbildning genom införandet av mer problemlösning i undervisningen vilket stimulerar både intresset och det logiska tänkandet hos eleverna.

Ung Vetenskapssport vill ha lokala verksamheter och kan hjälpa dig som har en bra idé relaterad till vetenskapssport; om du är intresserad av att starta en sådan – kontakta någon i styrelsen.

## Vetenskapstävlingar för gymnasister
<ul>
{% for comp in site.data.competitions %}
<li>
<a href="{{comp.url}}">{{comp.subject}} - {{comp.name}}</a>
</li>
{% endfor %}
</ul>

# Nyheter
<ul class="posts">
    {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
