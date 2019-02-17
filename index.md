---
layout: page
---

Välkommen till Ung Vetenskapssports hemsida!

Ung Vetenskapssport är en ideell förening vars syfte är att skapa mötesplatser och träningsmöjligheter för ungdomar intresserade av problemlösning. Detta görs genom träningsläger inom matematik, programmering, fysik, kemi, biologi och lingvistik samt genom andra problemlösningsinriktade event.

Föreningen har som långsiktigt mål att förbättra svensk skolutbildning till det bättre genom införandet av mer problemlösning i undervisningen vilket stimulerar både intresset och det logiska tänkandet hos eleverna.

Ung Vetenskapssport vill ha lokala verksamheter och kan hjälpa Dig som har en bra idé relaterad till vetenskapssport; om Du är intresserad av att starta en sådan – kontakta någon i styrelsen.

{% for post in paginator.posts %}
<div class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
        <h2 class="post-title">            {{ post.title }}
        </h2>
        {% if post.subtitle %}
        <h3 class="post-subtitle">
            {{ post.subtitle }}
        </h3>
        {% endif %}
    </a>
    <p class="post-meta" style="margin-bottom:5px">Posted by {{ post.author }} on {{ post.date | date: "%B %-d, %Y" }}</p>
</div>
<hr>
{% endfor %}
