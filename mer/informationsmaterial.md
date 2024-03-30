---
layout: page
id: informationsmaterial
title: Informationsmaterial
---
Vill du sprida information om Ung Vetenskapssport? Det välkomnar vi! Här hittar du material som du kan använda för att sprida information om oss.

### Posters
Nedan finns alla posters samlade i en PDF-fil så att du enkelt kan skriva ut en (eller flera) av varje.
<div class="buttonMedlem" style="max-width: 300px;" onclick="redirectToLink('/affisch/pdfs/alla_posters.pdf')">
    En av varje UVS-affisch <i class="fa fa-download"></i>
</div>

#### Allmän UVS-poster
Här hittar du en allmän poster som passar bra att hänga upp på skolan eller vid besök.
<div class="buttonMedlem" style="max-width: 300px;" onclick="redirectToLink('/affisch/pdfs/uvs-poster-vit-pussel.pdf')">
    Allmän UVS-affisch <i class="fa fa-download"></i>
</div>
<script src="/scripts/redirectOnClick.js"></script>

#### Exempelproblem
Här hittar du posters med exempelproblem per ämne:
<div class="buttonMedlem" style="max-width: 300px;" onclick="redirectToLink('/affisch/pdfs/alla_exempelproblem.pdf')">
    Alla problem <i class="fa fa-download"></i>
</div>

Respektive ämne:
{% for member in site.data.medlemsforeningar %}
{% if member.sampleproblem_poster %}

<div class="buttonInfo" style="max-width: 300px;" onclick="redirectToLink('{{ member.sampleproblem_poster }}')">
    {{ member.name }} <i class="fa fa-download"></i>
</div>
<!-- <br> -->

{% endif %}
{% endfor %}


### Presentation
<div class="buttonMedlem" style="max-width: 300px;" onclick="redirectToLink('/assets/Ung Vetenskapssport - allmän.pptx')">
    Allmän presentation (89 MB) <i class="fa fa-download"></i>
</div>