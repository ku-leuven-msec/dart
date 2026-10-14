---
layout: page
title: Knowledge Dissemination
permalink: /knowledge-dissemination/
---

<div class="hero-section" style="background: linear-gradient(135deg, rgba(0, 150, 210, 0.85) 0%, rgba(0, 120, 180, 0.85) 100%), url('/assets/images/john-adams-1xIN4FMR78A-unsplash.jpg') center/cover; background-attachment: fixed; min-height: 300px;">
  <div style="max-width: 900px;">
    <h1>📄 Knowledge Dissemination</h1>
    <p>Advisory group meetings, hands-on seminars, workshops, presentations and resources from the DART project.</p>
  </div>
</div>

# Advisory Group Meetings

The advisory group meets at least three times a year. It acts as a sounding board and helps validate the guidelines, templates and demonstrators developed in the project. Hands-on seminars and workshops share the results with the advisory group and the wider target group, together with our dissemination partners Agoria, LSEC and the Cyber Security Coalition.

<!--
  HOW TO ADD A MEETING
  - Replace "Date TBA" with the actual date and fill in the agenda.
  - For an event with slides, create a file in _dissemination/ (see README.md) and link to it:
      [Slides and materials]({{ '/knowledge-dissemination/<file-name>/' | relative_url }})
-->

## 1st Advisory Group Meeting – Kickoff (Date TBA)

<div style="margin: 2em 0; padding: 1.5em; background: #f9f9f9; border-radius: 8px; border-left: 4px solid #0096d2;" markdown="1">

**Agenda:**

- Welcome
- Introduction of KU Leuven (DistriNet@Gent) and VUB (Software Languages Lab)
- The DART project: goals, approach and roadmap
- Short introduction of the advisory group members
- Survey and interviews: detection and response needs (WP1)
- Feedback

</div>

## Hands-on Seminar I (Date TBA)

<div style="margin: 2em 0; padding: 1.5em; background: #f9f9f9; border-radius: 8px; border-left: 4px solid #0096d2;" markdown="1">

**Agenda:** *To be announced.*

</div>

## Workshop I (Date TBA)

<div style="margin: 2em 0; padding: 1.5em; background: #f9f9f9; border-radius: 8px; border-left: 4px solid #0096d2;" markdown="1">

**Agenda:** *To be announced.*

</div>

<!--
  Planned in year 2 (uncomment and fill in when scheduled):

## Advisory Group Meeting (Date TBA)
## Hands-on Seminar II (Date TBA)
## Workshop II (Date TBA)
-->

{% if site.dissemination.size > 0 %}
---

## Event Materials

{% for event in site.dissemination reversed %}
<div style="margin: 1.5em 0; padding: 1em; background: #f9f9f9; border-radius: 8px; border-left: 4px solid #0096d2;">
  <strong><a href="{{ event.url | relative_url }}" style="color: #1a1a1a; text-decoration: none;">{{ event.title }}</a></strong><br>
  <em>{{ event.date | date: "%B %d, %Y" }}{% if event.event_type %} · {{ event.event_type }}{% endif %}</em><br>
  <a href="{{ event.url | relative_url }}" style="color: #0078b4; font-size: 0.9em;">View presentations →</a>
</div>
{% endfor %}
{% endif %}

---

## Publications & Media

<!--
  HOW TO ADD AN ITEM: copy the block below into the right category (Articles / Podcasts / Videos)

<div style="margin: 1.5em 0; padding: 1em; background: #f9f9f9; border-radius: 8px; border-left: 4px solid #0096d2;">
  <strong><a href="https://..." target="_blank" style="color: #1a1a1a; text-decoration: none;">Title</a></strong><br>
  <em>Source (e.g. Cybersecurity Bites)</em><br>
  <a href="https://..." target="_blank" style="color: #0078b4; font-size: 0.9em;">Read article →</a>
</div>
-->

<p><em>Articles, podcasts and publications about DART will appear here.</em></p>

---

## Project Results

DART develops the following results to help organisations and their service providers organise detection and response:

<div style="margin: 2em 0; padding: 1.5em; background: #f9f9f9; border-radius: 8px;" markdown="1">
- **Practical security guide *"From Detection to Response"***, with documentation on context-based risk analysis and legal and procedural frameworks (NIS2, GDPR)
- **Open repository of building blocks**: validated detection rules, automation playbooks and reference architectures (tool-agnostic where possible, based on open standards)
- **Demonstrators and a reproducible testbed** with realistic simulation data and attack scenarios, for validation, workshops and hands-on training without risk to production environments
- **Guidelines and templates** for triage, response and incident reporting

Interim results are shared with the advisory group during the project. All results will be **publicly available as open source at the end of the project**. For more information, contact the project team via the <a href="{{ '/consortium/' | relative_url }}">Partners</a> page.
</div>

<!-- TODO: add links to the public repository and published deliverables here once available. -->
