---
layout: page
title: Project
permalink: /project/
---

<div class="hero-section" style="background: linear-gradient(135deg, rgba(0, 150, 210, 0.85) 0%, rgba(0, 120, 180, 0.85) 100%), url('/assets/images/john-adams-1xIN4FMR78A-unsplash.jpg') center/cover; background-attachment: fixed; min-height: 300px;">
  <div style="max-width: 900px;">
    <h1>🗺️ Project</h1>
    <p>Two yearly cycles, seven work packages: from needs analysis to validated, publicly available results.</p>
  </div>
</div>

# Work plan

DART runs for two years and is organised as two cycles of one year each, so that new technologies, attack techniques and regulatory changes can be taken into account along the way. Development starts from a needs analysis and technology scan (WP1) and a risk and compliance framework (WP2). Reusable knowledge and technical artefacts are then developed for each phase of the incident lifecycle (WP3–WP5), integrated and validated in representative test environments (WP6), and disseminated to the target group (WP7).

<div class="wp-diagram">
  <div class="wp-row"><div class="wp-box">WP1 · Needs analysis &amp; technology scan</div></div>
  <div class="wp-arrow">▼</div>
  <div class="wp-row"><div class="wp-box">WP2 · Risk &amp; compliance framework</div></div>
  <div class="wp-row wp-three">
    <div class="wp-box">WP3 · Pre-incident<br><small>Detection, configuration &amp; rollout</small></div>
    <div class="wp-box">WP4 · At-incident<br><small>Triage, containment &amp; response</small></div>
    <div class="wp-box">WP5 · Post-incident<br><small>Audit &amp; reporting</small></div>
  </div>
  <div class="wp-arrow">▼</div>
  <div class="wp-row"><div class="wp-box">WP6 · Integration &amp; validation</div></div>
  <div class="wp-arrow">▼</div>
  <div class="wp-row"><div class="wp-box">WP7 · Management &amp; dissemination</div></div>
</div>

---

## WP1 – Needs analysis and technology scan
*Lead: KU Leuven DistriNet@Gent*

Maps the current state of cybersecurity in the target groups, the technical constraints and the available technology, as the basis for later work packages.

- **Analysis of the SME context**: survey and interviews with the advisory group and a broader group of Flemish SMEs, based on NIST CSF 2.0 and CyFun® 2025, to map detection capabilities, resources and barriers to adoption
- **Technology scan and service offering analysis**: evaluates open-source and accessible commercial tools, and checks whether existing service formulas (SOC, MDR) fit the budget and operational context of SMEs
- **Selection of representative cases**: at least two cases (e.g. an administrative SME environment, or a production environment with IT/OT convergence) that guide validation in WP6

## WP2 – Risk and compliance framework
*Lead: KU Leuven DistriNet@Gent*

Helps SMEs determine and justify appropriate security measures by linking abstract compliance requirements to concrete operational and technical settings.

- **Identification and prioritisation**: a simplified risk analysis method for identifying assets and threats without deep theoretical knowledge
- **Inventory of legislation, standards and guidelines**: NIS2, GDPR and related standards, focusing on monitoring, detection, response and reporting obligations (e.g. notification duties, log retention)
- **Translation to operational requirements**: a matrix linking obligations to technical requirements, plus guidelines for the safe use of GenAI in security operations

## WP3 – Pre-incident: detection, configuration and rollout
*Lead: VUB SOFT*

Turns risk and compliance insights into feasible detection, configuration and automation practices, with attention to reuse and scalability.

- **Baseline detection and threat intelligence**: a minimal but effective standard for logging and detection, and procedures to filter external threat intelligence (e.g. CERT advisories) to the SME context
- **Automated configuration and rollout (X-as-Code)**: declarative templates (e.g. Ansible, YAML) for reproducible rollout of the security stack, applying configuration-, policy- and detection-as-code principles
- **GenAI support**: prompts and practices for drafting, interpreting and reviewing detection rules and configurations

## WP4 – At-incident: triage, containment and response
*Lead: VUB SOFT*

Develops feasible methods to minimise the time between detection and response, for both in-house and outsourced handling.

