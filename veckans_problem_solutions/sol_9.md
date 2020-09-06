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

**Lösning Vecka 9**

Ja, det går alltid.

Vi numrerar stolarna från $0$ till $9$, som på bilden nedan. Då kommer varje symmetrilinje motsvaras av att stol $x$ paras ihop med stol $s - x$ modulo $10$, för något tal $s$ som beror på symmetrilinjen. Till exempel gäller för symmetrilinjen i bild (a) att $x$ paras ihop med $5 - x$, och i bild (b) att $x$ paras ihop med $8 - x$. Notera att det är möjligt att $x$ paras ihop med sig själv, till exempel så kommer $4$ och $9$ paras ihop med sig själva i bild (b).

Antag nu att stolarna som redan är upptagna är $a_1, a_2, a_3, a_4$ och $a_5$. För varje par av stolar $x, y$ som redan är upptagna, så finns en unik symmetrilinje sådan att $x$ och $y$ paras ihop. Den symmetrilinjen ges av $s = x + y$, med notationen ovan.

Notera att det bland stolarna $a_1, a_2, a_3, a_4$ och $a_5$ finns $10$ stycken möjliga par av stolar. Varje par ger en symmetrilinje som motsvaras av att $s = a_i + a_j$ modulo $10$ enligt ovan. Vi ska visa att någon symmetrilinje förekommer för två *olika* par av stolar. Antag motsatsen. Eftersom det finns $10$ par av stolar och $10$ symmetrilinjer, så måste i så fall varje par ge en unik symmetrilinje. Alltså måste alla tal $0, 1, 2, ..., 9$ finnas bland summorna på formen $a_i + a_j$ modulo $10$, och varje tal exakt en gång. Med andra ord blir summan av alla tal på formen $a_i + a_j$ exakt $0 + 1 + 2 + ... + 9 = 45$ modulo $10$. Å andra sidan så kommer den summan också bli $4a_1 + 4a_2 + 4a_3 + 4a_4 + 4a_5$, eftersom varje stol förekommer i $4$ par. Men den summan är jämn, och kan alltså inte bli $45$ modulo $10$, vilket är en motsägelse.

Vi drar slutsatsen att det finns två olika par $a_i, a_j$ samt $a_x, a_y$ som har samma symmetrilinje, alltså sådana att $a_i+a_j \equiv a_x + a_y \equiv s$ modulo $10$. Om $a_i = a_x$ så är även $a_j = a_y$, vilket motsäger att det är olika par. Alltså är $a_i, a_j, a_x, a_y$ alla olika. Så det återstår bara en stol, utöver dessa fyra, kalla den för $a$. Om den sjätte personen nu sätter sig på stol $s - a$ (där $s \equiv a_i + a_j \equiv a_x + a_y$ (mod $10$)), så kommer $a_i, a_j$ paras ihop, $a_x, a_y$ paras ihop och $a, s-a$ paras ihop. Det enda problem som skulle kunna uppstå är om $s - a = a$, men i så fall går symmetrilinjen genom $a$ och den sjätte personen kan sätta sig på stolen mittemot, som också ligger på symmetrilinjen.

Därmed har vi visat att den sjätte personen alltid kan sätta sig så att det finns en symmetrilinje.

<img src="/imgs/veckans_problem_9_sol(a).png" alt="drawing" width="400"/>
<img src="/imgs/veckans_problem_9_sol(b).png" alt="drawing" width="400"/>


Gå tillbaka till uppgiften [här](/blog/2020/08/29/veckans-problem-9).
