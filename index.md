---
layout: page
---

Ung Vetenskapssport (UVS) är en ideell förening vars syfte är att skapa mötesplatser och träningsmöjligheter för ungdomar intresserade av problemlösning. Detta görs genom träningsläger inom matematik, programmering, fysik, kemi, biologi och lingvistik samt genom andra problemlösningsinriktade event.

Bli medlem i en av förbundets [sex ämnesspecifika medlemsföreningar](./medlem)! Ung Vetenskapssport har som långsiktigt mål att förbättra svensk skolutbildning genom införandet av mer problemlösning i undervisningen vilket stimulerar både intresset och det logiska tänkandet hos eleverna.

UVS vill ha lokala verksamheter och kan hjälpa dig som har en bra idé relaterad till vetenskapssport; om du är intresserad av att starta en sådan – [kontakta någon i styrelsen](mailto:styrelsen@ungvetenskapssport.se).

Välkommen hit!

<img src="/imgs/medlemsforeningar/uvs-medlemsforeningar-website.gif" style="width: 800%; position: relative; left: 0px; max-width: 100px;">

Hälsningar, [Styrelsen för Ung Vetenskapssport](./styrelsen.md)

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
    <li><span>01 Jun 2023</span> &raquo; <a href="/fa-lager">Fysik- och Astronomiläger 2023</a></li>
    {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

# Kalender
I denna kalender lägger vi in evenemang som vi organiserar, vilka dagar kvaltävlingarna i de olika vetenskapsolympiaderna för gymnasiet är och annat som vi tror kan vara av intresse för er. Om du använder Google kalender själv så går det bra att prenumerera på den!

<iframe src="https://calendar.google.com/calendar/embed?height=600&wkst=2&bgcolor=%23ffffff&ctz=Europe%2FStockholm&showTitle=1&mode=MONTH&hl=sv&showNav=1&showDate=1&showPrint=1&showTabs=1&showCalendars=1&showTz=1&src=Y19kYzAxOGRlODliNDFjMjIxNDE3MGM5N2NjM2M0NDU5ZTM5NzNjZTU4YThjYzk5ZjAwNWE2NjA4N2JhNWQxMWM5QGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20&color=%23009688" style="border-width:0" width="800" height="600" frameborder="0" scrolling="no"></iframe>
