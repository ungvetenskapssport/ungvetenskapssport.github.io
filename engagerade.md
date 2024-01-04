---
layout: page
id: engagerade
title: För engagerade
---

*Sidan är under konstruktion.*

Här kommer det finnas information för dig som är engagerad i Ung Vetenskapssport. Planen är att lägga upp länkar till användbart material, som stadgar, mallar, exempel, loggor med mera.

Här är några länkar hittills:
- [Loggor (svg och png)](https://drive.google.com/drive/folders/1a5i9cqt0LPvhXeHS_0XtpJltkz4okbYq?usp=sharing) *(medlemsföreningar, UVS, enskilda former)*
- [Mallar](https://drive.google.com/drive/folders/1vu4aOGeZxKOR3maN3p_OpigPUMD3Lfc9?usp=sharing) *(möten, budget, ...)*
- [Exempelansökan stiftelse för läger](https://docs.google.com/document/d/1alnCEtfmpyWw4kQwl3XT5tfZRlYzJcUmT5jgVqTk8TI/edit?usp=sharing) *(delvis beviljad)*
- [Handbok för läger](https://drive.google.com/drive/folders/1IpKrQGh6He2wKRPClcEic8xZXqc907SK?usp=sharing) *(allt du behöver)*


## Dokument & mallar
Dokument öppnas i Google Drive. Du kan skapa en redigerbar kopia av dokumentet till din egen Google Drive genom att välja "Arkiv" > "Kopia" i menyn. Om du har tillgång till UVS interna drive kan du även nå mallarna direkt när du skapar ett nytt dokument genom att högerklicka, hovra över pilen för "Mer" och välja "From a template".
<!-- Display sample documents! -->
<div class="row">
    {% assign categories = "Mallar,Läger,Styrdokument,Marknadsföring,Övrigt" | split: "," %}

    {% for category in categories %}
        <div class="col-xs-12">
            <h3>{{ category }}</h3>
        </div>

        {% for document in site.data.public-documents %}
            {% if document.category == category %}
                <div class="col-xs-6 col-sm-4 col-md-3 col-lg-3">
                    <div class="thumbnail" style="border: 0px; box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.0);">
                        {% if document.img %}
                            <a href="{{ document.file-url }}">
                                <img class="contact-image-doc" src="{{ document.img }}" alt="{{ document.name }}">
                            </a>
                        {% else %} 
                            <a href="{{ document.file-url }}">
                                <img class="contact-image-doc" src="/imgs/mallar/default-doc.jpg" alt="{{ document.name }}">
                            </a>
                        {% endif %}
                        <div class="caption">
                            <h4><strong>{{ document.name }}</strong></h4>
                            {% if document.example-url %}
                                <p><a href="{{ document.example-url }}" style="outline: none;">Ifyllt exempel</a></p>
                            {% endif %}
                            {% if document.description %}
                                <details>
                                    <summary style="display:list-item; font-size:8pt;">Beskrivning</summary>
                                    <p>{{ document.description }}</p>
                                </details>
                            {% endif %}
                        </div>
                    </div>
                </div>
                <script src="/scripts/redirectOnClick.js"></script>
            {% endif %}
        {% endfor %}

        <div class="clearfix"></div>
    {% endfor %}
</div>



<!-- TODO: 
- Stadgar
  Fler exempel?
  Ekonomi mer publikt?
  Mer grafisk design-grejs
  -->