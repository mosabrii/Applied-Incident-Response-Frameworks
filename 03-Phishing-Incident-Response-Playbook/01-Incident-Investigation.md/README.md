# Incident Investigation

## Alert Overview

- **Alert Type:** Phishing attempt with possible malware download  
- **Severity Level:** Medium  
- **Targeted User:** HR employee  

The alert was triggered after a phishing email successfully led to the download and execution of a malicious file on an employee endpoint.

---

## Incident Timeline

- **1:11 PM:** Phishing email delivered to the HR employee inbox  
- **1:13 PM:** Employee opened the email and downloaded the attachment  
- **1:17 PM:** Malicious file executed on the endpoint  
- **1:21 PM:** Security monitoring system generated an alert and notified SOC  

---

## Email & Attachment Analysis

The phishing email impersonated a legitimate job application request and prompted the employee to review an attached CV.  
The attachment was password-protected, with the password included directly in the email body.  

This technique is commonly used in phishing campaigns to:
- Bypass email security controls
- Increase user curiosity and trust
- Encourage manual execution of the attachment  

Targeting the HR department with a CV-related message is a strong social engineering indicator and aligns with known phishing tactics.

---

## File Validation

- **Hash Type:** SHA-256  
- **File Hash:**  
  `54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b`

The file hash was analyzed using VirusTotal.  
Results showed detection by approximately **95 security vendors**, confirming the file as **malicious**.

---

## Impacted Asset

- **Affected Device:** HR employee workstation  

Security telemetry confirmed that:
- Unauthorized executable files were created on the system
- The file was actively executed, not merely downloaded  

This confirms that the endpoint was compromised.

---

## Investigation Assessment

This incident is classified as a **confirmed phishing attack**, not a false positive.

Key indicators include:
- Successful user interaction with the malicious attachment
- Verified malicious hash with high vendor detection
- Unauthorized file execution on the endpoint
- Targeted social engineering against an HR user  

Due to the confirmed execution and the critical role of the affected user, the incident requires escalation to contain potential lateral movement and prevent further spread within the network.
