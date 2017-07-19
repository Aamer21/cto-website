---
title: DevSecOps Guide
category: DevOps
---

### Standard DevSecOps Platform Framework
Goal: Safer Software Sooner

The following document describes, at a high-level, the expectations, scope of responsibilities, maturity model, and metrics associated of any DevSecOps platform at GSA.

#### Baseline Definitions
**DevSecOps:** A cultural and engineering practice that breaks down barriers and opens collaboration between development, security, and operations organizations using automation to focus on rapid, frequent delivery of secure infrastructure and software to production. It encompasses intake to release of software and manages those flows predictably, transparently, and with minimal human intervention/effort.

Patch management is the process by which the operating system, software, and supporting services are upgraded. This is a key element of maintaining the security of systems.
Maturity Model
Level 1 (Not considered viable for a DevSecOps platform): Patching is both manual and is not enforceable as a requirement nor is the state of patches running machines discoverable
Level 2: Security teams inform the application owners of patches, and it is application owners’ responsibility to both be aware of those patches and implement them.
Level 3: Application owners are automatically notified when there are new security-related patches, and the platform owners are able to identify which applications are using which version of the relevant software via the platform.
Level 4: The platform automatically tests new patches on applications which run on it, informing the appropriate parties if decision points are reached (e.g., if a CVE is raised on an existing piece of software, the platform can automatically update that software, test it, and inform the application developers of the change if the tests pass or indicate that the patch needs to be applied in a particular timeframe). No downtime for patching.
Artifacts
Process (code, checklist or SOP) for patching a running system
Process (code, checklist or SOP) for introducing a patch into the platform [Note: This may overlap with image management]
