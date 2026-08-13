# GRC Program — Scenario Companies (Companion to the 45-Day Mastery Plan)

> **Note:** All organizations below are **fictional**, created for training purposes. Real cities and countries are used for realism (as in the PayFlow example), but the companies, incidents, and weaknesses described are invented and do not represent any actual organization. Scenario 1 (PayFlow) is reproduced in summary for continuity; Scenarios 2–6 are new.

These five companies span different **sectors**, **organizational life-phases**, **geographies**, and **regulatory regimes** — chosen to reflect where GRC professionals are most in demand. A student can run the *entire* 45-day program against any one of them; each also "shines" for particular weeks (see the mapping table at the end).

---

## SCENARIO 1 (Reference): FINTECH STARTUP — "PAYFLOW" · Lagos, Nigeria
Early-growth fintech startup processing digital payments for SMEs. Scaled 8 → 45 staff in a year; loose access control, no security policies, no incident response plan, no risk assessments; an exposed API key surfaced on public GitHub. Preparing for international payment partnerships requiring PCI DSS and ISO/IEC 27001. A GRC analyst is brought in to assess risk, implement controls, and prepare for compliance and audits.

PayFlow is a fast-growing fintech startup based in Lagos, Nigeria. The company provides digital payment solutions for small and medium-sized businesses, enabling merchants to accept payments via cards, bank transfers, and mobile wallets. Over the past year, PayFlow has scaled rapidly from a team of 8 employees to over 45 staff members, with thousands of daily transactions being processed through its platform. The infrastructure is hosted primarily on cloud services, with a mix of virtual machines and
managed services. 

The backend APIs handle sensitive financial transactions and are integrated with third-party payment processors. Customer data stored includes personally identifiable information (PII) such as names, phone numbers, email addresses, and partial financial details. Some logs and backups are stored in cloud storage buckets, but there is no consistent encryption policy across all systems. Access control within the organization is loosely managed. Developers have broad access to production systems, and there is no strict enforcement of role-based access control (RBAC). Multi-factor authentication (MFA) is enabled for some administrative accounts, but not consistently across all users. 

Employee onboarding is fast-paced, often skipping formal security briefings. The company has no formalized security policies in place. There is no documented incident response plan, and risk assessments have never been formally conducted. Recently, a minor security incident occurred where an exposed API key was discovered on a public GitHub repository, raising concerns among investors. PayFlow is preparing to partner with international payment providers, which requires alignment with standards like PCI DSS and ISO/IEC 27001. Leadership has now decided to prioritize security governance and has brought in a GRC analyst (your student) to assess risks, implement controls, and prepare the company for compliance and audits.

---

## SCENARIO 2: HEALTHCARE PROVIDER — "NOVACARE HEALTH"
**Sector:** Healthcare · **Phase:** Mid-size established, digital transformation · **Location:** Austin, Texas, USA

NovaCare Health is a mid-sized integrated healthcare provider headquartered in Austin, Texas, operating a network of 12 outpatient clinics and a fast-growing telehealth platform serving patients across several states. Founded 18 years ago as a single family practice, NovaCare has grown to roughly 600 employees — physicians, nurses, administrative staff, and a 25-person IT/engineering team assembled only in the last three years to support digital expansion. During the pandemic, telehealth visits exploded, and NovaCare rushed a patient-facing app and video-consultation system into production to meet demand.

The infrastructure is a mix of on-premise legacy systems and cloud services. The core Electronic Health Record (EHR) system runs on aging on-prem servers, while the newer telehealth platform, patient portal, and scheduling system run in the cloud. Connected medical devices (IoMT) — remote monitoring kits and imaging systems — feed data into the network, often on flat network segments using default credentials. The data held is extensive and highly sensitive: Protected Health Information (PHI) including names, dates of birth, diagnoses, prescriptions, insurance details, payment-card data for co-pays, and some lab/genetic data. PHI flows between the legacy EHR, the cloud telehealth system, and numerous third-party vendors (billing companies, labs, a transcription service, the cloud video provider).

