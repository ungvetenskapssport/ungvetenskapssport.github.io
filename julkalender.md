---
# meta
layout: julkalender
id: julkalender
header-img: ../imgs/fa-lager/header.png # recommended dimensions: 2732x668px but other aspect ratios should also be fine.
#header-size: 100px
# content
title: UVS Julkalender    # used on image
title-size: 4.8vw,65px       # Adjust to make text wrapping ok. Run through min(), e.g.: min(7vw,30px)
title-color: antiquewhite    # color of title, see choice here: https://developer.mozilla.org/en-US/docs/Web/CSS/named-color 
subtitle: Här kommer vi varje dag vid 8.00 lägga upp ett problem från en av våra åtta medlemsföreningar. På juldagen kommer en överraskning!
subtitle-size: 2.2vw, 26px   # Adjust to make text wrapping ok. Run through min(), e.g.: min(7vw,30px)
subtitle-color: antiquewhite # color of subtitle
---

##### Hej och välkomna till UVS julkalender! Här kommer vi varje dag vid 10.00 lägga upp ett problem från en av våra åtta medlemsföreningar. På juldagen kommer en överraskning! 
<br>
<br>


<head>
    <title>Julkalender</title>
    <style>
        .calendar {
            display: grid;
            grid-template-columns: repeat(6, 150px);
            grid-template-rows: repeat(4, 150px); /* Update grid-template-rows to 1fr */
            gap: 30px;
        }
        .calendar .square {
            background-color: #f2f2f2;
            border: 1px solid #ccc;
            padding: 20px;
            text-align: center;
            height: 100%; /* Update height to 100% */
            border-radius: 10px; /* Add rounded corners */
            display: flex;
            justify-content: center;
            align-items: center;
            font-weight: bold;
            font-size: 24px;
        }

        .thumbnail {
            position: relative;
        }

        .image-text {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: black; /* Set the text color */
            font-size: 50px; /* Set the font size */
            font-weight: bold; /* Set the font weight */
            text-align: center; /* Align the text to the center */
        }
        .custom-container {
        position: relative;
        width: 100vw; /* Full width of the viewport */
        height: 0;
        padding-bottom: 75vh; /* 75% of the viewport height */

        background: url('your-image.jpg') center/cover no-repeat;
        clip-path: polygon(0 0, 100% 0, 100% 100%, 0% 100%);
        }

        .custom-image {
        width: 100%;
        height: 100%;
        object-fit: cover;
        position: absolute;
        top: 0;
        left: 0;
        clip-path: polygon(0 0, 100% 0, 100% 100%, 0% 100%);
        }
    </style>
</head>


<body>

<div class="row">
    {% for lucka in site.data.julkalender %}

    <div class="col-xs-4 col-sm-3 col-md-2 col-lg-2">
        <div class="thumbnail" style="padding: 0px;">


            {% if lucka.available and lucka.forening %}
            <img class="contact-image-no-border" src="../imgs/julkalender_2023/{{ lucka.forening }}.png" alt="{{ lucka.date }}" style="padding: 0px;" onclick="redirectToLink('{{ lucka.url }}')">
            {% else %}
            <img class="contact-image-no-border" src="../imgs/default-eventicon.png" alt="{{ lucka.date }}" style="padding: 0px;" onclick="redirectToLink('{{ lucka.url }}')">
            {% endif %} 

            <div class="image-text">
            {{lucka.date}}
            </div>

<!-- 
            <div class="caption" style="margin-bottom: -15px">
                {% if member.form %}
                <script src="/scripts/redirectOnClick.js"></script>
                <div class="buttonMedlem" onclick="redirectToLink('{{ member.form }}')">
                Bli medlem <i class="fa fa-sign-in"></i>
                </div>
                {% endif %}

                {% if member.sampleproblem %}
                     <p><a href="{{ member.sampleproblem }}" >Exempelproblem</a></p> 
                    <div class="buttonInfo" onclick="redirectToLink('{{ member.sampleproblem }}')">
                Exempel<wbr>problem <i class="fa fa-puzzle-piece"></i>
                </div>
                {% endif %}

                {% if member.info_ebas %}
                <div class="buttonInfo" onclick="redirectToLink('{{ member.info_ebas }}')">
                Mer info <i class="fa fa-info-circle"></i>
                </div>
                {% endif %}

                <details>
                    <summary style="display:list-item; font-size:8pt;">Om {{ member.name }}</summary>
                    <p>{{ member.description }}</p>
                </details>
                
                {% if member.city %}
                <p> {{member.city}} </p>
                {% endif %}
                <h3>
                {% if member.github %}
                <a href="https://github.com/{{ member.github }}" target="_blank"><i class="fa fa-github-square"></i></a>
                {% endif %}
                {% if member.website %}
                <a href="https://{{ member.website }}" target="_blank"><i class="fa fa-home"></i></a>
                {% endif %}
                </h3> 
            </div>
            -->

        </div> 
        <script src="/scripts/redirectOnClick.js"></script>
        <!-- snö? -->

    </div>
    <!-- {% assign mod4 = forloop.index | modulo:4 %}
    {% assign mod3 = forloop.index | modulo:3 %}
    {% assign mod2 = forloop.index | modulo:2 %}
    {% if mod2 == 0 %}
    <div class="clearfix visible-xs-block"></div>
    {% endif %}
    {% if mod3 == 0 %}
    <div class="clearfix visible-sm-block"></div>
    {% endif %}
    {% if mod4 == 0 %}
    <div class="clearfix visible-md-block"></div>
    <div class="clearfix visible-lg-block"></div>
    {% endif %} -->

    {% endfor %}
</div>

</body>

<!-- 
<body>
    <div class="calendar">
        {% for lucka in site.data.julkalender %}

        <div class="square">1</div>

        
        {% if lucka.available == true %}
        <div class="square" onclick="redirectToLink('{{ lucka.url }}')">{{ lucka.day }}</div>
        {% endif %}

        {% if lucka.available == false %}
        <div class="square" onclick="redirectToLink('/unavailable')"></div>
        {% endif %}
        

        {% endfor %}
</body>


<body>
    <div class="calendar">
        <div class="square">19</div>
        <div class="square">2</div> 
        <div class="square">14</div>
        <div class="square">6</div>
        <div class="square">23</div>
        <div class="square">1</div>
        <div class="square">12</div>
        <div class="square">7</div>
        <div class="square">10</div>
        <div class="square">3</div>
        <div class="square">18</div>
        <div class="square">5</div>
        <div class="square">16</div>
        <div class="square">24</div>
        <div class="square">9</div>
        <div class="square">11</div>
        <div class="square">4</div>
        <div class="square">21</div>
        <div class="square">8</div>
        <div class="square">15</div>
        <div class="square">13</div>
        <div class="square">20</div>
        <div class="square">17</div>
        <div class="square">22</div>
    </div>
</body>
 -->
