---
layout: page
id: styrelsen
title: Ung Vetenskapssports styrelse 2021
---


Nedan finner du ansikten på alla styrelsemedlemmar. Vill du kontakta komma i kontakt med oss kan du skicka ett mail till <a href="mailto:styrelsen@ungvetenskapssport.se">styrelsen@ungvetenskapssport.se</a> 
<br>

<div class="row">
    {% for member in site.data.members %} {% if member.current == true %}

    <div class="col-xs-5 col-sm-4 col-md-3 col-lg-3">
        <div class="thumbnail">
            {% if member.img %}
            <img class="contact-image" src="{{ member.img }}" alt="{{ member.name }}">
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

    {% endif %}{% endfor %}
</div>
