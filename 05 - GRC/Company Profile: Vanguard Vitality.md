# Company Profile: Vanguard Vitality

## Overview
**Vanguard Vitality** is a rapidly expanding, regional fitness chain with five locations. Founded by fitness enthusiasts rather than corporate administrators, the company has historically prioritized gym equipment and member experience over robust IT infrastructure. 

## The Onboarding Process
To handle the influx of new members, Vanguard Vitality currently uses a standard, public-facing Google Form linked on their website and social media. When a prospective member applies, the form responses automatically populate into a single Google Sheet. 

---

## The Google Form Application
Here is a breakdown of the specific data fields Vanguard Vitality collects on their form:

| Field Category | Specific Data Collected | Sensitivity Level |
| :--- | :--- | :--- |
| **Basic Identification** | Full Name, Date of Birth, Home Address | Moderate |
| **Contact Information** | Email Address, Personal Cell Phone Number | Moderate |
| **Financial Details** | Bank account routing and account numbers for monthly drafts | Critical |

---

## Risk Assessment Matrix

### Scoring Key (Likelihood x Impact)
* **Likelihood:** 1 (Rare) to 5 (Almost Certain)
* **Impact:** 1 (Negligible) to 5 (Severe)
* **Risk Level:** * **1-6:** Low
  * **8-12:** Medium
  * **15-20:** High
  * **25:** Critical

---

### Vanguard Vitality: Information Systems Risk Register

| Risk ID | Risk Description | Likelihood (1-5) | Impact (1-5) | Overall Risk Score | Risk Level | Proposed Mitigation Strategy |
| :--- | :--- | :---: | :---: | :---: | :--- | :--- |
| **RSK-01** | **Exfiltration of Financial Data:** Unauthorized access to the unsecured Google Sheet containing bank routing and account numbers. | 4 | 5 | **20** | **High** | Immediately migrate financial onboarding to a PCI-compliant payment gateway (e.g., Stripe, Square) and purge financial data from all spreadsheets. |
| **RSK-02** | **Exposure of Protected Health Information (PHI):** Mishandling or breach of medical conditions and medication history collected on the onboarding form. | 4 | 5 | **20** | **High** | Stop collecting detailed medical history via Google Forms. Implement a secure, HIPAA-compliant health waiver system or utilize encrypted intake software. |
| **RSK-03** | **Loss of Database Access (Shadow IT):** The company loses access to the primary intake form and historical database because it is owned by a former employee's personal Gmail account. | 3 | 4 | **12** | **Medium** | Recreate the form under an official corporate Google Workspace account. Export all existing data to the corporate environment and sever the link to the personal account. |
| **RSK-04** | **Data Integrity Compromise:** Accidental deletion or overwriting of member records due to multiple managers editing the same sheet without access controls. | 5 | 3 | **15** | **High** | Implement Principle of Least Privilege. Lock the master sheet from direct editing and use a dedicated CRM (Customer Relationship Management) tool to manage member profiles. |
| **RSK-05** | **Regulatory Non-Compliance (Privacy):** Collecting personal data without explicit consent or a documented data retention/privacy policy. | 5 | 3 | **15** | **High** | Draft and publish a formal privacy policy. Add a mandatory checkbox to the intake form acknowledging the policy and consent to data processing. Implement a 90-day retention limit for non-active leads. |
