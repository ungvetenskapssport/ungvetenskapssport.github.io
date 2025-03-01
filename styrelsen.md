---
layout: styrelse_layout
id: styrelsen
title: Ung Vetenskapssports styrelse 2023
---

Nedan finner du information om alla våra styrelsemedlemmar. Vill du komma i kontakt med oss kan du skicka ett mail till <a href="mailto:styrelsen@ungvetenskapssport.se">styrelsen@ungvetenskapssport.se</a>
<br>

<div class="buttonInfo" style="max-width: 250px;" onclick="redirectToLink('../assets/Ung Vetenskapssport - Stadgar.pdf')">
    Stadgar <i class="fa fa-file-text"></i>
</div>
<script src="/scripts/redirectOnClick.js"></script>

<!-- SECRET EASTER-EGG -->
<!-- Benjamin's shenanigans... shhh -->
<style>
    body {
        transition: background-color 0.5s ease-in-out;
    }
</style>

<script>
    var clickCount = 0;
    var tripleClickThreshold = 3;
    var active = false;
    var notDelayed = true;

    function handleTripleClick(event, link) {
        clickCount++;

        if (active && notDelayed) {
            // Execute your redirection logic or any other action
            window.location.href = link;
            
            // Reset click count for future clicks
            clickCount = 0;
        }

        if (clickCount === tripleClickThreshold) {
            // Change background color to gray after 3 clicks & activate redirection if one more click is made
            document.body.style.backgroundColor = 'gray';
            active = true;
            notDelayed = false; // requires a short pause before allowing another click

            // set a 0.5 s delay before allowing another click
            setTimeout(function () {
                notDelayed = true;  // then allow it again
            }, 500);


            // Reset background color & deactivate after a delay (e.g., 3 seconds)
            setTimeout(function () {
                document.body.style.backgroundColor = '';
                clickCount = 0; // and reset the click count
                active = false;
            }, 3000);

        }

        // Reset click count if the time between clicks is too long (e.g., 2 second)
        setTimeout(function () {
            clickCount = 0;
        }, 2000);
    }
</script>
<!-- END OF EASTER EGG -->


<!-- This generates the boxes -->
<div class="row">
    {% for member in site.data.members %} {% if member.current == true %} {% if member.year == 2025 %}

    <div class="col-xs-6 col-sm-4 col-md-3 col-lg-3" style="display: flex; flex-direction: column;">
        <div class="thumbnail" {% if member.name == "Benjamin Verbeek" %} onclick="handleTripleClick(event, '/mer/engagerade')" {% endif %} >
            {% if member.img %}
                {% if member.img2 %}
                    <div class="contact-image-hover"
                    style="background-image: url({{ member.img2 }})"
                    onmouseover="this.style.backgroundImage='url({{ member.img }})'" 
                    onmouseout="this.style.backgroundImage='url({{ member.img2 }})'">
                    </div>
                {% else %}
                    <img class="contact-image" src="{{ member.img }}" alt="{{ member.name }}">
                {% endif %}
                
            {% endif %}
            <div class="caption">
                <h4>{{ member.name }}</h4>
                <p> {{ member.role }}</p>
                {% if member.city %}
                <p> {{member.city}} </p>
                {% endif %}
                <h2>
                {% if member.mail %}
                <a href="mailto:{{ member.mail }}"><i class="fa fa-envelope-square"></i></a>
                {% endif %}
                {% if member.github %}
                <a href="https://github.com/{{ member.github }}" target="_blank"><i class="fa fa-github-square"></i></a>
                {% endif %}
                {% if member.website %}
                <a href="https://{{ member.website }}" target="_blank"><i class="fa fa-home"></i></a>
                {% endif %}
                </h2>
            </div>
        </div>
    </div>
    {% assign mod4 = forloop.index | modulo:4 %}
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
    {% endif %}

    {% endif %} {% endif %} {% endfor %}
</div>


## Tidigare styrelser
<!-- Ändra 2023 nedan i framtiden. -->
{% for year in (2015..2024) reversed %}
<details>
  <summary style="font-size: larger;">{{ year }}</summary>
  <ul>
    {% for member in site.data.members %}
      {% if member.year == year %}
        <li><b>{{ member.name }}</b> - {{ member.role }}</li>
      {% endif %}
    {% endfor %}
  </ul>
</details>
{% endfor %}