Access control exists on paper but is poorly enforced in practice — clinicians frequently share logins at busy nursing stations, and former contractors' accounts are rarely deactivated promptly. Backups exist but have never been tested for restoration. There is an old HIPAA privacy policy but no comprehensive information security program, no formal risk analysis (a HIPAA Security Rule requirement), and no tested incident response plan.

Recently, a nearby hospital was crippled by ransomware that disrupted patient care for days, alarming NovaCare's board. At the same time, a large employer client is demanding proof of security maturity (a SOC 2 / HITRUST assessment) before renewing a major telehealth contract, and a patient complaint about a mis-sent records email has drawn fresh attention to data handling.

**Compliance drivers:** HIPAA/HITECH, state breach-notification laws, PCI DSS (co-pay card data), SOC 2 / HITRUST for B2B contracts, and GDPR for a small number of EU patients.

**The mandate:** NovaCare has hired a GRC analyst (your student) to conduct the organization's first formal HIPAA risk analysis, tighten access controls and vendor oversight, build an incident response and ransomware-recovery capability, and prepare the organization for its first third-party security audit.

---

## SCENARIO 3: E-COMMERCE MARKETPLACE — "MARKETNEST"
**Sector:** Retail / E-commerce · **Phase:** Rapid scale-up, post-breach crisis · **Location:** Manchester, United Kingdom

MarketNest is a rapidly scaling online marketplace based in Manchester, UK, connecting independent sellers with consumers across the UK and EU for fashion, homeware, and electronics. Launched four years ago, it has grown explosively to 220 employees and over 15,000 third-party sellers, processing hundreds of thousands of orders monthly — with traffic multiplying tenfold during seasonal peaks like Black Friday and the holidays.

The platform is cloud-native and built on microservices, with many third-party integrations: a payment gateway, shipping and logistics APIs, marketing and analytics platforms, customer-support chat tools, and a recommendation engine. Card payments are handled mostly through a third-party processor, but some legacy checkout flows still touch cardholder data. The company holds customer PII (names, addresses, emails, phone numbers, purchase history), partial card data, and seller business and banking details. A large volume of behavioural and marketing data is routinely shared with ad-tech partners.

The culture has prioritized speed over security. Numerous marketing and analytics SaaS tools were adopted by individual teams without any security review (shadow IT). Access to the customer database is broad across engineering, support, and marketing, with limited logging. Customer data is regularly copied into analytics environments and spreadsheets with no data-loss-prevention controls. A privacy notice exists, but the data-handling discipline behind it is weak.

MarketNest has just suffered a serious breach: an attacker exploited a vulnerable third-party support plugin and exfiltrated a customer database of roughly 400,000 records. The breach reached local news, the UK Information Commissioner's Office (ICO) has opened an inquiry — UK GDPR carries heavy fines — and several large sellers are threatening to leave the platform. Customer trust and brand reputation are now on the line.

**Compliance drivers:** UK GDPR / EU GDPR, PCI DSS, emerging EU digital regulations, and contractual security demands from enterprise sellers and payment partners.

**The mandate:** The GRC analyst (your student) is brought in during crisis-recovery to lead the post-incident review, stand up a proper third-party/vendor risk management programme, implement data classification and DLP, formalize incident response, and demonstrate GDPR accountability to regulators and partners.

---

## SCENARIO 4: ENERGY UTILITY — "HELIOS GRID UTILITIES"
**Sector:** Energy / Critical Infrastructure · **Phase:** Mature incumbent modernizing legacy OT · **Location:** Frankfurt, Germany (EU)

Helios Grid Utilities is a regional electricity distribution operator headquartered in Frankfurt, Germany, supplying power to roughly 1.4 million households and businesses across several districts. A 40-year-old utility with around 3,200 employees, Helios is a mature, heavily regulated incumbent in the middle of a major modernization: rolling out smart meters, grid-automation sensors, and a renewable-integration platform — while still running decades-old operational technology (OT) and SCADA systems that control substations and distribution.

