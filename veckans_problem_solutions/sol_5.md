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

**Lösning Vecka 5**

Om grodan börjar med att hoppa till vänster så slutar den direkt och kan inte hamna på någon av tre nedersta eller de tre översta gitterpunkterna. Sannolikheten att den *inte* gör det är $\frac{3}{4}$. I så fall kommer den efter första hoppet sitta på en diagonal, och då blir problemet helt symmetriskt i fortsättning. Alltså blir sannolikheten exakt $\frac{1}{2}$ att den efter detta slutar på tre nedersta eller de tre översta gitterpunkterna. Så för att sluta på de tre översta eller tre nedersta måste grodan först hoppa upp, höger eller ner vilket sker med sannolikhet $\frac{3}{4}$, och sen kommer den i hälften av dessa fall sluta längst ner eller längst upp. Svaret blir därför $\frac{3}{4} \cdot \frac{1}{2} = \frac{3}{8}$.

Gå tillbaka till uppgiften [här](/blog/2020/08/01/veckans-problem-5).
