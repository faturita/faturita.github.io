---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<p style="font-size:1.05em; color:#555; border-left: 4px solid #2a7ae2; padding-left: 1em; margin-bottom: 1.5em;">
Research at the intersection of Brain-Computer Interfaces, Medical Robotics, Neurorehabilitation, and Machine Learning.
</p>

<div style="margin-bottom: 2em;">
  <a href="https://scholar.google.com/citations?user=zN6ty9QAAAAJ&hl=en" target="_blank"
     style="display:inline-block; background:#4285F4; color:white; padding:0.5em 1.2em; border-radius:4px; text-decoration:none; font-weight:bold; margin-right:0.8em;">
    Google Scholar Profile
  </a>
  <a href="https://www.ncbi.nlm.nih.gov/pubmed/?term=Ramele%20R%5BAuthor%5D&cauthor=true&cauthor_uid=31333439" target="_blank"
     style="display:inline-block; background:#336699; color:white; padding:0.5em 1.2em; border-radius:4px; text-decoration:none; font-weight:bold;">
    PubMed
  </a>
</div>

---

## Patents

<div style="border: 1px solid #ddd; border-radius:6px; padding: 1.2em 1.5em; margin-bottom:1.2em; background:#fafafa;">
  <strong>System and Methods for Auditory Stimulation to Affect Sleep</strong><br>
  <span style="color:#555;">Rodrigo Ezequiel Ramele, Cecilia Forcato</span><br>
  <span style="color:#888; font-size:0.9em;">US Patent Application 20250213172A1 &nbsp;·&nbsp; 2025</span><br>
  <p style="margin: 0.6em 0 0.6em 0; font-size:0.95em;">
    A system that monitors brain wave signals to detect slow oscillations during sleep and applies adaptive, personalised auditory stimulation with time delays optimised via a reinforcement signal derived from post-stimulation brain activity.
  </p>
  <a href="https://scholar.google.com/citations?view_op=view_citation&hl=en&user=zN6ty9QAAAAJ&cstart=20&pagesize=80&citation_for_view=zN6ty9QAAAAJ:9ZlFYXVOiuMC" target="_blank" style="font-size:0.9em;">View on Google Scholar &rarr;</a>
</div>

---

## Journal Articles & Conference Papers

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
