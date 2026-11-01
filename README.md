# Awesome-Managed-Identity-Threat-Protection

# Top Managed Identity Threat Protection Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on 24/7 Managed ITDR, Identity Attack Surface Reduction & Self-Hosted Identity Threat Detection*  
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Managed Identity Threat Protection**. These services and tools enable organizations to detect and respond to identity-based attacks—credential theft, privilege escalation, lateral movement, and MFA manipulation—before adversaries can establish persistence or reach critical systems.

**Examples** include CrowdStrike Falcon Complete Identity Threat Protection, Silverfort, Semperis, Arctic Wolf, Expel, Vectra AI, Red Canary, Sophos, BeyondTrust, and CyberArk (the category leaders).

**Open-source emphasis**: Managed Identity Threat Protection is a domain where the **"managed" component is fundamentally a human service**—24/7 monitoring by expert analysts who investigate and remediate identity threats on your behalf. No open-source project replicates that service. What open-source *does* provide is **tooling for identity threat detection and response (ITDR) that organizations can run themselves**: **Authomize's OpenITDR** framework provides an open API standard and community connectors for pulling identity context and building automated remediation workflows , **ThreatFlix** demonstrates an explainable identity-threat investigation system (though it is a student/research-grade demo) , and **M365IdentityPosture** provides read-only PowerShell reporting for Microsoft 365 identity posture assessment . The critical caveat: **open-source gives you the tools, not the team**—managed ITDR is a service delivered by human analysts, and organizations without dedicated identity security staff should evaluate MDR/MITDR providers rather than attempting to self-manage with open-source tools alone.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[CrowdStrike Falcon Complete Identity Threat Protection](https://www.crowdstrike.com/)**  
  The **first fully managed identity protection solution**; combines Falcon Identity Threat Protection technology with the Falcon Complete team's expertise—managing, monitoring, and surgically remediating identity incidents in minutes . Use cases include shrinking the attack surface with tightly tuned policies (blocking unauthorized admin logins, forcing MFA for RDP to critical servers) and stopping identity-driven attacks in real time via countermeasures like blocking authentication with stolen credentials or issuing MFA challenges . **Best for organizations wanting fully managed ITDR** without building an internal identity security program.

