---
title: "Joy Buongiorno - Laguna Negra"
layout: piclay
excerpt: "Joy Buongiorno -- Pictures"
permalink: /LN_pictures/
---

# Laguna Negra

#### Photos from the field and under the petrographic microscope:

{% for piclist in site.data.piclist %}
- [{{ piclist.description }}]({{ piclist.title }})
{% endfor %}