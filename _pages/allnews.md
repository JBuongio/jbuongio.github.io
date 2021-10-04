---
title: "News"
layout: textlay
excerpt: "Joy Buongiorno"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
  <p>{{ article.date }} <br>
      {{ article.headline }}
  </p>
{% endfor %}

<a class="twitter-timeline" href="https://twitter.com/DrJoyBuongiorno?ref_src=twsrc%5Etfw">Tweets by DrJoyBuongiorno</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>