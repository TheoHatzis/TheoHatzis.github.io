---
title: "Experience"
layout: single
permalink: /docs/experience/
---

<div class="grid-container">
{% for client in site.data.experience %}
  <div class="grid-item">
    ### {{ client.name }}
    **Experience:** {{ client.sector }}
    
    {{ client.description }}
  </div>
{% endfor %}
</div>