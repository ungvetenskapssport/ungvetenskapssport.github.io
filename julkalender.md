---
layout: page
title: Julkalender
id: julkalender
---

<script type="text/javascript"
        src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.0/MathJax.js?config=TeX-AMS_CHTML"></script>
<script type="text/x-mathjax-config">
MathJax.Hub.Config({
tex2jax: {
inlineMath: [['$','$'], ['\\(','\\)']],
processEscapes: true},
jax: ["input/TeX","input/MathML","input/AsciiMath","output/CommonHTML"],
extensions: ["tex2jax.js","mml2jax.js","asciimath2jax.js","MathMenu.js","MathZoom.js","AssistiveMML.js", "[Contrib]/a11y/accessibility-menu.js"],
TeX: {
extensions: ["AMSmath.js","AMSsymbols.js","noErrors.js","noUndefined.js"],
equationNumbers: {
autoNumber: "AMS"
}
}
});
</script>

Här publicerar vi ett problem varje dag under december 2021! Du kan också hitta problemen i vår story på [instagram](https://www.instagram.com/ungvetenskapssport/).

### Lucka 1
På tavlan står talen $2, 5, 11, 17, 23, 31$. Vad är nästa tal i sekvensen?
<details>
<summary>Visa lösning</summary>
<br>
Sekvensen innehåller vartannat primtal. Därför är nästa tal i talföljden <strong>41</strong>.
</details>


### Lucka 2
Nicole ska gå från rutan med 1 till rutan med 2. Hon kan bara gå höger och neråt, och får inte gå genom rutan med ett X. <br>
![Rutnät för problemet till lucka 2](../imgs/julkalender_lucka2.png)
<details>
<summary>Visa lösning</summary>
<br>
 I varje ruta kan vi skriva på hur många sätt man kan komma till den. Då blir talet i en ruta summan av talen i rutan precis ovanför och till vänster. Så svaret blir <strong>7</strong>.
<br>
<img src="../imgs/julkalender_lucka2_lsg.png">
</details>


### Lucka 3
Hur många reella lösningar har ekvationen
![Ekvationen x^{2021} + 12*x^{21} = 2021 - x](../imgs/julkalender_lucka3.svg)
<details>
<summary>Visa lösning</summary>
<br>
Vi observerar att vänsterledet är strikt ökande, så det kan finnas max en reell lösning. Eftersom vänsterledet är negativt när $x = -2$ och positivt när $x = 24$ så finns en lösning mellan $-2$ och $2$. Därmed finns exakt <strong>1 lösning</strong>.
</details>


### Lucka 4
Fyra positiva heltal står på tavlan. Produkten av de två minsta talen är $45$. Produkten av de två största är $192$. Vad är summan av talen på tavlan?
<details>
<summary>Visa lösning</summary>
<br>
Vi har $45 = 1 \cdot 45 = 3 \cdot 15 = 5 \cdot 9$, och det är alla möjligheter. De två minsta talen är därmed antingen $(1,45)$, $(3,15)$ eller $(5,9)$. Varken $(1,45)$ eller $(3,15)$ kan vara de två minsta, för då skulle de två största talen båda vara minst $15$, men då skulle deras produkt vara minst $15 \cdot 15 = 225 > 192$. Alltså är de två minsta talen $5$ och $9$. De två största talen är då båda större än $9$ och har produkt $192$. Det finns bara en möjlighet som uppfyller detta: $12 \cdot 16 = 192$. Summan av talen är därför $5+9+12+16 = $ <strong>42</strong>.
</details>


### Lucka 5
Tomten ska ut på tur med sin släde som dras av $6$ renar. Renarna står på ett led när de drar släden. De spelar inte så stor roll vilken ordning de står i, förutom att Rudolf måste stå längre fram än Stjärna. Hur många sätt kan de ordnas på så att detta villkor är uppfyllt?
<details>
<summary>Visa lösning</summary>
<br>
Det finns totalt $6! = 1 \cdot 2 \cdot 3 \cdot 4 \cdot 5 \cdot 6 = 720$ sätt att ordna renarna, om vi bortser från det extra villkoret att Rudolf måste stå längre fram än Stjärna. I precis hälften av dessa står Rudolf längre fram än Stjärna så är svaret $\frac{720}{2} = $ <strong>360</strong>.
</details>

### Lucka 6
Björn har i julklapp fått tre primtal som kallas för $x, y$ och $z$ där $x > y > z$. Björn gillar att räkna matte med sina primtal och beräknar att $x + y + z = 56$ och $x - y - z = 30$. Vad blir $xyz$?
<details>
<summary>Visa lösning</summary>
<br>
Addera ekvationerna och få att $2x = 86 \implies x = 43$. Då får vi att $y + z = 13$. När summan av två heltal blir ett udda tal måste ett av dem vara jämnt och ett udda. Det finns endast ett jämnt primtal vilket är $2$ och därmed blir det sista primtalet $11$. Svaret blir därmed $43 \cdot 11 \cdot 2 = $ <strong>946</strong>.
</details>

### Lucka 7
Två tal står på tavlan. Sebastian avrundade talen, som inte nödvändigtvis måste vara heltal, NER och multiplicerade därefter resultaten och fick $100$. När Sebastian tog de ursprungliga talen på tavlan, avrundade talen UPPÅT och multiplicerade resultaten fick han talet X. Vad är det största värdet på X?

<details>
<summary>Visa lösning</summary>
<br>
Den maximala skillnaden när ett och samma tal avrundas ner respektive upp är $1$. Låt kalla de två nedrundade talen för $a$ och $b$. Vi har $ab = 100$, och vi vill att $X = (a+1)(b+1) = ab + a + b + 1 = 101 + a + b$ ska ge ett så stort tal som möjligt. Då $a$ och $b$ båda är heltal fås den största ökningen genom att $a = 1$ och $b = 100$. Detta gör att $X$ maximalt kan vara <strong>202</strong>.
</details>

### Lucka 8
En morgon ska Julia till skolan. I sin strumplåda har hon $2$ gröna, $4$ röda och $9$ vita strumpor. En tredjedel av Julias strumpor är trasiga, dock vet hon inte vilken färg de trasiga strumporna har. Julia tar strumpor från strumplådan och hoppas få två hela strumpor av samma färg. Hur många strumpor måste hon ta för att vara helt säker på att få ett helt par?

<details>
<summary>Visa lösning</summary>
<br>
$5$ strumpor, en tredjedel av alla $15$ strumpor är trasiga. I värsta fallet finns det åtminstone en söndrig strumpa i varje färg. I värsta fall kommer Julia ta alla $5$ söndriga strumpor plus en hel strumpa av var färg. Det är alltså först när Julia tar sin <strong> nionde strumpa</strong> som hon kan vara säker på att det kommer finnas åtminstone ett helt par strumpor i samma färg.
</details>

### Lucka 9
Manja har en $10 \times 10 \times 10$-kub som målats julröd på alla sex sidor. Kuben sönderdelas till småkuber som är i storlek $1 \times 1 \times 1$. Hur många av alla småkuber har julröd färg på sig?

<details>
<summary>Visa lösning</summary>
<br>
De småkuber som inte målats julröda är de som finns innanför i en kub av storlek $8 \times 8 \times 8$. Antalet småkuber som inte målats julröda är därmed $10 \times 10 \times 10 – 8 \times 8 \times 8 =$ <strong>488</strong>.
</details>

### Lucka 10
Ruth har heltalsparet $(x,y)$ där $x \leq y$ och så att produkten $xy$ är fem gånger summan $x+y$. Hon undrar hur många sådana heltalspar det finns?

<details>
<summary>Visa lösning</summary>
<br>
Vi ska hitta heltalslösningar till $5(x + y) = xy$.
<br> Vi har att $5(x + y) = xy \iff 5x – xy + 5y = 0$.
<br> Bryt ut $x$ och subtrahera $25$: $x(5–y) + 5y = 0 \iff x(5–y) + 5y \ – 25 = -25$.
<br> Bryt ut $-5$ ur $5y \ – 25$: $x(5–y) – 5(5–y) = -25 \iff (5–y)(x–5) = -25 \iff (5 – y)(5 – x) = 25$.
<br> Vi söker heltalslösningar $(x,y)$ där $x \leq y$. Notera att $25 = 1 \cdot 25 = (-1) \cdot (-25) = 5 \cdot 5 = (-5) \cdot (-5)$, vilket ger lösningarna $(-20,4)$, $(0,0)$, $(6,30)$ och $(10,10)$. Totalt får vi alltså <strong>4 lösningar</strong>.
</details>

### Lucka 11
Ruth, Manja och Linn tänkte alla köpa en mattebok att ge till Hugo i julklapp. Dessvärre har priset på den eftertraktade matteboken höjts och Ruth saknar $200$ kr för att kunna köpa boken. Manja saknar $400$ kr och Linn saknar $500$ kr. Om de lägger ihop sina pengar räcker det precis till att köpa presenten. Vad kostar matteboken?

<details>
<summary>Visa lösning</summary>
<br>
Om vi betecknar mattebokens kostnad med $K$ får vi följande ekvation:
$(K - 200) + (K - 400) + (K - 500) = K \iff 2K = 1100 \iff K = 550$.
Matteboken kostar alltså <strong>550 kr</strong>.
</details>

### Lucka 12
Hugo har skrivit tal i ett antal boxar och sett till så att summan av fyra boxar i rad alltid är $5$. Julia har varit busig och suddat ut alla tal, förutom de tre tal som syns i figuren nedan. Vilket tal från vänster var det tredje Hugo skrev?
<br>
![Rutnät för problemet till lucka 12](../imgs/julkalender_lucka12.png)
<details>
<summary>Visa lösning</summary>
<br>
En ruta har alltid samma värde som dess grannruta fyra steg till höger respektive fyra steg till vänster. Det är för att, till exempel, så är summan i ruta $1$ till $4$ samma som i ruta $2$ till $5$, så ruta $1$ och $5$ måste ha samma tal i sig eftersom ruta $2$ till $4$ är samma i båda summorna.
<br> I bilden ser vi att låda $8$ har värde $1$. Alltså har låda $4$ också värde $1$. Vidare vet vi att det finns minst en $2$:a i raden, och eftersom alla tal upprepas i var fjärde låda, så måste antingen låda $1$ eller låda $3$ har en $2$:a i sig. Eftersom summan av de fyra första lådorna är $5$ så måste då den av ruta $1$ och $3$ som inte har $2$:an i sig ha $5-0-1-2 = 2$ i sig, så det visar sig att båda låda $1$ och $3$ har en $2$:a. Alltså är svaret <strong>2</strong>.
</details>

### Lucka 13
Björn, Nicole, Sebastian och Marcus går Luciatåg. På varje sång är det en av dem som ska spela piano medan de andra tre sjunger. Det visade sig att Björn sjöng flest gånger av alla, hela sju gånger, medan Nicole sjöng minst antal sånger av alla, bara fyra. Hur många sånger sjöngs totalt i luciatåget?

<details>
<summary>Visa lösning</summary>
<br>
På varje sång skedde tre sånginsatser. Alltså måste det totala antalet sånginsatser vara delbart med 3. Då fyra var det minsta och sju var det största, sjöng Sebastian och Marcus antingen fem eller sex gånger vardera:
<br>$4 + 5 + 5 + 7 = 21$
<br>$4 + 5 + 6 + 7 = 22$
<br>$4 + 6 + 6 + 7 = 23$
<br>$21$ är delbart med $3$. Alltså var antalet sånger $\frac{21}{3} =$ <strong>7</strong>.
</details>

### Lucka 14
Fyra änglar sitter på en julgran bland all pynt. Två av dem hade blå glorior och två hade gula. Änglarna vet inte vem som har vilket sorts gloria, men alla vet vem som kan se vem. Ängel A, som sitter högst upp i granen, kan se änglarna B och C som sitter under honom. Ängel B kan se ängeln C som sitter på grenen under. Ängel C kan inte se någon, eftersom ängel D gömmer sig bakom stammen, så att ingen kan se honom, men han kan inte se någon heller. Vem av dem kan bestämma färgen på sin gloria först och berätta det för andra?

<details>
<summary>Visa lösning</summary>
<br>
Ängeln A kan både se ängeln B och C. Ifall de har samma färg på glorian (båda är gula eller båda är blå), vet A direkt att han då han den andra färgen, och i så fall säger han det. Ifall B och C har olika färg, vet inte A något och då är tyst. Då förstår B att han inte har samma färg som C och då kan han säga sin färg. Därför är det <strong>ängel B</strong> som, oavsett färgfördelning, kan bestämma färgen på sin gloria och berätta det för de andra.
</details>

### Lucka 15
Av $27$ kuber av storleken $1 \times 1 \times 1$ limmade man ihop en kub av storleken $3 \times 3 \times 3$ genom att alla kontaktytor limmades. För att limma ihop två sidor använde en droppe lim varje gång. Hur många droppar lim använde man totalt?

<details>
<summary>Visa lösning</summary>
<br>
$27$ kuber har $6$ ytor var, så totalt $27 \cdot 6 = 162$ ytor. Av dessa så är det några som inte fått något lim på sig, nämligen $9 \cdot 6 = 54$ ytor ($9$ på varje sida av den stora kuben). Så det var $162 - 54 = 108$ ytor som limmades. Varje limdroppe limmade ihop två ytor, därför använde man $\frac{108}{2} =$ <strong>54 limdroppar</strong>.
</details>

### Lucka 16
Manja tar ett heltal och fördubblar det. Därefter fördubblas det igen, sen en gång till. Vilket av följande tal kan vi vara säkra på inte är Manjas slutresultat: $56, 64, 84$?

<details>
<summary>Visa lösning</summary>
<br>
Om vi börjar med talet $x$ så kommer vi efter $3$ fördubblingar ha talet $8x$. Alltså måste slutresultatet vara delbart med $8$. Både $56$ och $64$ är delbara med $8$, men <strong>84</strong> är inte det, så det är vårt svar!
</details>

### Lucka 17
Dario fick en stor säck i julklapp av en väldigt rik person. I säcken ligger sjukt många ädelstenar, gröna och gula, men han kan inte avgöra på formen vilken färg de har. Dario tar ut $100$ ädelstenar på måfå först och sedan $10$ ädelstenar på måfå. När är sannolikheten större att han får lika många stenar av varje färg: i första eller andra fallet?

<details>
<summary>Visa lösning</summary>
<br>
Ju färre ädelstenar man drar, desto större är sannolikheten för att man ska dra lika många av varje färg. Om $N$ stenar dras, så kan resultatet bli på $2^N$ olika sätt (först kommer en gul eller en grön sten, sedan en gul eller en grön och så vidare). I hur många av de fallen har vi lika många av varje sort? Jo, när vi bestämmer oss för vilka i följden som skall vara gröna ($50$ stycken i fallet med $100$ dragna stenar), så har vi ett bestämt utfall, eftersom resten av stenarna måste vara gula. Och att välja $\frac{N}{2}$ stycken bland $N$ kan man göra på $\frac{N!}{(N/2)!(N/2)!}$ olika sätt. Alltså är sannolikheten för att ta ut $\frac{N}{2}$ av varje färg lika med $\frac{1}{2^N} \cdot \frac{N!}{(N/2)!(N/2)!}$.
<br>Vi sätter in våra värden: <br>$\frac{1}{2^{10}}\cdot\frac{10!}{5!\cdot5!}$ är ungefär lika med $0.25$, medan <br>$\frac{1}{2^{100}}\cdot\frac{100!}{50!\cdot50!}$ är ungefär $0.08$.
<br>Alltså är sannolikheten att få ut lika många av varje färg <strong>större när vi drar 10 stenar</strong>. Dessutom kan vi bevisa att sannolikheten är avtagande för växande $N$ (visa med induktion till exempel).
</details>

### Lucka 18
I havet bor bläckfiskar med $6,7$ eller $8$ armar. De som har $7$ armar ljuger alltid, medan de som har $6$ eller $8$ armar alltid talar sanning. Fyra bläckfiskar möttes en gång. Den blåa sa: “Tillsammans har vi $28$ armar”, den gröna sa: “Tillsammans har vi $27$ armar”, den gula: “Tillsammans har vi $26$ armar”, den röda: “Tillsammans har vi $25$ armar”. Hur många armar har varje bläckfisk?

<details>
<summary>Visa lösning</summary>
<br>
Eftersom alla bläckfiskarna sade emot varandra, måste minst tre av dem ha ljugit. Således har minst tre av dem $7$ armar var, det vill säga $21$ armar tillsammans. Om den fjärde bläckfisken också ljuger, så har den $7$ armar. Då har bläckfiskarna tillsammans $28$ armar, vilket är precis vad den blå bläckfisken säger. Men då säger den sanningen och inte kan ljuga, vilket alla bläckfiskarna skulle göra. Denna situation är alltså omöjlig. Den fjärde bläckfisken (som inte är bland de tre som ljuger), talar alltså sanning. Således, om den blå bläckfisken är den som talar sanning, så menar den att den har $7$ armar. Om den gröna talar sanning måste den ha $6$ armar. Den gula – $5$ armar, den röda – $4$ armar. Den enda som kan tala sanning och ha rätt antal armar är alltså den gröna bläckfisken. Den har $6$ armar och alla andra har $7$ armar, vilket blir $27$ armar totalt.
</details>

### Lucka 19
Summan av tre positiva heltal är $11$. Summan av talen kuber är $251$. Hur många taltripplar uppfyller dessa två villkor?
