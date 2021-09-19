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
<html>
<head>
<style>
div.gallery {
  margin: 5px;
  border: 1px solid #ccc;
  float: left;
  width: 400px;
}

div.gallery:hover {
  border: 1px solid #777;
}

div.gallery img {
  width: 100%;
  height: auto;
}

div.desc {
  padding: 15px;
  text-align: center;
}
</style>
</head>
<body>

<div class="gallery">
  <a target="_blank" href="img_5terre.jpg">
    <img src="{{ site.url }}{{ site.baseurl }}images/classpic/dna.jpeg" alt="BIO349" width="600" height="400">
  </a>
  <div class="desc"><b>BIO349: Bioinformatics</b><p> The advent of next-generation sequencing technology has revolutionized microbiology, enabling transformative breakthroughs in fields ranging from agriculture to conservation to medicine. New methods enable full genome sequencing of microorganisms, and through varied ‘omic techniques, scientists can analyze of millions of short sequences that comprise “big data”. In this course, students will learn about the computational algorithms that underly bioinformatic tools. In the computer-based lab component, students will gain hands-on experience with both web-based and Unix command line bioinformatic tools for sequence searching and alignment, assembly, read mapping, gene calling, and gene annotation. </div></div>
  
 <div class="gallery">
  <a target="_blank">
    <img src="{{ site.url }}{{ site.baseurl }}images/classpic/Plate.jpg" alt="BIO112" width="600" height="400">
  </a>
  <div class="desc"><b>BIO112: Principles of Microbiology </b><p>
  </p>An overview of microbiology, with particular emphasis on the role of microbes in human health and disease. Core concepts of evolution, cell structure and function, metabolism, genetics, microbial systems, and the impact of microorganisms on humans will be covered, and competencies in the application of the process of science, and use of quantitative reasoning will be developed. After students master sterile technique and safe laboratory practices, the laboratory portion of the course will focus on the development of microscopy, culture, and bacterial identification techniques.  

