---
title: "Teaching"
layout: textlay
excerpt: "Joy Buongiorno -- Teaching"
sitemap: false
permalink: /teaching/
---

# Teaching
{% assign number_printed = 0 %}
{% for publi in site.data.classlist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="container">
{% endif %}

<style>
        .well {
            background-color: rgb(255, 228, 255);
        }
    </style>
    
<div class="col-sm-6 clearfix">
 <div class="well well-lg">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/classpic/{{ publi.image }}" class="img-responsive" width="50%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p>{{ publi.authors }}. {{ publi.year }}. {{ publi.title }}. <em><a href="{{ publi.link.url }}">{{ publi.link.display }}. {{ publi.doi }}</a></em></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>