- **Triage and false positives/negatives**: decision trees for the initial assessment of alerts, plus a feedback loop that turns false positives and negatives into improved detection rules
- **Playbooks-as-Code**: automated containment and response scripts (SOAR) for common, low-risk incidents, such as isolating a host or blocking a user account
- **AI-assisted incident handling and analysis**: GenAI for interpreting, summarising and correlating incident information, and for supporting root cause analysis and forensic reporting

## WP5 – Post-incident: audit and reporting
*Lead: KU Leuven DistriNet@Gent*

Streamlines correct, timely and proportionate post-incident handling.

- **Documentation and legal reporting**: practical guidelines and templates for incident reporting that fit an SME context and meet the requirements of the supervisory authorities (CCB/GBA)
- **Post-incident analysis**: a structured method that feeds incidents back into risk assessment (WP2), detection and configuration (WP3) and response (WP4)

## WP6 – Integration and validation
*Lead: KU Leuven DistriNet@Gent*

Brings the results together and validates them from the perspective of SMEs (in-house, outsourced or hybrid) and of service providers serving many SMEs.

- **Testbed**: a test environment that simulates the WP1 cases and implements the artefacts from WP2–WP5
- **Case development**: technical demonstrators built together with the advisory group, accounting for differences in sector, maturity and operational context
- **Validation**: simulated attack scenarios measuring *Time-to-Detect* and *Time-to-Respond*, and evaluating effectiveness, efficiency, compliance and usability of the documentation

## WP7 – Management and dissemination
*Lead: KU Leuven DistriNet@Gent*

Shares the results through this website, advisory group meetings, hands-on seminars, workshops, a public repository and a practical security guide. See [Knowledge dissemination]({{ '/knowledge-dissemination/' | relative_url }}).

---

## Deliverables

| #    | Deliverable                                                              | Due   |
|------|--------------------------------------------------------------------------|-------|
| R1.1 | Overview of detection and response needs of Flemish SMEs                 | Y1 M4 |
| R1.2 | SWOT analysis of existing technologies                                   | Y1 M4 |
| R1.3 | Technology–needs matrix                                                  | Y2 M2 |
| R2.1 | Report on cyber risk management and analysis for SMEs                    | Y1 M4 |
| R2.2 | Overview of existing and upcoming cybersecurity standards and regulation | Y2 M2 |
| R3.1 | Guidelines for AI-assisted configuration management                      | Y1 M7 |
| R3.2 | Guidelines for automated, context-aware deployment of security tools     | Y2 M6 |
| R4.1 | Guidelines for AI-assisted incident handling and analysis                | Y1 M10 |
| R4.2 | Guidelines for effective and efficient incident triage                   | Y2 M5 |
| R4.3 | Guidelines for effective and efficient incident response                 | Y2 M8 |
| R5.1 | Incident reporting template for SME environments                         | Y1 M7 |
| R5.2 | Guidelines for feedback from post-incident analyses                      | Y2 M6 |
| R6.1 | Technical demonstrators integrated in the testbed                        | Y2 M11 |
| R6.2 | Validation report of the worked-out cases                                | Y2 M11 |
| R7.8 | Practical security guide *"From Detection to Response"*                  | Y2 M12 |

<!-- TODO: once a deliverable is published, link it from the table above and from the Knowledge dissemination page. -->

<style>
.wp-diagram {
  max-width: 760px;
  margin: 2em auto;
  font-weight: 600;
}
.wp-row {
  display: flex;
  gap: 0.5em;
  margin-bottom: 0.5em;
}
.wp-box {
  flex: 1;
  background: #4472c4;
  color: white;
  text-align: center;
  padding: 0.9em 0.6em;
  border-radius: 4px;
  line-height: 1.3;
}
.wp-box small {
  font-weight: 400;
  opacity: 0.9;
}
.wp-arrow {
  text-align: center;
  color: #4472c4;
  font-size: 1.3em;
  margin: -0.2em 0 0.3em 0;
}
@media screen and (max-width: 600px) {
  .wp-three {
    flex-direction: column;
  }
}
</style>
