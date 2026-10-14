---
layout: default
title: Home
---

<!-- TODO: replace the hero background image with a DART-specific image (see IMAGES_GUIDE.md) -->
<div class="hero-section" style="background: linear-gradient(135deg, rgba(0, 150, 210, 0.85) 0%, rgba(0, 120, 180, 0.85) 100%), url('/assets/images/john-adams-1xIN4FMR78A-unsplash.jpg') center/cover; background-attachment: fixed;">
  <div style="max-width: 900px;">
    <h1>🎯 DART</h1>
    <h2 style="color: white; border: none; padding: 0; margin: 0;">Intelligent Detection, Response and Analysis of Security Events</h2>
    <p>Helping SMEs, non-profits and their service providers build feasible, NIS2-aligned detection and incident response capabilities. A TETRA project funded by VLAIO.</p>
    <p><a href="#about" class="btn" style="margin-top: 20px;">Learn more</a></p>
  </div>
</div>

<div class="capabilities-section">
  <div class="wrapper">
    <h2>Focus areas</h2>
    <div class="capabilities-grid">
      <div class="capability-card">
        <div class="icon">⚖️</div>
        <h3>Risk &amp; compliance</h3>
        <p>Translating NIS2, GDPR and frameworks such as NIST CSF 2.0 and CyFun® into concrete, proportionate technical requirements.</p>
      </div>
      <div class="capability-card">
        <div class="icon">🔍</div>
        <h3>Detection</h3>
        <p>Baseline detection, threat intelligence and detection-as-code templates for a reproducible security monitoring setup.</p>
      </div>
      <div class="capability-card">
        <div class="icon">🚨</div>
        <h3>Triage &amp; response</h3>
        <p>Decision trees, playbooks-as-code and AI assistance to reduce alert fatigue and shorten the time from detection to response.</p>
      </div>
      <div class="capability-card">
        <div class="icon">📋</div>
        <h3>Post-incident</h3>
        <p>Templates for legal incident reporting and structured post-incident analysis that feeds lessons learned back into detection.</p>
      </div>
    </div>
  </div>
</div>

<div class="three-levels-section">
  <div class="wrapper">
    <h2>Across the incident lifecycle</h2>
    <div class="levels-container">
      <div class="level-card">
        <div class="level-number">1</div>
        <h3>Pre-incident</h3>
        <p>Detect: prioritised data sources, rule-based detection and automated configuration and rollout of security tooling.</p>
      </div>
      <div class="level-card">
        <div class="level-number">2</div>
        <h3>At-incident</h3>
        <p>Respond: fast, proportionate triage, containment and response, whether handled in-house or outsourced.</p>
      </div>
      <div class="level-card">
        <div class="level-number">3</div>
        <h3>Post-incident</h3>
        <p>Analyse: correct and timely reporting to authorities (CCB/GBA) and structural lessons learned.</p>
      </div>
    </div>
  </div>
</div>


<a id="about"></a>
# About DART

DART closes the gap between what regulation expects of detection and incident response and what Flemish SMEs and non-profit organisations can realistically do. Through practice-oriented research, the project delivers context-aware guidelines, methodologies and reference architectures that help these organisations and their service providers organise detection and response in a feasible way.

## The challenge

With the NIS2 directive, European organisations, including many Flemish SMEs, face growing pressure to strengthen their cyber resilience. Many have taken measures to *identify* and *protect*, but detection and incident response remain the least mature parts of their security approach.

At the same time, ICT environments keep getting more complex. Cloud, network, IoT and industrial (OT) environments generate large volumes of security events. That data makes fast detection possible, but most SMEs and non-profits lack the expertise and resources to use it. Available security solutions are often built for large enterprises and don't match the cost, complexity or skills of smaller organisations. Security teams struggle with *alert fatigue*, while *dwell time*, the time an attacker stays unnoticed, remains too high.

## Our approach

The building blocks already exist. What is missing is their translation to the SME context. DART focuses on lowering the operational burden through context-specific configuration and automation, rather than adding more and larger tools. Concretely, the project explores:

- **Detection-as-code and configuration-as-code** for reproducible, verifiable security setups
- **Playbooks-as-code** for automated containment of common, low-risk incidents
- **Generative AI and AI agents** as a "copilot" that turns natural-language risk descriptions into detection rules, and that supports triage and filtering of false positives
- **Tool-agnostic, open standards** wherever possible, so results don't depend on one vendor

## Target groups

The project addresses three sub-target groups:

- **Cybersecurity and IT service providers and integrators**: need scalable, modular methods to offer detection and response services cost-effectively to many smaller clients
- **Organisations with in-house or hybrid security operations**: monitor their environment but lack the resources for a 24/7 SOC or complex enterprise tooling (SIEM, SOAR)
- **Organisations in the awareness phase**: have not yet implemented detection and response, and are reached through targeted knowledge dissemination

---

## Expected results

1. **A practical framework** for interpreting and prioritising cyber risks and legal obligations around monitoring, incident handling and reporting
2. **Practical guidelines** for setting up security operations in line with risk profile, maturity and available resources, without compromising compliance
3. **Standardised workflows and playbook templates** for triage and response, usable without a permanent SOC or specialised security experts
4. **Reference architectures** for detection and alert processing, focused on filtering, correlation and contextual enrichment of alerts
5. **A practical security guide**, *"From Detection to Response"*, bundling all insights, guidelines and tools

All results are validated in representative cases together with members of the advisory group, and are made publicly available as open source at the end of the project.

---

## Partners

<p>This TETRA project is carried out by:</p>
<br>
- **KU Leuven – DistriNet, Campus Gent** (project lead): secure distributed systems, IoT, network security, cybersecurity standards and AI for security
- **Vrije Universiteit Brussel – Software Languages Lab (SOFT)**: event-driven architectures, rule-based systems and declarative programming

The project is funded by **VLAIO** (Flanders Innovation & Entrepreneurship) within the TETRA programme, using earmarked funds of the Flemish Cybersecurity research programme.

---

<div style="text-align: center; margin: 3em 0;">
  <a href="{{ '/project/' | relative_url }}" class="btn">Explore the work plan</a>
  <a href="{{ '/knowledge-dissemination/' | relative_url }}" class="btn">Events &amp; results</a>
  <a href="{{ '/consortium/' | relative_url }}" class="btn">Meet the partners</a>
</div>
