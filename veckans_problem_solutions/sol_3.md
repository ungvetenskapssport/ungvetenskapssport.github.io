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

**Lösning Vecka 3**

Först och främst så måste $x$ och $y$ vara större än $N$ om båda ska vara positiva. Notera nu att $\frac{1}{x} + \frac{1}{y} = \frac{1}{N}$ är ekvivalent med $(N - x)(N - y) = N^2 - Nx - Ny + xy = N^2$. Så för varje positiv lösning $(x,y)$ så är $N-x$ och $N-y$ positiva delare till $N$, eftersom $x,y > N$. Dessutom så kommer varje $x$ sådant att $N - x = d$ är en positiv delare till $N^2$ ge en unik lösning $(x,y) = (N - d, N - \frac{N^2}{d})$. Alltså är totala antalet lösningar precis lika många som antalet delare till $N^2$, som vi ju redan vet är $2005$. Låt $N = p_1^{a_1}p_2^{a_2}...p_k^{a_k}$ vara primtalsfaktoriseringen av $N$. Då är antalet delare till $N^2 = p_1^{2a_1}p_2^{2a_2}...p_k^{2a_k}$ exakt $(2a_1 + 1)...(2a_k + 1) = 2005 = 5 \cdot 401$. Det finns nu bara två möjligheter för $a_1, a_2, ..., a_k$: antingen så är $k = 1$ och $2a_1 + 1 = 2005$ eller så är $k = 2$ och {$2a_1 + 1, 2a_2 + 1$} $=$ {$5, 401$}. I första fallet så är $a_1 = 1002$, så $N = p_1^{1002}$ vilket är en kvadrat. I andra fallet så är {$a_1, a_2$} $=$ {$2, 200$} och $N = p_1^2p_2^{200}$ eller $p_1^{200}p_2^2$ är fortfarande en kvadrat. Så vi är klara!

Gå tillbaka till uppgiften [här](/blog/2020/07/18/veckans-problem-3).
