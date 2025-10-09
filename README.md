# 🌌 Project Horizon
### *An Open-Source Zero Trust Security & Operations Framework*

---

## 📖 Overview

**Project Horizon** is an independently developed research initiative demonstrating how **enterprise-grade Zero Trust Architecture (ZTA)** can be implemented using **only open-source and free-tier tools**.

It unifies **five critical security domains** — `ZTNA`, `CNAPP`, `DSPM`, `CDP`, and `XDR/UEBA` — into a single, integrated ecosystem.

Each subsystem was designed, implemented, and validated in a controlled lab environment to replicate **production-grade security** functions without proprietary software.

---

## 🎯 Project Vision

> *“Project Horizon represents my personal vision of unifying open-source security tools into a self-sustaining, AI-ready Zero Trust platform.”*

The project aims to build a **modular**, **transparent**, and **scalable** Zero Trust ecosystem capable of:

- 🔒 Enforcing **identity-aware access** for every request  
- 👁️ Providing **continuous visibility and detection** across workloads, networks, and data flows  
- ⚙️ Enabling **policy-driven governance** for data, identity, and infrastructure  
- 💡 Proving that open-source can achieve **enterprise-grade security outcomes**

---

## 🧩 Research Inspiration

The initiative originated from enterprise Zero Trust modernization requirements.  
Rather than building a vendor solution, **Horizon** reimagines those needs through open-source implementations.

| **Enterprise Challenge** | **Horizon Implementation** |
|---------------------------|-----------------------------|
| Unified Zero Trust & Secure Access | **Keycloak (IdP)** + **Pomerium (ZTNA Proxy)** + **pfSense / Suricata (Network Enforcement)** |
| Cloud-Native Security & Runtime Visibility | **Falco**, **Kyverno**, **Trivy**, **Checkov**, **Cosign** on **K3s cluster** |
| Data Security & Compliance Automation | **MinIO**, **NiFi**, **Presidio**, **Cloud Custodian** |
| Customer Intelligence & Campaign Orchestration | **PostgreSQL**, **Python**, **Mailgun**, **ELK Stack** |
| Extended Detection & Automated Response | **Elastic Stack**, **UEBA (Isolation Forest)**, **Tines SOAR** |

---

## ⚙️ Implementation Highlights

### 🔐 Zero Trust Network Access (ZTNA)
- Identity federation via **Keycloak (OIDC)** and **Pomerium** policy enforcement  
- Full **TLS pipeline** with inspection through **pfSense + Suricata**  
- Centralized authentication telemetry in **ELK Stack** for behavioral visibility  

### ☁️ Cloud-Native Application Protection (CNAPP)
- Automated IaC scanning with **Checkov**, image signing via **Cosign**, and runtime detection using **Falco**  
- **Kyverno** enforces Kubernetes policies; **Trivy** manages vulnerability tracking  
- Dashboards display vulnerabilities, policy violations, and runtime anomalies  

### 🔎 Data Security Posture Management (DSPM)
- Sensitive data discovery using **Presidio** and ingestion through **NiFi**  
- Automated remediation via **Cloud Custodian** on **MinIO** buckets  
- Compliance dashboards visualize entity exposure and trend analytics  

### 📊 Customer Data Platform (CDP)
- Synthetic behavior simulation with **Python microservices** and **PostgreSQL**  
- Churn scoring and campaign automation using **Mailgun SMTP**  
- **ELK dashboards** provide insights into engagement and churn metrics  

### 🧠 XDR & Insider Risk (UEBA + SOAR)
- Unified telemetry from all modules in **Elastic SIEM**  
- Custom **UEBA engine** using *Isolation Forest* for SSH anomaly detection  
- **Tines automation workflows** for enrichment, alerting, and host isolation  

---

## 🏆 Key Achievements

✅ End-to-end **Zero Trust access validation** (Keycloak → Pomerium → Application)  
✅ Complete **container security chain** (IaC → Build → Runtime → Detect)  
✅ **Sensitive data discovery** and **automated remediation** with Custodian  
✅ Simulated **data analytics pipeline** for engagement insights  
✅ **Cross-domain detection engineering** in Elastic SIEM with UEBA scoring  
✅ **SOAR automation** reducing manual SOC intervention time  

---

## 📈 Research Outcomes

| **Dimension** | **Result** |
|----------------|------------|
| **Architecture** | Unified Zero Trust prototype spanning five core security domains |
| **Scalability** | Modular, tool-agnostic, extensible design validated in multi-VM lab |
| **Visibility** | 100% log integration into Elastic Stack; dashboards for every module |
| **Automation** | Real-time enrichment and containment via Tines workflows |
| **Learning Value** | Deep hands-on expertise in DevSecOps, detection engineering, and SOAR |

---

## 🚀 Future Enhancements

- Transition to **multi-node Kubernetes** deployment with CI/CD integration  
- Expand **policy coverage** for RBAC, PSP, and data residency  
- Implement **cross-source correlation** for dynamic risk scoring  
- Integrate **Azure AD / Okta federation** for enterprise identity management  
- Extend **UEBA** to SaaS, email, and privileged activity analytics  
- Publish as a **technical whitepaper** on open-source Zero Trust frameworks  

---

## 🧰 Technology Stack

`Keycloak` • `Pomerium` • `pfSense` • `Suricata` • `Falco` • `Kyverno` • `Trivy` • `Checkov` • `Cosign`  
`MinIO` • `NiFi` • `Presidio` • `Cloud Custodian` • `PostgreSQL` • `Mailgun` • `Elastic Stack` • `Tines`

---

## 🧑‍💻 Author

**Yogendra Jain**  
Cybersecurity Analyst & Researcher — Zero Trust, SOC, and Threat Detection Engineering  

---

## ⭐ Support the Project

If you find this project insightful or useful, please consider:
- 🌟 Starring the repository  
- 🧩 Contributing to future research modules  
- 🗣️ Sharing feedback or feature ideas  

---

> *“Security is not about products — it’s about principles, discipline, and visibility.”*
