---
tags:
  - security
  
hide:
  - toc
---

# Qualitative and Quantitative Risk Assessment

Risk assessments can be performed using qualitative methods, quantitative methods, or a combination of both. Each approach serves a different purpose and level of maturity, and both are valid when applied appropriately.

---

## Qualitative Risk Assessment

Qualitative risk assessment evaluates risk using descriptive scales rather than precise numerical values. It focuses on relative severity and likelihood to support prioritisation and decision-making.

### Characteristics
- Uses categories such as **Low / Medium / High**
- Relies on expert judgement and contextual understanding
- Faster to perform and easier to communicate
- Commonly used as a baseline or first-pass assessment

### Typical Outputs
- Risk registers
- Heat maps or risk matrices
- Ranked lists of risks

### Example (Qualitative)

**Scenario:**  
Remote access to an OT network is protected by single-factor authentication.

- **Likelihood:** Medium  
  (Remote access is actively used and exposed, but not publicly accessible)
- **Impact:** High  
  (Compromise could disrupt production and impact safety)
- **Risk Rating:** High

This result indicates the risk should be prioritised for treatment, such as implementing multi-factor authentication or additional monitoring.

!!! note
    Qualitative assessments are particularly effective when data is limited or when rapid prioritisation is required.

---

## Quantitative Risk Assessment

Quantitative risk assessment uses numerical values to estimate risk in financial or operational terms. It focuses on measurable impact and probability to support cost-based decision-making.

### Characteristics
- Uses numerical values (e.g. dollars, downtime hours)
- Requires reliable data and assumptions
- More complex and time-consuming
- Commonly used for high-impact or high-cost decisions

### Typical Outputs
- Estimated annual loss
- Cost-benefit analysis
- Return on investment (ROI) justification

### Example (Quantitative)

**Scenario:**  
Ransomware impacting a critical business system.

- **Estimated impact per incident:**  
  - Downtime cost: \$250,000  
  - Recovery and response: \$150,000  
  - Total impact: \$400,000
- **Estimated likelihood:**  
  Once every 4 years (0.25 per year)

**Annualised Risk:**  
\$400,000 × 0.25 = **\$100,000 per year**

If a proposed control costs \$40,000 per year and significantly reduces the likelihood, the investment can be justified based on risk reduction.

!!! tip
    Quantitative assessments are most valuable when comparing control costs against potential losses.

---

## Using Both Approaches Together

In practice, organisations often use **both qualitative and quantitative methods**.

A common approach is:
1. Use **qualitative assessment** to identify and prioritise risks
2. Apply **quantitative analysis** to a small number of critical or high-cost risks

This balances speed, clarity, and financial justification.

!!! note
    Not every risk requires quantitative analysis. It should be reserved for risks where cost, impact, or investment decisions need stronger justification.

---

## Key Takeaways

- Qualitative assessment answers: *Which risks matter most?*
- Quantitative assessment answers: *How much does this risk cost us?*
- Both approaches support informed, risk-based decision-making
- The method chosen should match the organisation’s maturity and needs
