---
layout: page
antal_medlemsforeningar: åtta
---

<!--textbook style definition with syllable division of vetenskapssport-->

<div className="max-w-3xl mx-auto">
  <Card className="bg-white shadow-lg">
    <CardContent className="p-8 font-times">
      <div style="border: 2px solid black; padding: 10px;">
        <h1 className="text-4xl font-bold text-[#403E43] mb-2">
          ve·ten·skaps·sport
        </h1>
        
        <div className="text-lg text-[#8A898C] mb-4">
          /veːtənskapsspoːʈ/ <span className="italic font-bold text-black text-xl ml-4"><strong>subs.</strong></span>
        </div>

        <hr style="border: 1px solid black;"> 
        <!-- Black horizontal line -->

        <div className="space-y-6">
          <section>
            <p className="text-black leading-relaxed">
                Vetenskaplig problemlösning med eller utan tävlingsmoment. Kan innefatta både individuella och lagbaserade utmaningar.
            </p>
          </section>
        </div>
      </div>
    </CardContent>
  </Card>
</div>

<!--Vetenskapssport, substantiv
Betydelse: Vetenskaplig problemlösning med eller utan tävlingsmoment
Exempel: "Läger för vetenskapssport lockar ungdomar från hela landet."-->
<br>

Ung Vetenskapssport (UVS) är en ideell förening vars syfte är att skapa mötesplatser och träningsmöjligheter för ungdomar intresserade av problemlösning.

Ta del av vår verksamhet och stötta oss genom att bli medlem i förbundets [{{ page.antal_medlemsforeningar }} ämnesspecifika medlemsföreningar](./medlem)! Mer om våra evenemang finns [här](/events).

Har du en bra idé, en fundering eller förfrågan – tveka inte att [kontakta styrelsen](mailto:styrelsen@ungvetenskapssport.se).

Välkommen hit!

<img src="/imgs/medlemsforeningar/uvs-medlemsforeningar-website-small.webp" style="width: 100%; position: relative; left: 0px; max-width: 100px;">

Hälsningar, <br>
[Styrelsen för Ung Vetenskapssport](./styrelsen.md)

<!-- Bli medlem-knapp som länkar till bli-medlem sidan -->
<a href="./medlem" class="buttonInfo" style="max-width: 220px;" role="button" aria-pressed="true"><b>Våra föreningar</b></a>

# Nyheter
<ul class="posts">
    {% for post in site.posts  limit:6%}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
    {% endfor %}

    <details>
    <summary>äldre nyheter...</summary>

    {% for post in site.posts offset:6 %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
    {% endfor %}
    </details>
</ul>

## Vetenskapstävlingar för gymnasister
<ul>
{% for comp in site.data.competitions %}
<li>
<a href="{{comp.url}}">{{comp.subject}} - {{comp.name}}</a>
</li>
{% endfor %}
</ul>

## Vad är vetenskapssport?
Vetenskaplig problemlösning liknar på många sätt sport: träning ger färdighet, det är kul att göra i grupp och det kan förekomma tävlingsmoment. Ung Vetenskapssport fokuserar på två delar:
- Löpande träningsmöjligheter inom vetenskaplig problemlösning
- Tävlingar och förberedelser inför dessa

Något många inte känner till är att det liksom fotboll finns internationella tävlingar inom vetenskapliga ämnen som varje år drar hundratals deltagare från över hundra olika länder. I vår förening finns många tidigare landslagsmedlemmar och finalister från dessa tävlingar som gärna delar med sig av sina erfarenheter och lärdomar. Vi har även många nybörjare eller personer som inte tävlar alls. Vad vi har gemensamt är vår nyfikenhet och vilja att lära oss mer om vetenskap och att lösa problem.

Ung Vetenskapssport har som långsiktigt mål att förbättra svensk skolutbildning genom införandet av mer problemlösning i undervisningen vilket stimulerar både intresset och det logiska tänkandet.

## Kalender

<style>
  @media (max-width: 768px) {
    .calendar-iframe {
      width: 100%;
      height: 400px;
    }
  }
</style>

I denna kalender lägger vi in evenemang som vi organiserar, vilka dagar kvaltävlingarna i de olika vetenskapsolympiaderna för gymnasiet är och annat som vi tror kan vara av intresse för er. Om du använder Google kalender själv så går det bra att prenumerera på den!

<iframe class="calendar-iframe" src="https://calendar.google.com/calendar/embed?height=600&wkst=2&bgcolor=%23ffffff&ctz=Europe%2FStockholm&showTitle=1&mode=MONTH&hl=sv&showNav=1&showDate=1&showPrint=1&showTabs=1&showCalendars=1&showTz=1&src=Y19kYzAxOGRlODliNDFjMjIxNDE3MGM5N2NjM2M0NDU5ZTM5NzNjZTU4YThjYzk5ZjAwNWE2NjA4N2JhNWQxMWM5QGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20&color=%23009688" style="border-width:0" width="800" height="600" frameborder="0" scrolling="no"></iframe>