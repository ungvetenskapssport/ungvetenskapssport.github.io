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

**Lösning Vecka 6**

Lösning 1: Notera att talen $1111$, $2222$, ..., $9999$ alla är delbara med $101$. Alltså är även $n = 1111222233334444555566667777888899990000$ delbart med $101$. Men $n$ är också delbart med $20$, så det är delbart med $20 \cdot 101 = 2020$ eftersom $101$ och $20$ är relativt prima.

Lösning 2: Det går faktiskt att för varje tal $n$ hitta en multipel av $n$ som har lika många av varje siffra! Betrakta följden $a_1, a_2, ...$ där $a_i$ är talet vi får om vi skriver $123456789$ efter sig själv $i$ gånger. Till exempel så är $a_1 = 123456789$ och $a_3 = 123456789123456789123456789$. Eftersom det bara finns ändligt många restklasser modulo $n$ så måste minst två tal $a_i$ och $a_j$ vara kongruenta modulo $n$, och vi kan till och med garantera att $i - j \geq k$ för vilket $k$ som helst. Om vi nu betraktar $a_i - a_j$ får vi något delbart med $n$. Men $a_i - a_j$ kommer också vara på formen $123456789123456789...123456789000000000...000000000$, där antalet grupper av $123456789$ i början är $i - j \geq k$ och antalet nollor i slutet är $9j$. Vi får alltså att talet $a_{i - j} \cdot 10^{9j}$ är delbart med $n$.

För att avsluta lösningen så väljer vi $k$ ovan stort nog för att $n$ inte ska delas av varken $2$ eller $5$ fler än $k$ gånger. Då kommer $n \mid a_{i-j} \cdot 10^k \mid a_{i-j} \cdot 10^{i-j}$, där det sista talet har precis lika många av varje siffra!

Gå tillbaka till uppgiften [här](/blog/2020/08/08/veckans-problem-6).