There is a sharp divide between corporate IT (email, ERP, billing, customer portal — modern and cloud-connected) and OT/ICS (industrial control systems running the grid — legacy, partly unsupported, historically "air-gapped" but increasingly networked for remote monitoring). The smart-grid rollout introduces thousands of internet-connected field devices from multiple vendors. The organization holds customer billing data and consumption data, plus highly sensitive operational data about grid topology and control systems. A successful attack could cause physical outages affecting public safety — raising the stakes far beyond data confidentiality.

IT and OT are governed by different teams with no unified security program. OT engineers prioritize uptime and safety over patching, and many control systems cannot be easily updated. Remote-access pathways for vendors into the OT environment are poorly inventoried. Identity and access management is fragmented across old and new systems, and there is no consolidated asset inventory spanning IT and OT.

European energy operators have faced a wave of nation-state and ransomware threats, and a peer utility in a neighboring country recently suffered an OT-disrupting attack. Regulators are tightening requirements under the EU's NIS2 Directive, and Germany's BSI/KRITIS critical-infrastructure rules now demand demonstrable cybersecurity governance, risk management, and incident reporting. Helios faces formal audits and potential penalties for non-compliance.

**Compliance drivers:** NIS2 Directive, national KRITIS/BSI requirements, IEC 62443 (OT/ICS security), ISO/IEC 27001, and NIST CSF as a guiding framework.

**The mandate:** The GRC analyst (your student) is tasked with establishing a unified IT/OT cybersecurity governance program aligned to NIST CSF, building a complete asset inventory and risk register spanning both environments, managing third-party (vendor and OT-supplier) risk, and preparing Helios for NIS2/KRITIS regulatory audits.

---

## SCENARIO 5: B2B SaaS COMPANY — "QUANTA LABS"
**Sector:** Technology / B2B SaaS · **Phase:** High-growth scale-up chasing certification · **Location:** Bangalore, India

Quanta Labs is a fast-growing B2B SaaS company based in Bangalore, India, offering an AI-powered people-analytics and HR-workflow platform used by mid-market and enterprise clients in India, the US, and Europe. Three years old and fresh off a Series B funding round, Quanta has scaled from 30 to 180 employees and is aggressively pursuing larger enterprise customers — who bring much bigger contracts but also much tougher security expectations.

The platform is fully cloud-native, with a multi-tenant architecture on a major cloud provider, CI/CD pipelines, containerized microservices, and a data platform that ingests sensitive HR data from client organizations. Quanta holds large volumes of employee PII on behalf of its customers — names, contact details, compensation, performance data, and sometimes sensitive categories — making it a data processor with significant downstream obligations.

Quanta has a classic high-growth startup posture: security has lagged behind engineering velocity. There is no formal Information Security Management System (ISMS), security policies are ad hoc, access to production and customer data is broad among engineers, secrets management is inconsistent, and there is no structured security-awareness training despite rapid hiring. Logging and monitoring are minimal.

The pressure is now commercial. Enterprise deals are stalling in procurement: prospects are sending lengthy security questionnaires and demanding a SOC 2 Type II report and/or ISO/IEC 27001 certification before they will sign. Two large deals are on hold pending evidence of a mature security program, and investors want the compliance gap closed quickly to unlock the company's next stage of growth.

