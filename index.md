---
layout: single
author_profile: true
title: "Goat Mountain Semiconductor Solutions"
excerpt: "The Ibex: An overseer on the heights, watching the clever Fuchs at the coalface. <br/><br/>"
header:
  image: /assets/images/bg.png
  teaser: /assets/images/bg.png
  overlay_filter: 0.1
  caption: "The High Perch: Architectural oversight meets technical intuition."
  actions:
    - label: "Technical Matrix"
      url: "/myfile3/"
    - label: "Download CV"
      url: "/THEO%20HATZIS%20CV.pdf"
---


{: .notice--info}
**The Summit View:** From the high-altitude perspective of an Architect, the goal is not just to see the circuit, but to understand the entire ecosystem. As the Ibex watches the valley, I oversee the intersection of hardware, software, and power to ensure architectural grace.

<div style="float: right; margin-left: 20px; text-align: center;">
  <img src="/assets/images/Gemini_Generated_Image_mofdbemofdbemofd.png" alt="The Goatherd" style="width: 250px; border-radius: 5px;">
  <p style="font-style: italic; font-size: 0.8em; color: #666;">The Seasoned Presence</p>
</div>

> **Current Status:** {{ site.availability }}  
> **Location:** {{ site.last_sighting }}




[Click for More Details]({{ 'docs/myfile3/' | relative_url }}){: .btn .btn--info .btn--large}


## ⏳ Professional Expertise: Semiconductor Hub

<div class="trinity-timeline">
  {% for era_group in site.data.experience %}
  <details class="era-layer" style="margin-bottom: 25px; border-left: 6px solid #d35400; padding-left: 15px;">
    <summary style="font-weight: bold; font-size: 1.5em; cursor: pointer; color: #1a1a1a;">
      {{ era_group.era }}
    </summary>

    {% for job in era_group.jobs %}
    <details class="job-layer" style="margin: 15px 0 15px 30px; border-left: 2px solid #aaa; padding-left: 15px;">
      <summary style="cursor: pointer; font-size: 1.1em; font-weight: 500;">
        {{ job.duration }} | <strong>{{ job.company }}</strong> — {{ job.role }}
      </summary>
      
      <div style="padding: 10px 0;">
        <p style="margin-bottom: 10px;">{{ job.description }}</p>

        <details class="leaf-layer">
          <summary style="cursor: pointer; color: #d35400; font-size: 0.85em; font-weight: bold;">
            ▼ Reveal Technical Coalface (The Fuchs)
          </summary>
          <div style="margin-top: 10px; display: flex; flex-wrap: wrap; gap: 8px;">
            {% for leaf in job.leaves %}
            <span style="background: #efefef; border: 1px solid #ccc; padding: 2px 10px; border-radius: 4px; font-size: 0.8em; font-family: monospace;">
              {{ leaf }}
            </span>
            {% endfor %}
          </div>
        </details>
      </div>
    </details>
    {% endfor %}

  </details>
  {% endfor %}
</div>

---

🌍
Endnote
The moniker “Der Fuchs” originates from my time contracting at Ericsson (later as ST Ericsson) located in Franconia
Germany. It reflects the German idiom **“Der Fuchs findet den Fehler, den keiner sieht” — the fox finds the
flaw no one else sees [our clever fox]. — a recognition of my diagnostic intuition and ability to resolve elusive
system-level issues. I remained with the programme for four years — unusually long for a contractor — reflecting the trust
and reliance the team placed in my pivotal designs and diagnostic work.