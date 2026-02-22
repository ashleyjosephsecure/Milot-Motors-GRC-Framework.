# Playbook: Lost or Stolen Device
**Scope:** Mobile tablets, shop laptops, and employee phones with Milot Motors access.

## 1. Identification
- User reports device missing.
- Administrator (You) identifies the Device ID and Serial Number.

## 2. Containment (Within 30 Minutes)
- **Remote Wipe:** Trigger factory reset via MDM (Mobile Device Management).
- **Session Kill:** Force logout of all Milot Motors apps and G-Suite/Microsoft accounts.
- **Credential Rotation:** Change passwords for any accounts stored on the device.

## 3. Investigation
- Determine if any unencrypted Customer PII (Names/Phone numbers) was stored locally.
- Check "Last Seen" GPS location via the management console.

## 4. Documentation
- Log the event in `incident-log.csv`.
- Complete an `incident-report.md`.
