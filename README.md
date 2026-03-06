# ITGC Audit – SwiftTel Nigeria (Telecommunications)

*This project is inspired by real-world engagements; however, all documents have been independently recreated using synthetic data to reflect practical scenarios. No client materials are reproduced. All templates are either self-developed or open-sourced.*

---

Led an Information Technology General Controls (ITGC) [audit](https://drive.google.com/drive/folders/1UgjnSuxPiqI6DkHrdp2rbvMe2di0buD7?usp=sharing) for a telecommunications provider operating critical network infrastructure, subscriber billing platforms, and customer-facing applications. The assessment evaluated controls across five domains—**Access Control, Backup & Recovery, Change Management, IT Operations, and Program Development & Acquisition**—against industry standards and Nigerian Communications Commission (NCC) requirements to determine the effectiveness of the IT control environment supporting core telecom systems.

---

## Approach
*   Administered a structured **[ITGC Audit Checklist](https://docs.google.com/spreadsheets/d/1iOSQeI6tKEOCyUr4aTtaPOlcRYYJOO-B/edit?usp=sharing&ouid=101134501969411208830&rtpof=true&sd=true)** covering access controls, backup verification, change management processes, patch governance, and SDLC controls for critical systems including OSS/BSS platforms, HSS databases, and billing engines.
  
*   Performed evidence-based testing documented in the **[ITGC Audit Report](https://docs.google.com/document/d/1RBFpGajj-sbt9ljgWmwYAHnomDoBIREk/edit?usp=sharing&ouid=101134501969411208830&rtpof=true&sd=true)**, including access recertification reviews, backup log analysis, change ticket sampling, vulnerability scan validation, job scheduler monitoring, and third-party integration assessments.

---

## Key Findings & Recommendations

*   **Missing MFA on CPNI Databases & Uncleared Contractor Access (Critical):** 15 of 22 database administrators accessed subscriber data without MFA; OSS access review outstanding for two quarters; two ex-contractors retained active access. *Recommendation*: Enforce MFA immediately on all administrative accounts and automate HR-identity integration to disable accounts upon termination.

*   **Untested Disaster Recovery & No Off-Site Backups (Critical):** Production billing engine not restoration-tested in 18 months; backup media stored only in primary data centre with no replication to DR site. *Recommendation*: Schedule live restoration test within next quarter and configure backup replication to geographically separated DR site immediately.

*   **Unpatched Critical Systems & SDLC Bypass (High):** 12 of 20 critical servers missing patches >90 days; customer self-service app launched without mandatory security architecture review; third-party API integrated with no risk assessment. *Recommendation*: Establish formal 30-day patch cycle, enforce security review as mandatory SDLC gate, and implement vendor risk assessment process.

---

## Outcome & Reflection

The audit revealed a mixed control environment: user provisioning, backup completion, CAB approvals, NOC monitoring, incident management, and pre-deployment penetration testing were effective. However, critical gaps—missing MFA on CPNI databases, untested DR capabilities, unpatched systems, and bypassed SDLC controls—exposed subscriber data and network stability to foreseeable failure. Findings reinforced that operational reliability does not guarantee control effectiveness.

---

## Linked Project Documents

ITGC Audit – (Telecommunications)(https://drive.google.com/drive/folders/1UgjnSuxPiqI6DkHrdp2rbvMe2di0buD7?usp=sharing)
