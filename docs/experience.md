---
title: "Experience"
layout: single
permalink: /docs/experience/
---

<div class="grid-container">
{% for item in site.data.experience %}
  <div class="grid-item">
    ### {{ item.name }}
    **Sector:** {{ item.sector }}
    
    {{ item.description }}
  </div>
{% endfor %}
</div>