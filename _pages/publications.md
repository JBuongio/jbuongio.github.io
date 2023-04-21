---
title: "Joy Buongiorno - Research & Publications"
layout: gridlay
excerpt: "Joy Buongiorno -- Research & Publications"
sitemap: false
permalink: /publications/
---


# Research
I combine my background in geoscience with a diverse toolkit of novel molecular methods, sequencing analysis, bioinformatics tools, and imaging techniques to delve into the interactions between the biosphere and geosphere that make life thrive in some of the harshest, uninhabitable environments. By combining results from wet-lab and in silico experiments, my work provides a holistic understanding of microbial activity in systems characterized by different geochemical regimes. Clues into how life shaped Earth's environments and vice versa are hypothesized to be written in the DNA of ancient microbial lineages and the rock record. It's my job to uncover these clues, and unlock the secrets to how life can perhaps evolve on other planets. My field sites include the western coast of Svalbard, Antarctic permafrost, hypersaline lakes in the high Andes mountains and hot springs in the Andean Altiplano. 

# Philosophy on SciComm
I am large supporter of science communication - read my blog post about it <a href= 'https://drive.google.com/file/d/1NwHcnNq77RGNdZxySkAKpYdpQVSd_niB/view?usp=sharing'>here</a>. 
I believe in open science and the removal of paywalls between science and the people. I try to be as transparent as possible with my research by uploading all of my code, protocols, and data to GitHub and appropriate public data repositories. 

# Publications
Jump to the bottom of the page to see a [full list of publications](#full-list) and [Preprints](#preprints). A complete list of papers and conference abstracts is also available in my [Google Scholar](https://scholar.google.com/citations?user=3pa76GEAAAAJ&hl=en&oi=ao) profile.

## Highlights

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="50%" style="float: left" />
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


## Full List

{% for publi in site.data.publist %}

  {{ publi.authors }}. <strong>{{ publi.year }}</strong>. {{ publi.title }}. <em><a href="{{ publi.link.url }}">{{ publi.link.display }}. {{ publi.doi }}</a></em>

{% endfor %}

## Preprints
{% for publi in site.data.preprintlist %}

  {{ publi.authors }}. <strong>{{ publi.year }}</strong>. {{ publi.title }}. <em>{{ publi.link.display }}</em>

{% endfor %}
