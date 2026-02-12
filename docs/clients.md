---
title: "Clients"
layout: single
permalink: /docs/clients/
---

<div class="grid-container">
{% for client in site.data.clients %}
  <div class="grid-item">
    ### {{ client.name }}
    **Sector:** {{ client.sector }}
    
    {{ client.description }}
  </div>
{% endfor %}
</div>