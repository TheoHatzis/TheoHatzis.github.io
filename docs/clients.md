---
title: "Clients"
layout: single
permalink: /docs/clients/
---

The following organizations represent the landscape of my recent engagements:

{% for client in site.data.clients %}
  ### {{ client.name }}
  **Sector:** {{ client.sector }}
  
  {{ client.description }}

  ---
{% endfor %}