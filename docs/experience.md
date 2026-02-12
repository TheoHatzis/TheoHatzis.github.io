---
title: "Experience"
layout: single
permalink: /docs/experience/
---

{% for item in site.data.experience %}
  ### {{ item.title }}
  {{ item.description }}
{% endfor %}