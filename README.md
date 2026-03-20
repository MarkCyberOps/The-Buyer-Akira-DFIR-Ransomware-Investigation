# The Buyer – DFIR Ransomware Investigation

## Overview

This repository documents a full digital forensics and incident response (DFIR) investigation involving a ransomware attack attributed to an Akira affiliate.

The attacker re-entered the environment using pre-staged access and executed a multi-stage intrusion involving credential theft, lateral movement, data exfiltration, and ransomware deployment.

---

## Scenario Overview

![Scenario](screenshots/01-scenario-overview.png)

---

## Ransom Note Evidence

![Ransom Note](screenshots/02-ransom-note.png)

---

## Encrypted Environment

![Encrypted Files](screenshots/03-encrypted-files.png)

---

## Objectives

- Identify initial access vector
- Track attacker activity across endpoints
- Detect credential access and lateral movement
- Analyze command and control behavior
- Investigate data exfiltration
- Identify ransomware execution
- Determine scope of compromise

---

## Environment

- Platform: Microsoft Defender for Endpoint (MDE)
- Query Language: KQL
- Hosts:
  - as-pc2
  - as-srv

---

## Compromised Hosts
