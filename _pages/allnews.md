---
title: "News"
layout: textlay
excerpt: "Giovannelli Lab at University of Naples 'Federico II'"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
  <p>{{ article.date }} <br>
      {{ article.headline }}
  </p>
{% endfor %}
