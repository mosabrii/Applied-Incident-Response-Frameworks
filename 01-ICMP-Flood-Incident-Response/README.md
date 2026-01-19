# ICMP Flood DoS Incident Response

## Project Overview
This project simulates a real-world cybersecurity incident involving a Denial of Service (DoS) attack caused by an ICMP flood.  
It represents an incident response scenario where a corporate network experienced service disruption due to misconfigured network security controls.

The purpose of this project is to document and analyze the incident scenario and outline a structured incident response approach.  
Detailed analysis, response actions, and recovery planning are provided within the accompanying incident report files.

---

## Scenario Description
You are a cybersecurity analyst working for a multimedia company that provides web design, graphic design, and social media marketing services to small businesses.

The organization experienced a **Denial of Service (DoS) attack** that disrupted internal network operations for approximately **two hours**.

### What Happened
- Network services became unresponsive due to a large volume of incoming **ICMP packets**
- Legitimate internal traffic was unable to reach network resources
- The incident was traced to a **misconfigured firewall** that allowed unrestricted ICMP traffic
- A malicious actor exploited this misconfiguration to flood the network

### Initial Response Actions
The incident response team took immediate actions to restore services:
- Blocked incoming ICMP traffic
- Disabled non-critical network services
- Restored critical business services

---

## Incident Findings
After investigation, the security team identified:
- An ICMP flood originating from spoofed or untrusted source IP addresses
- Lack of rate limiting and insufficient firewall filtering rules
- Absence of effective monitoring for abnormal traffic patterns

---

## Implemented Security Improvements
To mitigate the incident and prevent future occurrences, the following measures were implemented:
- ICMP rate-limiting firewall rules
- Source IP validation to detect spoofed packets
- Network traffic monitoring to identify abnormal behavior
- Deployment of IDS/IPS to filter suspicious ICMP traffic

---

## Project Scope
This project focuses on:
- Incident scenario analysis and documentation
- Identification of attack type and affected systems
- Incident response planning and process improvement
- Detection, response, and recovery considerations
- Alignment with structured cybersecurity incident response practices

---

## Repository Contents
This project repository includes:
- **Incident Summary** – high-level overview of the incident
- **Incident Report** – detailed technical and operational analysis
- **Supporting Evidence** – logs, observations, or documentation related to the incident

> Note:  
> The exact structure and depth of documentation may vary depending on project requirements.

---

## Disclaimer
- This scenario is fictional and created for educational and professional demonstration purposes only  
- No real systems, organizations, or individuals are involved  
- Any resemblance to real incidents is purely coincidental
