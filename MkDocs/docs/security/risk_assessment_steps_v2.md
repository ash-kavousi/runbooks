---
tags:
  - security
  
hide:
  - toc
---

# Cybersecurity Risk Assessment Process

This article describes a practical 10-step approach to cybersecurity risk assessment. It walks through scoping, understanding the system, identifying threats and vulnerabilities, assessing controls, and evaluating and treating risk. The approach is designed to be easy to follow, repeatable, and suitable for IT, OT, and hybrid environments.

---

## 1. Scope and Context Definition
*This step prevents “boiling the ocean” and aligns stakeholders.*

Define the boundaries and purpose of the assessment.

- Assessment objective (why the assessment is being performed)
- In-scope systems, processes, applications, or assets
- Explicit out-of-scope items and assumptions
- Business and operational context (IT, OT, safety, regulatory)

!!! warning
    Poorly defined scope is the most common cause of ineffective risk assessments and uncontrolled scope creep.

!!! note
    Early engagement with management helps establish ownership, priorities, and approval before starting a significant security initiative.

---

## 2. System Characterisation
*This step establishes asset value and exposure.*

Understand what you are protecting.

- System architecture, dependencies, and integrations
- Data flows and trust boundaries
- Criticality to business operations, production, safety, or compliance
- Asset owners and key operational stakeholders

!!! tip
    High-level system and data flow diagrams are usually sufficient and significantly improve shared understanding during workshops and reviews.

---

## 3. Threat Identification
*This step focuses on who or what could realistically cause harm to the system.*

Identify credible threat sources and events relevant to the environment.

- External threats (cybercriminals, nation-state actors, hacktivists)
- Internal threats (malicious, negligent, or accidental)
- Environmental or operational threats (power loss, misconfiguration)
- IT-specific and OT-specific threat scenarios

!!! note
    Threat catalogues can be used as reference points, but should be filtered to include only realistic and applicable threats.

---

## 4. Vulnerability Identification & Analysis
*This step focuses on weaknesses in systems, processes, or people that could allow harm to occur.*

Identify weaknesses that threats could exploit.

- Technical vulnerabilities (software, firmware, network)
- Configuration weaknesses
- Process or procedural gaps
- People and capability gaps

!!! tip
    Focus on material weaknesses that meaningfully increase risk rather than compiling exhaustive lists of low-risk findings.

---

## 5. Control Analysis (Current State)
*This step determines the true exposure — not just theoretical risk.*

Assess existing controls and their effectiveness.

- Preventive, detective, and corrective controls
- Technical, administrative, and physical controls
- Control coverage, maturity, and known gaps

!!! note
    This step often produces a valuable by-product in the form of a control gap assessment, which can inform prioritisation and investment decisions.

---

## 6. Likelihood Assessment
*This step estimates how probable a threat scenario is.*

Estimate the probability of threat exploitation by considering:

- Threat capability and intent
- Vulnerability exploitability
- Effectiveness of existing controls
- Environmental exposure

!!! tip
    Likelihood should be assessed using a consistent and repeatable scale (e.g. Low / Medium / High or numeric) to support comparison across risks.

---

## 7. Impact Assessment
*This step evaluates the consequences if a risk materialises.*

Determine the potential impact to the organisation.

- Safety and human impact
- Operational disruption
- Financial loss
- Regulatory or legal consequences
- Reputational damage

!!! note
    Impact ratings should reflect worst-credible outcomes, not worst-case speculation.

---

## 8. Risk Determination (Inherent and Residual)
*This step allows risks to be compared and prioritised.*

Calculate and classify the risk level.

- **Inherent Risk**: Likelihood × Impact (before controls)
- **Residual Risk**: Likelihood × Impact (after controls)
- Risk ratings aligned to the organisation’s risk matrix

!!! tip
    Consistent risk scoring enables meaningful prioritisation and executive-level reporting.

---

## 9. Risk Treatment & Recommendations
*This step defines how risk will be managed.*

Determine how each risk will be handled.

- Mitigate (improve or implement controls)
- Accept
- Transfer
- Avoid

!!! note
    Each treatment decision should clearly identify accountable owners and the intended target risk state.

---

## 10. Documentation, Review & Approval
*This step ensures traceability, governance, and repeatability.*

- Document assumptions, analysis, and decisions
- Obtain stakeholder and risk owner sign-off
- Define review triggers (e.g. annual, post-change, post-incident)

!!! warning
    Risk assessments that are not reviewed regularly can quickly become outdated and misleading.

---

> **Framework Alignment**  
> This risk assessment approach aligns with ISO/IEC 27005 and NIST SP 800-30 and is designed to be applicable across IT, OT, and hybrid environments.

---

<div class="sources-block">
  <div class="sources-title">Sources</div>
  <ul>
    <li><em>NIST SP 800-30 Rev.1 – Guide for Conducting Risk Assessments</em></li>
    <li><em>ISO/IEC 27005 – Information Security Risk Management</em></li>
    <li><em>ISO/IEC 27001 – Information Security Management Systems</em></li>
    <li><em>NIST Cybersecurity Framework (CSF)</em></li>
  </ul>
</div>
