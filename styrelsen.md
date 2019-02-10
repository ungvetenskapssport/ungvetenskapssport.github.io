---
layout: page
title: Styrelsen
---

# Ung Vetenskapssports styrelse 2019

<br>

<div class="row">
    {% for member in site.data.members %} {% if member.current == true %}

    <div class="col-xs-4 col-md-3">
        <div class="thumbnail">
            {% if member.img %}
            <img class="contact-image" src="{{ member.img }}" alt="{{ member.name }}">
            {% endif %}
            <div class="caption">
                <h5>{{ member.name }}</h5>
                <p> {{ member.role }}</p>
            </div>
        </div>
    </div>
        {% assign mod = forloop.index | modulo:4 %}
        {% if mod == 2 %} 
    <div class="clearfix visible-xs-block"></div>
    <div class="clearfix visible-sm-block"></div>
        {% endif %}
        {% if mod == 0 %} 
    <div class="clearfix visible-xs-block"></div>
    <div class="clearfix visible-sm-block"></div>
    <div class="clearfix visible-md-block"></div>
    <div class="clearfix visible-lg-block"></div>
        {% endif %}

    {% endif %}{% endfor %}
</div>
