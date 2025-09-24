# Phishing-email-analysis

# Cybersecurity Case Study: Phishing Email Analysis

This repository contains a detailed, step-by-step analysis of a sample phishing email. The project serves as a practical demonstration of identifying malicious emails using standard cybersecurity tools and techniques.

---

## 🎯 Objective

The goal of this analysis was to dissect a suspicious email pretending to be from the "StreamFlix" streaming service. The process involved identifying characteristics of social engineering, technical spoofing, and malicious intent to determine its threat level.

---

## 📄 The Analysis Report

The complete, in-depth analysis is documented in the following file. It includes the full text of the sample email and a breakdown of each phishing indicator found.

* **➡️ [View the Full Phishing Analysis Report](phishing_analysis_report.md)**

---

## 🔍 Key Findings Summary

The analysis concluded that the email was a definitive phishing attempt based on several critical red flags:

* **Sender Impersonation:** The sender's email address (`info@mailer-cluster-123.net`) did not belong to the official company domain.
* **Suspicious Email Headers:** Technical analysis of the headers revealed a failed SPF check and a mismatched `Reply-To` address pointing to a scammer's inbox.
* **Deceptive URL:** The embedded link pointed to a fake, look-alike domain (`security-center.com`) that was recently registered, a classic tactic for credential harvesting.
* **Social Engineering:** The email body used urgent and threatening language to pressure the user into acting without thinking.

---

## 🛠️ Tools & Techniques Used

This investigation was conducted using a combination of publicly available tools and critical analysis:

* **Email Header Analysis:** MXToolbox / Google Admin Messageheader
* **URL Scanning & Sandboxing:** VirusTotal, URLscan.io
* **Domain Intelligence:** WHOIS Lookup
* **Critical Thinking:** Analysis of social engineering tactics and language.

---

