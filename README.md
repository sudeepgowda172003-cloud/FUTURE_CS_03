# 🛡️ API Security Risk Analysis - ReqRes SaaS Audit
**Task 3: Cyber Security Internship @Future Interns**[cite: 1, 4]

## 🔍 Project Overview
Modern SaaS applications rely heavily on APIs to power mobile apps, dashboards, and integrations[cite: 1]. This project involved a **read-only security audit** of the `ReqRes` public API to identify vulnerabilities that could lead to data exposure, authentication bypass, or system abuse.

The audit followed the **OWASP API Security Top 10 (2023)** framework to assess the security posture of the target endpoints[cite: 7].

## 🛠️ Tools & Methodology
*   **Postman (Desktop & Web):** Primary tool for request crafting, header inspection, and automated testing[cite: 1, 7].
*   **Browser DevTools:** Used for supplementary network analysis and header verification[cite: 1, 7].
*   **Methodology:** Read-Only Black-Box Testing. No data was modified or exploited during the assessment[cite: 1, 7].

## 🚩 Key Security Findings
The audit identified **5 major security risks**, categorized by their business impact and severity[cite: 7]:

| Finding ID | Risk Title | Severity | OWASP Reference |
| :--- | :--- | :--- | :--- |
| **F-01** | Broken Authentication & Verbose Error Disclosure | **HIGH** | API2:2023 |
| **F-02** | CORS Misconfiguration (Wildcard Origin `*`) | **MEDIUM** | API7:2023 |
| **F-03** | Improper HTTP Method Handling (`GET` on login) | **MEDIUM** | API7:2023 |
| **F-04** | Sensitive Information Disclosure (Internal Headers) | **LOW** | API7:2023 |
| **F-05** | Plaintext Credential Transmission in JSON Body | **LOW** | API8:2023 |

## 📊 Business Impact
If these vulnerabilities existed in a production SaaS platform, the impact could include:
*   **Data Breaches:** Unauthorized access to customer PII (Personally Identifiable Information)[cite: 7].
*   **Compliance Violations:** Potential fines under **GDPR**, **SOC 2**, and India's **DPDP Act 2023**[cite: 7].
*   **Reputational Damage:** Loss of customer trust and brand value due to security failures[cite: 7].

## 📂 Deliverables
*   `API_Security_Risk_Analysis_Report_Sudeep_M_Improved.pdf`: The full 19-page professional audit report[cite: 7].
*   `/Screenshots/`: Contains Postman request/response captures used as forensic evidence[cite: 7].

## 👨‍💻 Author
**Sudeep M**
*   **Role:** SOC Analyst & Security Consultant[cite: 7]
*   **Internship:** Future Interns Cyber Security
*   **Track Code:** CS[cite: 4]
