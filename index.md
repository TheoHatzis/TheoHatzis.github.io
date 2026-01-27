
---
layout: single
author_profile: true
title: "Goat Mountain Semiconductor Solutions"
excerpt: "The Ibex: An overseer on the heights, watching the clever Fuchs at the coalface. <br/><br/>"
header:
  image: /assets/images/bg_wide.png
  teaser: /assets/images/bg_wide.png
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

> **Current Status:** {{ site.availability }}  
> **Location:** {{ site.last_sighting }}

## Theo Hatzis
### Senior Electronics Architect & Semiconductor Validation Specialist  
_“Der Fuchs” — the fox who finds the flaw no one else sees_

## **About Me**
I focus on hardware engineering, specialising in semiconductor validation, mixed-signal power systems, and system-level triage. Over two decades, I have built my career across the Munich semiconductor ecosystem, Denmark, and the Thames Valley 'Silicon Hub' in the UK.

During my time at Ericsson in Nürnberg, I earned the nickname **“Der Fuchs”** — *the fox who finds the flaw no one else sees*. This reflects a diagnostic intuition and creative problem-solving, and the delivery of elegant solutions and applications under hard real-time RMS pressures.

---

## **Engineering Applications**
* **Post‑Silicon Validation:** PMIC/PMU, PVT corners, and silicon‑to‑model correlation.
* **Mixed‑Signal & Power:** Buck/Boost, GaN/SiC gate drivers, and multiphase converters.
* **Automation & Data:** Python-driven analysis (PyVISA, Pandas, NumPy, Pytest).
* **Mentorship:** Guiding students and junior engineers through the complexities of the semiconductor landscape.


## Interests & Capabilities

---

### **High-Altitude Architectural Oversight**
* **Silicon Triage:** Specialising in the "Der Fuchs" methodology—identifying elusive system-level stressors and PVT corner exceptions that automated V&V often misses.
* **Measurement-Driven Engineering:** Bridging the gap between physical-layer behaviour and silicon reliability, from sub-picoampere sensor interfaces to high-speed digital integrity.

### **Specialised Domain Expertise**
* **Power & Energy Systems:** Advanced validation of GaN/SiC topologies, multiphase DCDC converters, and BMS state-of-health (SoH) characterisation using Electrochemical Impedance Spectroscopy (EIS).
* **Safety-Critical Systems:** Navigating complex regulatory landscapes including ISO 26262 (Automotive), ISO 13485 (Medical), and TRG 1068 (UK Infrastructure).
* **Multidisciplinary Diagnostic Intuition:** Leveraging a foundation in Physical Chemistry and Spectroscopy to resolve root-cause failures in MedTech, Photonics (SPAD/dToF), and Scientific Instrumentation.


[Click for More Details]({{ 'docs/myfile3/' | relative_url }}){: .btn .btn--info .btn--large}


## ⏳ Professional Expertise: Semiconductor Hub

<div class="experience-list">
  {% for job in site.data.experience %}
  <details class="exp-card" style="border-bottom: 1px solid #eee; margin-bottom: 1.5rem; padding-bottom: 1rem;">
    <summary style="cursor: pointer; font-weight: bold; list-style: none; display: flex; align-items: center; font-size: 1.15em; outline: none;">
      <span style="color: #d35400; margin-right: 12px; transition: transform 0.2s;" class="icon-toggle">▸</span> 
      {{ job.duration }} | {{ job.company }} — {{ job.role }}
    </summary>
    
    <div style="padding: 1rem 2rem; color: #444; line-height: 1.6; background: rgba(0,0,0,0.02); border-radius: 4px; margin-top: 10px;">
      <p style="margin-top: 0; margin-bottom: 0.5rem;"><strong>Location:</strong> {{ job.location }}</p>
      <p style="margin-bottom: 0;">{{ job.description }}</p>
    </div>
  </details>
  {% endfor %}
</div>

<style>
  .experience-list summary::-webkit-details-marker { display: none; }
  .experience-list summary { list-style: none; }
  .experience-list summary:hover { color: #d35400; }
  .exp-card[open] summary { color: #d35400; }
  .exp-card[open] .icon-toggle { transform: rotate(90deg); display: inline-block; }
</style>
