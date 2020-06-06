---
title: "Giovannelli Lab - Pictures"
layout: piclay
excerpt: "Giovannelli Lab -- Pictures"
permalink: /pictures/
---

# Pictures and Videos

#### Our short documentary from the "Biology Meets Subduction" expedition:
<iframe width="560" height="315" src="https://www.youtube.com/embed/NAf7MvYZfwY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br/>
<br/>

 Jump to the [video section](#videos) or check out the [gallery](#pictures) from the lab and field.
 work around the world.

#### Videos
Here some videos from the lab and the field! More are available on our [youtube channel]() or in our social media feed on [Twitter]() or [Instagram]().

<iframe width="355" height="200" src="https://www.youtube.com/embed/TX0dIqX_UaE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="355" height="200" src="https://www.youtube.com/embed/u9JxQdqtB_s" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

#### Pictures
##### From the Field
(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.piclist %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/field/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>
