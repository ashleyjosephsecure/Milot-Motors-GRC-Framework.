# 🛡️ Milot Motors: Access Control Policy (ACP)
**Author:** ashleyjosephsecure  
**Version:** 1.0  
**Status:** Internal / Regulatory Compliance  

---

## 1.0 Purpose
This policy defines the standards for granting, reviewing, and revoking access to Milot Motors' internal systems and dealership software. Our goal is to protect client PII (Personally Identifiable Information) and maintain brand integrity.

## 2.0 Core Principles
* **Least Privilege (PoLP):** Users are granted only the minimum access necessary to perform their job functions.
* **Individual Accountability:** No shared accounts. Every action must be traceable to a unique user identity.

## 3.0 Identity Lifecycle (Joiner-Mover-Leaver)
* **Joiners:** Access is granted based on job role. Initial access is "Read-Only" until training is completed.
* **Movers:** When an employee changes roles, all previous permissions are revoked and a new access request must be submitted.
* **Leavers:** Upon termination or resignation, all access is revoked within **24 hours**.

## 4.0 Technical Controls
* **Multi-Factor Authentication (MFA):** Required for all remote and administrative logins.
* **Password Complexity:** Minimum 14 characters, including special characters and numbers.
* **Session Timeout:** Workstations and CRM software will auto-lock after 5 minutes of inactivity.

## 5.0 Compliance Framework Mapping
This policy aligns with international security standards to ensure Milot Motors meets the high expectations of the luxury automotive sector.

| Control | NIST CSF (v2.0) | ISO/IEC 27001:2022 |
| :--- | :--- | :--- |
| Identity Management | PR.AC-01 | Annex A 5.15 & 5.16 |
| Multi-Factor Auth | PR.AC-04 | Annex A 5.17 |
| Least Privilege | PR.AC-03 | Annex A 8.2 |
| Remote Access / VPN | PR.AC-05 | Annex A 6.7 |
| Access Reviews | GV.PO-01 | Annex A 5.18 |

---
**Approved by:** Ashley Joseph, GRC Lead  
**Date:** February 2026