**Compliance drivers:** SOC 2 (Trust Services Criteria), ISO/IEC 27001:2022, GDPR (EU customers' data), India's Digital Personal Data Protection Act 2023, and customer-contractual security requirements.

**The mandate:** The GRC analyst (your student) is hired to stand up an ISMS from scratch, run a gap assessment against SOC 2 and ISO 27001, implement core controls (IAM, access reviews, change management, vendor risk), launch a security-awareness program, and shepherd Quanta through its first external certification audit — directly enabling enterprise sales.

---

## SCENARIO 6: GOVERNMENT AGENCY — "NATIONAL DIGITAL SERVICES AUTHORITY (NDSA)"
**Sector:** Government / Public Sector · **Phase:** Large public institution under reform & scrutiny · **Location:** Nairobi, Kenya

The National Digital Services Authority (NDSA) is a **fictional** government agency in Nairobi, Kenya, responsible for delivering digital public services — online identity, tax and licensing portals, and citizen benefit programs — to tens of millions of citizens. A large, mature public institution with roughly 1,500 staff plus many contractors, NDSA is in the middle of an ambitious digital-transformation mandate: consolidating fragmented legacy systems, moving services to the cloud, and launching a unified citizen-identity platform.

The infrastructure is a complex mix of aging government data centers, legacy database systems, and newer cloud deployments, stitched together with integrations to banks, ministries, and external service providers. The data is among the most sensitive imaginable: national identity records, biometric data, tax and financial information, and health and benefits data — for the entire citizenry. The scale and sensitivity make NDSA a prime target for criminal and nation-state actors, and a single major breach would carry national consequences and severely erode public trust.

Governance is bureaucratic and siloed. Security responsibilities are unclear across departments and contractors; procurement is slow; legacy systems are difficult to secure; and privileged access is widely and informally held, with poor offboarding of departing staff and vendors. Documentation is inconsistent, and there has never been an enterprise-wide risk assessment. Unlike private firms, NDSA also operates under intense public accountability — freedom-of-information expectations, media attention, and parliamentary oversight.

Recently, investigative journalists revealed that a misconfigured database briefly exposed citizen records, prompting public outcry and a parliamentary inquiry. International development partners funding the modernization now require demonstrable security governance and independent audits before releasing further funds.

**Compliance drivers:** Kenya's Data Protection Act 2019 (and the Office of the Data Protection Commissioner), national cybersecurity regulations, NIST SP 800-53 / NIST CSF and the Risk Management Framework (commonly adopted as a baseline), ISO/IEC 27001, and donor/international audit requirements (including FedRAMP-style expectations for cloud authorization).

**The mandate:** The GRC analyst (your student) is engaged to establish enterprise security governance, lead the first organization-wide risk assessment, implement strong identity, access, and privileged-access management, build vendor/third-party oversight, formalize incident response, and prepare NDSA for independent audits — all under intense public and political scrutiny.

---

## Mapping Scenarios to the 45-Day Program

Every scenario supports the **full** program, but each is especially rich for certain weeks/deliverables. Assign students a primary company for continuity, and use a second for contrast where useful.

| Program Week / Deliverable | PayFlow (Fintech) | NovaCare (Health) | MarketNest (Retail) | Helios (Energy) | Quanta (SaaS) | NDSA (Gov) |
|---|---|---|---|---|---|---|
| **Wk 1 – Governance** | ● | ● | ● | ★ unified IT/OT governance | ● | ★ enterprise gov under scrutiny |
| **Wk 2 – Risk Mgmt** | ● | ★ HIPAA risk analysis | ● | ★ IT+OT risk register | ● | ★ first enterprise-wide assessment |
| **Wk 3 – Compliance/Frameworks** | ★ PCI/ISO | ★ HIPAA/HITRUST | ★ GDPR/PCI | ★ NIS2/IEC 62443 | ★ SOC 2/ISO 27001 | ★ 800-53/RMF |
| **Wk 4 – Audits & Reporting** | ● | ● | ● | ★ regulatory audit | ★ certification audit | ★ independent/donor audit |
| **Wk 5 – Asset Mgmt & IAM** | ● | ● | ● | ★ IT/OT asset inventory | ● | ★ privileged access (PAM) |
| **Wk 6 – Awareness / DLP / IR / 3rd-party** | ● IR (API key) | ★ ransomware IR + vendor risk | ★ DLP + post-breach IR + vendor | ★ OT-vendor risk | ★ awareness program | ● IR + vendor |
| **Wk 7 – NIST CSF Capstone** | ● | ● | ● | ★ flagship NIST CSF program | ● | ★ 800-53/CSF program |

★ = especially strong fit · ● = solid fit

**Suggested pairings for variety:** Fintech ↔ SaaS (both startup-phase, different frameworks) · Healthcare ↔ Retail (both breach/PII-driven, HIPAA vs GDPR) · Energy ↔ Government (both large, mature, critical, OT/legacy and public-interest stakes).
