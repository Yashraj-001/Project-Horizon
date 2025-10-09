Project Horizon
Open-Source Zero Trust Security & Operations Framework
🔭 1. Vision

Project Horizon is my independent research initiative to design and implement a unified Zero Trust security architecture entirely with open-source and free-tier technologies.
The project explores how a modular, cloud-agnostic security ecosystem can deliver end-to-end protection, observability, and automation across identity, data, infrastructure, and analytics layers — without relying on commercial platforms.

Aether represents a personal vision:

“To demonstrate that enterprise-grade security can be achieved through thoughtful architecture, community-driven tools, and deep technical integration.”

🧭 2. Inspiration from Enterprise Requirements

The initial inspiration came from a real-world enterprise brief (Getir 2025) that outlined the need for a Next-Generation AI-Driven Security & Operations Platform.
Those requirements were reinterpreted as the following research goals for Aether:

Original Requirement	Reframed Research Objective
XDR & Insider Risk Management	Build an open-source detection and response system with UEBA and automation (Elastic + Tines).
SASE / ZTNA Architecture	Enforce identity-aware, TLS-secured access using Keycloak + Pomerium + pfSense/Suricata.
CNAPP for Cloud-Native Workloads	Protect the container lifecycle with Falco, Kyverno, Trivy, Cosign, Checkov, ELK.
AI-Driven Customer Data Platform	Simulate customer engagement and churn prediction via PostgreSQL, Python, Mailgun, ELK.
Data Security Posture Management	Discover, classify, and remediate sensitive data with MinIO, NiFi, Presidio, Custodian.

Rather than fulfilling a commercial contract, the aim was to prototype these enterprise-class capabilities through self-driven design and experimentation.

⚙️ 3. Approach & Methodology

The project followed a solution-oriented, phased methodology:

Modular Design First: Each pillar (ZTNA, CNAPP, DSPM, CDP, XDR) was built independently in a controlled lab VM environment.

Open-Source Toolchain: Every component was chosen from the open-source ecosystem to ensure transparency and reproducibility.

Iterative Integration: Once validated, all modules were unified under a centralized ELK telemetry layer.

Detection Engineering: Correlation and rule creation were performed in Elastic SIEM with enrichment and automated response through Tines.

Documentation & Evidence: Each module was fully documented with configurations, dashboards, and technical reports.

This approach ensured that every subsystem could stand alone yet contribute to a cohesive Zero Trust ecosystem.

🧩 4. Solution Architecture
4.1 Zero Trust Network Access (ZTNA)

Tools: Keycloak (IdP), Pomerium (reverse proxy), pfSense + Suricata (IDS/IPS)

Outcome: Identity-based, TLS-secured application access with full authentication telemetry in ELK.

4.2 Cloud-Native Application Protection Platform (CNAPP)

Tools: Checkov, Trivy, Cosign, Kyverno, Falco, Falcosidekick, ELK

Outcome: Secured the container lifecycle — IaC scan → image sign → runtime detect → log visualize.

4.3 Data Security Posture Management (DSPM)

Tools: MinIO, Apache NiFi, Microsoft Presidio, Cloud Custodian, PostgreSQL, ELK

Outcome: Sensitive-data discovery, automatic remediation of exposed buckets, compliance dashboards.

4.4 Customer Data Platform (CDP)

Tools: PostgreSQL, Python services, Mailgun SMTP, ELK

Outcome: Synthetic user-activity simulation, churn-risk scoring, alert-driven campaigns, full observability.

4.5 Extended Detection & Response (XDR + Insider Risk)

Tools: Elastic Stack, Suricata, Pomerium, DSPM feeds, UEBA (Isolation Forest), Tines

Outcome: Centralized telemetry, rule-based detections, ML-driven SSH anomaly detection, automated response.

🚀 5. Implementation Highlights

End-to-end Zero Trust access flow validated via Keycloak → Pomerium → Application with ELK visibility.

CNAPP successfully blocked unsigned images and detected runtime intrusions on K3s.

DSPM pipeline achieved automated policy remediation and real-time entity classification.

CDP pipeline executed churn scoring → alert → campaign → dashboard cycle using synthetic data.

XDR / UEBA correlated events across all layers and triggered Tines playbooks for enrichment and host isolation.

Unified Kibana dashboards provided full visibility and cross-domain correlation.

Each subsystem was independently deployed, integrated, and validated within a controlled, single-node lab setup.

🧠 6. Outcomes & Learnings

Demonstrated a fully functional Zero Trust prototype using 100 % open-source components.

Proved that enterprise-grade detection and response can be achieved through modular integration.

Built a scalable architecture blueprint adaptable to any cloud or hybrid environment.

Strengthened personal expertise in DevSecOps, SOC engineering, data protection, and automation.

🔮 7. Future Roadmap

Scale to Kubernetes Clusters: Introduce multi-node clustering and CI/CD automation.

Enhance Policy Depth: Expand Kyverno and Custodian rules for RBAC and governance.

Advanced Correlation: Implement cross-source risk scoring and threat graph analytics.

Identity Federation: Integrate Azure AD / Okta for production-grade SSO and MFA.

Expanded UEBA: Extend anomaly detection beyond SSH to email and SaaS usage.

Research Publication: Convert findings into a whitepaper on “Open-Source Zero Trust Security Architectures.”

⚖️ 8. Disclosure & Acknowledgment

This repository presents Project Aether as a personal open-source research project.
While the initial concept was inspired by a corporate problem statement, all design decisions, implementations, and documentation were developed independently using publicly available open-source resources.
No proprietary code, data, or confidential information is included.
