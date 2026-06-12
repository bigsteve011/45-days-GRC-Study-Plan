# 45-Day GRC Mastery Plan — Beginner to Professional
### Governance, Risk & Compliance in Cybersecurity · 5 hours/week

---

## How to Use This Plan

- **Duration:** 45 days, structured as 7 weeks (Week 7 is a 3-day finish).
- **Time budget:** ~5 hours/week, split into **3 sessions** so it fits around work/life.
  - Suggested split: **Session A = 2 hrs · Session B = 1.5 hrs · Session C = 1.5 hrs.**
  - Swap the days to whatever suits you (e.g., Tue / Thu / Sun).
- **Total guided time:** ~32 hours of focused learning + a capstone project.
- **Learning loop each week:** *Learn the concept → Apply it in a hands-on exercise → Produce a portfolio artifact → Self-check against the milestone.*
- **The golden thread:** The **NIST Cybersecurity Framework (CSF) 2.0** and its six Functions — **Govern, Identify, Protect, Detect, Respond, Recover** — tie every week together. You'll reference them weekly and assemble a full program in the capstone.

> **Honest expectation-setting:** 32 hours takes you from zero to *job-ready entry-level GRC analyst* — confident with the vocabulary, frameworks, core artifacts (risk register, gap assessment, audit report, policy), and a portfolio. "Professional" mastery continues afterward through repetition, a certification, and real work. The plan ends with a roadmap for that.

---

## Schedule at a Glance

| Week | Days | Theme | Core Deliverable (Portfolio Artifact) |
|------|------|-------|----------------------------------------|
| 1 | 1–7 | GRC Foundations & Governance | One-page "What is GRC" brief + 25-term glossary |
| 2 | 8–14 | Cybersecurity Risk Management | A completed Risk Register + mini risk assessment |
| 3 | 15–21 | Compliance Frameworks & Regulations | Framework comparison matrix + gap assessment |
| 4 | 22–28 | Audits, Assessments & Reporting | A sample audit report with findings |
| 5 | 29–35 | Asset Management & IAM | Asset inventory + access-control / IAM policy |
| 6 | 36–42 | Awareness, DLP, Incident Response & Third-Party Risk | Awareness plan, DLP policy, IR runbook, vendor assessment |
| 7 | 43–45 | NIST CSF Capstone + Career Launch | Full mini cybersecurity program + résumé/portfolio |

---

## WEEK 1 — GRC Foundations & Governance
**Days 1–7 · ~5 hrs · NIST Function focus: GOVERN**

**Objectives:** Understand what Governance, Risk, and Compliance mean, why they exist, how they interrelate, and what a GRC professional actually does day to day.

**Session A (2 hrs) — Core concepts**
- What is GRC? Define **Governance** (direction & oversight), **Risk** (uncertainty management), **Compliance** (meeting obligations) — and how the three reinforce each other.
- The CIA Triad (Confidentiality, Integrity, Availability) as the foundation of all security objectives.
- The policy hierarchy: **Policy → Standard → Procedure → Guideline** (know the difference cold).

**Session B (1.5 hrs) — Governance structures**
- The **Three Lines of Defense** model (operational management / risk & compliance functions / internal audit).
- Roles & responsibilities: CISO, GRC analyst, risk owner, control owner, auditor.
- Security governance: charters, steering committees, board reporting, "tone at the top."

**Session C (1.5 hrs) — The framework landscape**
- High-level tour of the major frameworks you'll go deep on later: **NIST CSF 2.0, NIST 800-53, ISO/IEC 27001, CIS Controls, COBIT, SOC 2.**
- Introduce the six NIST CSF 2.0 Functions and how this course maps to them.

**Hands-on deliverable:** Write a **one-page "What is GRC" executive brief** + a **glossary of 25 key terms** (define each in your own words).

**Milestone self-check:** Can you explain to a non-technical friend what GRC is, name the three lines of defense, and list the six NIST CSF Functions from memory?

---

## WEEK 2 — Cybersecurity Risk Management
**Days 8–14 · ~5 hrs · NIST Function focus: IDENTIFY**

