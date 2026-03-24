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

## GRC Summary & Implications

This current setup presents several immediate challenges from an information systems perspective.

### 1. Governance
* **Access Control:** The underlying Google Sheet is currently shared via an "Anyone with the link can view/edit" URL among the five gym managers to make processing easier. There is no centralized access management or principle of least privilege enforced.
* **Data Retention:** Vanguard Vitality has no established policy for how long application data is kept. Applications from people who canceled their memberships years ago still sit in the original spreadsheet.
* **Asset Ownership:** The Google Form was created using a former manager's personal Gmail account rather than a corporate workspace account, creating a severe gap in administrative control.

### 2. Risk
* **Data Breach Vulnerability:** Storing critical financial data (routing numbers) and sensitive health information in a weakly secured spreadsheet creates a massive risk for data exfiltration.
* **Data Integrity:** Because multiple managers edit the same sheet without tracking changes, there is a high risk of accidental data deletion or modification. 
* **Shadow IT:** Reliance on a personal Google account means the company could lose access to their entire membership database if that former manager deletes their account or changes the password.

### 3. Compliance
* **PCI-DSS (Payment Card Industry Data Security Standard):** While they are collecting bank details rather than credit cards, storing financial routing data in an unencrypted, broadly accessible format violates basic financial data security standards.
* **HIPAA / Health Privacy Laws:** Collecting specific medical conditions and medication history on an unsecured form exposes the company to severe regulatory penalties regarding the mishandling of Protected Health Information (PHI).
* **General Privacy Regulations:** The form lacks a privacy policy acknowledgment, meaning applicants do not officially consent to how their data will be stored, used, or processed.
