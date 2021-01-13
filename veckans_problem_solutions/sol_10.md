---
layout: page
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

**Lösning Vecka 10**

Vi visar med hjälp av induktion att vi kan skriva varje positivt heltal $x \leq n!$ som en summa av som mest $n$ delare till $n!$. Med andra ord är planen att först visa att det är sant då $n=1$, och sen visa att om det är sant för $n$ så är det också sant för $n+1$. Om vi lyckas med det kan vi nå alla positiva tal $n$ genom att gå "ett steg i taget".

*Basfall:* Om $n = 1$ så är det uppenbart, det enda giltiga talet är $x = 1$.

*Induktionsantagande:* Antag att alla tal $y \leq (n-1)!$ kan skrivas som en summa av som mest $n-1$ delare till $(n-1)!$.

*Induktionssteg:* Vi vill nu visa att samma sak gäller för alla tal $x \leq n!$. Låt $r$ vara ett tal mellan $0$ och $n-1$ så att $x-r$ är delbart med $n$ ($r$ är alltså resten då $x$ delas med $n$). Låt vidare $y = \frac{x-r}{n}$. Vi vet att $yn = x-r \leq x \leq n!$, vilket ger att $y \leq (n-1)!$. Alltså kan $y$ skrivas som en summa av som mest $n-1$ delare till $(n-1)!$, enligt induktionsantagandet. Om vi nu multiplicerar alla dessa delare med $n$, så kommer de bli delare till $n!$. Vidare kommer deras summa bli precis $n$ gånger större, alltså $yn = x - r$. Slutligen kan vi lägga till talet $r$, som ju är antingen $0$ eller en delare till $n!$ eftersom det är mindre än $n$, och vi har då som mest $n$ tal som antingen är $0$ eller en delare till $n!$, och vars summa är $yn + r = x$. Det fullbordar induktionen.


Gå tillbaka till uppgiften [här](/blog/2020/09/05/veckans-problem-10/).
