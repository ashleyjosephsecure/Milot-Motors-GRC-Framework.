# 📋 SOP-001: Unauthorized Enumeration Response
**Standard Operating Procedure for Milot Motors Security Operations**

---

## 1. Objective
To provide Tier 1 SOC Analysts with a structured workflow for detecting, analyzing, and neutralizing unauthorized directory brute-forcing and network scanning.

## 2. Detection (NIST DE.AE-2)
The SOC will be alerted by the SIEM if any of the following triggers occur:
* **Trigger A:** More than 50 "404 Not Found" errors from a single source IP within 60 seconds.
* **Trigger B:** Detection of common user-agents associated with scanning tools (e.g., `dirb`, `nmap`, `gobuster`).

## 3. Immediate Action Steps
| Step | Action | Description |
| :--- | :--- | :--- |
| **1** | **Identify** | Extract the source IP address from the logs. |
| **2** | **Verify** | Cross-check the IP against the "Authorized Vendor List." If not found, treat as malicious. |
| **3** | **Contain** | Implement a 24-hour block on the Web Application Firewall (WAF) for the offending IP. |
| **4** | **Escalate** | Notify the GRC lead to document a "Attempted Unauthorized Access" incident for the quarterly risk report. |

## 4. Post-Incident Review
* Did the attacker find any sensitive directories before being blocked?
* Does the `/admin` portal need to be moved behind a VPN?
* Update the Blocklist with the offending IP range.

---
*Last Updated: February 14, 2026*