- **[Silverfort](https://www.silverfort.com/)**  
  Identity security platform with **patented Runtime Access Protection (RAP)** technology that integrates natively with IAM infrastructure (e.g., Active Directory) to enforce controls at runtime—stopping threats before authentication completes . Features: **Identity Graph & Inventory**, **Authentication Firewall** for identity-based segmentation, **ISPM**, **Access Intelligence**, **NHI Security**, and **ITDR** for real-time detection of credential misuse, lateral movement, and privilege escalation . Integrates with CyberArk PAM to extend protection to unmanaged privileged accounts without additional onboarding . **Best for organizations wanting inline, real-time identity threat prevention** without replacing existing IAM.

- **[Semperis](https://www.semperis.com/)**  
  Identity-driven cyber resilience and crisis management company; protects **Active Directory, Entra ID, Ping Identity, and Okta** environments . AI-powered platform unifies identity lifecycle defense and crisis management—hardening identity infrastructure, detecting and containing active threats, enabling rapid trusted recovery, and supporting secure out-of-band coordination during incidents . **Free community tools**: Purple Knight and Forest Druid for identity security assessment . Trusted by over **1,000 organizations** including **25%+ of the 100 largest U.S. companies** . **Best for organizations needing identity-focused resilience and recovery** alongside threat detection.

- **[Arctic Wolf](https://arcticwolf.com/)**  
  Managed detection and response with **identity threat detection and response (ITDR)** capabilities; monitors Active Directory, IAM solutions, and endpoint telemetry, correlating identity detections with other domains (endpoint, network, cloud) for faster, more accurate attack identification . **Concierge Security Team** provides proactive hardening, identity posture analysis, and lifecycle identity management; SOC monitors 24/7 . **Managed Risk** detects software defects, system misconfigurations, and credential exposure . **Best for organizations wanting managed ITDR integrated with broader MDR**.

- **[Expel](https://expel.com/)**  
  MDR with **ITDR capabilities** monitoring Okta, Azure AD (Entra ID), Duo, and Ping Identity for credential compromise, privilege abuse, and MFA manipulation . **Ruxie** applies agentic AI, machine learning, and structured reasoning to identity alerts—auto-closing benign noise and returning verdicts with full evidence in **under 30 seconds** . Detects MFA fatigue attacks by monitoring anomalous push volumes and can automatically suspend accounts . **Best for organizations wanting fast, AI-augmented identity threat detection** with transparent evidence.

- **[Vectra AI](https://www.vectra.ai/)**  
  AI-driven hybrid cloud threat detection and response covering **public cloud, SaaS, identity, and network infrastructure** . **Attack Signal Intelligence** correlates attacker TTPs rather than simply alerting on anomalies, enabling prioritization of the most urgent threats . Named a **Leader in Gartner Magic Quadrant 2025 for Network Detection and Response (NDR)** . **Best for organizations wanting identity threat detection integrated with network and cloud security**.

- **[Red Canary](https://redcanary.com/)**  
  MDR with identity and cloud threat protection; **customer-validated 99% threat accuracy** . Q3 FY25 innovations: **GenAI agent flows** achieving **60%+ faster mean time to investigate**; **Security Data Lake** for long-term retention and MDR enhancement; and **Managed XSIAM** bringing Red Canary analytics into Palo Alto Cortex XSIAM . **Best for organizations wanting high-accuracy MDR** across identities, endpoints, and cloud.

- **[Sophos](https://www.sophos.com/)**  
  MDR with **Sophos ITDR** add-on (GA October 2025); enables analysts to identify identity security gaps, detect and respond to sophisticated identity threats, and monitor dark web for exposed credentials . When used with **Sophos MDR**, analysts investigate and respond to identity threats on the customer's behalf . **Integrations included at no additional charge** with MDR/XDR subscriptions . **Best for Sophos MDR customers** wanting identity threat coverage without additional integration licensing.

- **[BeyondTrust](https://www.beyondtrust.com/)**  
  Identity security platform fusing **PAM, ITDR, CIEM, and remote support** into one AI-driven system (Pathfinder Platform) . Acquired **Entitle** (2026) to add **Just-in-Time (JIT) access, modern IGA, and CIEM** across cloud environments—addressing the shift from standing privileges to zero standing privilege . **Best for organizations wanting PAM-centric identity security** with JIT access governance.

- **[CyberArk](https://www.cyberark.com/)**  
  Identity security platform protecting human and machine identities with **PAM, IGA, and IAM** unified . **MSP Hub** (2025) provides SaaS-based multi-tenant management for service providers delivering CyberArk identity security services . **Best for organizations wanting the broadest identity security portfolio** with managed service provider options.

## Open-Source GitHub Projects

### Identity Threat Detection & Response (ITDR) Frameworks

- **[Authomize OpenITDR](https://github.com/authomize/Open-ITDR)**  
  An **open framework for the ITDR community** (Authomize) . Provides: **OpenITDR Query API** for pulling identity context; **community connectors** for data ingestion from SaaS, IaaS, and on-premises sources; **automated workflows/playbooks** for remediation (e.g., protecting compromised Okta users, remediating over-privilege in AWS, eliminating exposed Git repositories) ; and **security research tools** including **PassBleed** for detecting risky Okta misconfigurations . **Best for organizations building custom ITDR pipelines** or wanting to integrate identity context into existing security tools—but it is a framework and connector library, not a managed service.

- **[ThreatFlix](https://github.com/scienstien/threatFlix)**  
  An **explainable identity-threat investigation system** (student/research-grade demo, not a hosted product) . Architecture separates **authority from assistance**: a deterministic investigation engine provides evidence and attack chains; UEBA ensemble refines risk scores; graph similarity finds earlier incidents with similar structure; a local LLM explains cases without changing evidence . Features: topology explorer showing attack progression (failed login → success → MFA disabled → privilege change → persistence → export), raw telemetry as ground truth, and analyst chat grounded in frozen incident context . **Best for researchers and security engineers** wanting an architecture reference for explainable identity threat investigation—**not production-ready** .

### Identity Posture Assessment (Microsoft 365)

- **[M365IdentityPosture](https://github.com/Noble-Efffeciency13/M365IdentityPosture)**  
  A **PowerShell security reporting framework** for Microsoft 365 identity posture assessment (read-only, safe for production) . Reports: **Authentication Context Inventory** (security policy enforcement analysis) and **Access Package Documentor** (access governance and delegation workflows) . Analyzes PIM, Conditional Access, risky users/sign-ins, password health, and authentication methods . **Best for Microsoft 365 administrators** wanting identity posture visibility without commercial tooling—but it is a reporting module, not a managed detection service.

### Additional Strong Open-Source Options

- **crm-lead-management-app-react-native** — **Not an ITDR tool**; listed only to clarify that no mature open-source Managed ITDR platform exists. The open-source ecosystem provides frameworks (OpenITDR), research demos (ThreatFlix), and posture reporting (M365IdentityPosture)—not the 24/7 human-led detection and response that defines managed ITDR.

**Frameworks for building custom systems**: For **building custom ITDR pipelines with open connectors and remediation playbooks**, Authomize OpenITDR provides the most complete framework . For **identity posture assessment in Microsoft 365**, M365IdentityPosture provides read-only reporting . For **research into explainable identity threat investigation**, ThreatFlix demonstrates the architecture (not production) . **No open-source project provides managed identity threat protection**—that is a human service. Organizations requiring 24/7 ITDR should evaluate CrowdStrike Falcon Complete ITP, Silverfort, Semperis, Arctic Wolf, or Expel rather than attempting to self-manage with open-source tools alone.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Managed identity threat protection platforms handling identity telemetry must comply with organizational security policies and privacy regulations; **self-hosted ITDR frameworks require skilled operators**—OpenITDR and ThreatFlix are powerful starting points but demand identity security expertise to configure and interpret.
- **Open-source cannot replicate managed identity threat protection**—managed ITDR is a service delivered by human analysts 24/7 (CrowdStrike Falcon Complete ITP, Arctic Wolf Concierge Security Team, Expel SOC) . Open-source provides **frameworks (OpenITDR), research demos (ThreatFlix), and posture reporting (M365IdentityPosture)** —not the human expertise and continuous monitoring that define managed ITDR. Organizations without dedicated identity security staff should evaluate MDR/MITDR providers.
- Verify license terms for commercial use; Authomize OpenITDR is open-source (check repository) , ThreatFlix is a student project (check repository) , and M365IdentityPosture is a PowerShell module (check repository) .

---

**Made for identity security architects, SOC analysts, and organizations choosing their managed identity threat protection strategy.**  
Let's make identity threat protection more open at the framework and posture layer, but with clear eyes about the human expertise and 24/7 monitoring that managed services uniquely provide.
