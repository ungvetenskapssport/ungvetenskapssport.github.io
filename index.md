---
layout: page
---

Välkommen till Ung Vetenskapssports hemsida!

Ung Vetenskapssport (UVS) är en ideell förening vars syfte är att skapa mötesplatser och träningsmöjligheter för ungdomar intresserade av problemlösning. Detta görs genom träningsläger inom matematik, programmering, fysik, kemi, biologi och lingvistik samt genom andra problemlösningsinriktade event.

Ung Vetenskapssport består av [sex ämnesspecifika medlemsföreningar](./medlem). Förbundet har som långsiktigt mål att förbättra svensk skolutbildning genom införandet av mer problemlösning i undervisningen vilket stimulerar både intresset och det logiska tänkandet hos eleverna.

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

# Kalender
I denna kalender lägger vi in evenemang som vi organiserar, vilka dagar kvaltävlingarna i de olika vetenskapsolympiaderna för gymnasiet är och annat som vi tror kan vara av intresse för er. Om du använder Google kalender själv så går det bra att prenumerera på den!

<iframe src="https://calendar.google.com/calendar/embed?src=c_dc018de89b41c2214170c97cc3c4459e3973ce58a8cc99f005a66087ba5d11c9%40group.calendar.google.com&ctz=Europe%2FStockholm" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>