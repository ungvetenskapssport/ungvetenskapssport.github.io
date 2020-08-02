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

**Lösning Vecka 4**

(a) Notera att $x^3 + y^3$ kan faktoriseras som $(x+y)(x^2 - xy + y^2)$. Om vi väljer $a = b^6$ så får vi att $n^6 + a = n^6 + b^6 = (n^2 + b^2)(n^4 - n^2b^2 + b^4) = (n^2 + b^2)((n^2-b^2)^2 + n^2b^2)$. Om $b$ är minst $2$ så är båda faktorerna heltal större än $1$ oberoende av vad $n$ är. Alltså är $n^6 + 64$ inte ett primtal för något heltal $n$.

(b) Notera att $x^4 + y^4 = x^4 + 2x^2y^2 + y^4 - 2x^2y^2 = (x^2 + y^2)^2 -(\sqrt{2}xy)^2 = (x^2 + y^2 - \sqrt{2}xy)(x^2 + y^2 + \sqrt{2}xy)$. Om vi väljer $a = (\sqrt{2}b)^4$ får vi alltså $n^4 + a = n^4 + (\sqrt{2}b)^4 = (n^2 + 2b^2 - 2bn)(n^2 + 2b^2 + 2bn) = ((n-b)^2 + b^2)((n+b)^2 + b^2)$. Om $b$ är minst $2$ så är båda faktorerna heltal större än $1$ oberoende av vad $n$ är. Alltså är $n^4 + 64$ inte ett primtal för något heltal $n$.

Gå tillbaka till uppgiften [här](/blog/2020/07/25/veckans-problem-4).