**Objectives:** Identify, assess, prioritize, and treat cybersecurity risks — the single most important skill in GRC.

**Session A (2 hrs) — Risk fundamentals**
- Core vocabulary: **asset, threat, vulnerability, likelihood, impact**, and **Risk = f(likelihood × impact)**.
- **Inherent vs. residual risk**; **risk appetite vs. risk tolerance**.
- The risk management lifecycle (frame → assess → respond → monitor), referencing **NIST SP 800-39 / 800-37 (RMF)** and **ISO 31000**.

**Session B (1.5 hrs) — Assessing risk**
- **Qualitative** assessment (likelihood/impact matrices, heat maps).
- **Quantitative** assessment: **SLE = Asset Value × Exposure Factor**, **ALE = SLE × ARO** — work a worked example with real numbers.
- Risk scoring and prioritization.

**Session C (1.5 hrs) — Treating & tracking risk**
- The four treatment options: **Avoid, Mitigate, Transfer, Accept.**
- Building and maintaining a **Risk Register** (the GRC analyst's core working document).
- Control selection to reduce risk to acceptable levels.

**Hands-on deliverable:** Build a **Risk Register** for a fictional small company (≥10 risks) with likelihood, impact, scores, owners, and treatment decisions. Run one **quantitative calculation** (SLE/ALE).

**Milestone self-check:** Given a scenario, can you identify the asset/threat/vulnerability, score the risk, and recommend a justified treatment?

---

## WEEK 3 — Compliance Frameworks & Regulatory Requirements
**Days 15–21 · ~5 hrs · NIST Function focus: GOVERN / IDENTIFY**

**Objectives:** Understand the major control frameworks and the laws/regulations that drive compliance, and learn to map controls and find gaps.

**Session A (2 hrs) — Control frameworks**
- Deep-dive: **NIST CSF 2.0**, **NIST SP 800-53** (control catalog), **ISO/IEC 27001:2022** (ISMS + Annex A), **CIS Controls v8**, **SOC 2** (Trust Services Criteria), **COBIT** (IT governance).
- When you'd use each and how they differ (prescriptive vs. risk-based vs. certification-oriented).

**Session B (1.5 hrs) — Laws & regulations**
- **GDPR** (EU privacy), **HIPAA** (US healthcare), **PCI DSS** (payment cards), **SOX** (financial reporting), **CCPA/CPRA**, **GLBA**. Know *who they apply to* and *what they require*.
- Privacy vs. security; data classification basics.

**Session C (1.5 hrs) — Mapping & gap assessment**
- **Control crosswalks / mapping** (one control satisfying multiple frameworks).
- The **gap assessment** process: current state vs. required state → remediation plan.

**Hands-on deliverable:** Create a **framework comparison matrix** (NIST CSF vs. ISO 27001 vs. CIS, with pros/cons/use-cases) **+** run a **mini gap assessment** against ~10 NIST CSF subcategories for your fictional company.

**Milestone self-check:** Can you match a given organization (e.g., a hospital, an e-commerce store) to the regulations that apply to it and justify a framework choice?

---

## WEEK 4 — Audits, Assessments & Reporting
**Days 22–28 · ~5 hrs · NIST Function focus: DETECT / GOVERN**

**Objectives:** Plan and conduct a cybersecurity audit and write a clear, professional audit report.

**Session A (2 hrs) — Audit fundamentals**
- Audit types: internal vs. external, **1st/2nd/3rd-party**; compliance audit vs. risk assessment vs. penetration test (know the difference).
- The audit lifecycle: **scoping → planning → fieldwork (evidence gathering) → analysis → reporting → follow-up.**
- Evidence and **testing methods**: inquiry, observation, inspection, re-performance.

**Session B (1.5 hrs) — Findings & evidence**
- Writing strong **findings**: Condition, Criteria, Cause, Consequence, Recommendation (the "5 C's").
- Rating findings by severity/risk; designing remediation timelines.
- Working papers and audit trails.

**Session C (1.5 hrs) — The audit report**
- Structure of a professional report: executive summary, scope/methodology, findings, recommendations, management response.
- Communicating to technical *and* executive audiences.

**Hands-on deliverable:** Conduct a **mock audit** of your fictional company against 8–10 controls and write a **complete audit report** with at least 3 findings (each using the 5 C's) and an executive summary.

**Milestone self-check:** Could you hand your report to a manager and have the findings be clear, defensible, and actionable?

---

## WEEK 5 — Asset Management & Identity and Access Management (IAM)
**Days 29–35 · ~5 hrs · NIST Function focus: IDENTIFY / PROTECT**

**Objectives:** Manage organizational assets and design strong identity & access controls.

**Session A (2 hrs) — Asset management**
- Why "you can't protect what you don't know you have." Hardware, software, data, and people as assets.
- Asset inventory, ownership, and **data classification** (public / internal / confidential / restricted).
- Asset lifecycle: acquisition → use → maintenance → secure disposal.

**Session B (1.5 hrs) — IAM core concepts**
- **AAA**: Authentication, Authorization, Accounting.
- **Least privilege** and **separation of duties**.
- Access models: **RBAC, ABAC, MAC, DAC**; **MFA**; privileged access management (PAM).

**Session C (1.5 hrs) — IAM lifecycle & governance**
- Joiner–Mover–Leaver (JML) provisioning/deprovisioning.
- **Access reviews / recertification** (a recurring GRC task).
- Identity governance and common IAM audit findings.

**Hands-on deliverable:** Build an **asset inventory** (with classifications) **+** draft an **Access Control / IAM policy** that defines roles, least-privilege rules, MFA requirements, and a quarterly access-review process.

**Milestone self-check:** Can you design a role-based access scheme for a small org and explain how you'd prove (to an auditor) that access is appropriate?

---

## WEEK 6 — Awareness, DLP, Incident Response & Third-Party Risk
**Days 36–42 · ~5 hrs · NIST Function focus: PROTECT / RESPOND / RECOVER**

> This is the most packed week — four connected topics. Keep deliverables lean (1 page each). If you need more time, this is the natural place to add a buffer day.

**Session A (2 hrs) — Security education & awareness + DLP**
- Building a **security awareness program**: audience segmentation, phishing simulations, metrics, reinforcing a security culture.
- **Data Loss Prevention (DLP)**: data-in-use / in-motion / at-rest; DLP policies, detection rules, and how DLP enforces data classification.

**Session B (1.5 hrs) — Incident response**
- The IR lifecycle (NIST SP 800-61): **Preparation → Detection & Analysis → Containment, Eradication & Recovery → Post-Incident (lessons learned).**
- Roles, escalation, communication, and the link to **Business Continuity / Disaster Recovery (BCP/DR)**.

**Session C (1.5 hrs) — Third-party / vendor risk management**
- Why vendors are a top breach vector; the **vendor risk lifecycle** (due diligence → onboarding → monitoring → offboarding).
- Security questionnaires, SOC 2 reports, contractual clauses, and continuous monitoring.

**Hands-on deliverables (keep each to ~1 page):**
1. A **security awareness program outline** (topics, cadence, metrics).
2. A short **DLP policy**.
3. An **incident response runbook** for one scenario (e.g., ransomware or phishing-led breach).
4. A **third-party risk assessment** (questionnaire + risk rating for one fictional vendor).

**Milestone self-check:** Can you walk through what happens, step by step, from the moment an incident is detected — and explain how you'd vet a new SaaS vendor?

---

## WEEK 7 — NIST CSF Capstone + GRC Career Launch
**Days 43–45 · ~3 hrs · NIST Function focus: ALL SIX**

**Objectives:** Tie everything together into a mini cybersecurity program, and prepare to pursue GRC roles.

**Day 43 (1.5 hrs) — Capstone build**
- Assemble your week-by-week artifacts into a single **"Cybersecurity Program for [Fictional Company]"** organized by the **six NIST CSF 2.0 Functions**:
  - **Govern** → your governance brief, policies, roles.
  - **Identify** → asset inventory + risk register.
  - **Protect** → IAM policy, DLP policy, awareness plan.
  - **Detect** → audit/monitoring approach.
  - **Respond** → incident response runbook.
  - **Recover** → BCP/DR notes + lessons-learned process.
- Write a 1-page executive summary of the program and its current maturity.

**Day 44 (1 hr) — Career prep**
- **GRC career landscape:** common entry roles (GRC Analyst, IT Auditor, Compliance Analyst, Risk Analyst, Security Analyst).
- **Certification roadmap** (pick a target — see below).
- Build/refresh a **résumé** highlighting your portfolio artifacts; optimize a LinkedIn profile with GRC keywords.

**Day 45 (0.5 hr) — Interview & next steps**
- Prep answers to common GRC interview questions (e.g., "Walk me through a risk assessment," "How do you handle a control that's failing an audit?").
- Set a 90-day post-course plan (cert study + a real or open-source project).

**Final deliverable:** A polished **portfolio** (capstone program + all weekly artifacts) and an updated **résumé/LinkedIn**.

---

## Capstone Project — "Mini GRC Program in a Box"

By Day 45 you'll have a cohesive portfolio that demonstrates real competence:

- [ ] GRC executive brief + glossary
- [ ] Risk register (with a quantitative example)
- [ ] Framework comparison matrix + gap assessment
- [ ] Audit report with findings (5 C's)
- [ ] Asset inventory + IAM/access-control policy
- [ ] Awareness program outline
- [ ] DLP policy
- [ ] Incident response runbook
- [ ] Third-party/vendor risk assessment
- [ ] Capstone: full program mapped to NIST CSF 2.0 + executive summary

This portfolio is your strongest interview asset — it proves you can *do the work*, not just describe it.

---

## Recommended Resources (mostly free)

**Primary frameworks & guidance (authoritative, free):**
- **NIST Cybersecurity Framework 2.0** — nist.gov/cyberframework
- **NIST SP 800-53** (controls), **800-30** (risk assessment), **800-37** (RMF), **800-39** (risk management), **800-61** (incident handling)
- **ISO/IEC 27001:2022** (ISMS) — overview material is free; the standard itself is paid
- **CIS Controls v8** — cisecurity.org (free download)
- **SOC 2 / Trust Services Criteria** — AICPA

**Learning sources:**
- NIST and CISA (cisa.gov) free guidance and toolkits
- SANS reading room (free whitepapers)
- ISACA articles and glossaries
- Vendor blogs and YouTube channels dedicated to GRC analyst skills

**Certification roadmap (choose based on your goal):**
- **Foundational:** CompTIA Security+ (broad security base) · ISC2 Certified in Cybersecurity (CC)
- **GRC-specific:** **OCEG GRC Professional (GRCP)** · **ISC2 CGRC** (Governance, Risk & Compliance; formerly CAP)
- **Risk-focused:** **ISACA CRISC** (Certified in Risk and Information Systems Control)
- **Audit-focused:** **ISACA CISA** (Certified Information Systems Auditor)
- **Governance/leadership (later-stage):** ISACA CGEIT · ISC2 CISSP

> Certification details and exam requirements change over time — verify current specifics on each provider's site before committing.

---

## Tips for Success

1. **Produce, don't just consume.** The weekly artifact matters more than the reading. Employers hire for what you can build.
2. **Reuse one fictional company** all the way through — it makes every deliverable connect and turns into a believable capstone.
3. **Speak the language.** Re-read your glossary weekly; fluency in GRC vocabulary is half the interview.
4. **Map everything back to NIST CSF.** Treat the six Functions as the filing cabinet for every concept you learn.
5. **Stay consistent over intense.** Three reliable sessions a week beats one heroic cram. If you fall behind, shrink the deliverable rather than skip it.

---

## Beyond Day 45 (Continuing to "Professional")

- **Weeks 7–12:** Study for one certification (CRISC, CISA, CGRC, or GRCP) — your portfolio already covers much of the material.
- **Ongoing:** Contribute to or recreate a real control framework mapping; follow regulatory updates (GDPR/CCPA/sector rules); practice mock audits.
- **Hands-on:** Try a free-tier GRC platform or spreadsheet-based GRC to manage a live risk register and control library.

*You finished this plan with a portfolio, a vocabulary, and a framework-based mental model. That's a credible entry-level GRC foundation — keep building on it.*
