# Awesome-Data-Detection-And-Response-DDR

## Top Data Detection and Response (DDR) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Data-Centric Threat Detection, Behavioral Analytics & Automated Exfiltration Response*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Data Detection and Response (DDR)**. These tools monitor how sensitive data is actually accessed, moved, and used across cloud, SaaS, on-premises, and endpoint environments—then trigger automated responses when behavior deviates from normal, catching insider exfiltration, compromised accounts, and ransomware staging that perimeter defenses miss.

**Examples** include Druva MDDR, Forcepoint DDR, Securiti, Normalyze, Cyera, Sentra, Varonis, BigID, Theom, and Polar Security (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted data discovery, open-source DSPM/DDR, and community-driven classification—ideal for organizations seeking data sovereignty and predictable costs over per-user or per-data-source enterprise licensing. Note that **purpose-built open-source DDR is genuinely nascent**: the search results surfaced almost no direct open-source DDR equivalents to Druva or Forcepoint, so the practical path is composing open-source DSPM (data discovery/classification) with custom behavioral detection and response automation.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Data Detection and Response (DDR) market is estimated at **$4.0B – $4.5B** in 2026 and is projected to expand to **$9.3B by 2031** at a ~15.6% CAGR, catalyzed by rapid cloud data sprawl, strict privacy mandates, and unmonitored AI agents accessing enterprise data stores. The sector is currently **moderately fragmented**: specialized DSPM/DDR innovators (such as Cyera, Sentra, and Securiti) drive rapid architectural shifts across multi-cloud and lakehouses, while legacy platform giants (IBM, Proofpoint, Cisco, and CrowdStrike) actively consolidate the space through aggressive acquisitions.

## SaaS/Hosted Platforms

*Sorted by Company Size / Valuation (Descending)*

| Product | Company Size / Valuation | Description | Pricing (Starting Tier) | Free Tier / Trial Limits |
|---|---|---|---|---|
| **[Polar Security (IBM)](https://www.ibm.com/products/guardium-insights)** | **$231B+ Market Cap** (Parent IBM; Polar acquired for ~$60M) | DSPM/DDR platform acquired by IBM and integrated into Guardium Insights. Discovers, classifies, and maps sensitive data flows across AWS, Azure, and GCP with automated policy-driven response. | Starting from **$15,000/year** (IBM Guardium SaaS baseline) | **30-day free trial** with full access to cloud data discovery connectors and policy evaluation. |
| **[Normalyze](https://www.normalyze.com/)** | **$12.3B Valuation** (Parent Proofpoint / Thoma Bravo; acquired ~$76M) | Cloud data security and DDR platform mapping sensitive data exposure, privileges, and attack paths across cloud, DBaaS, and SaaS environments. | Starting from **$1,500/month** ($18,000/year for Premium tier) | **Free Forever Tier**: 1 cloud account (AWS, Azure, or GCP), basic data risk dashboards, up to 30 days of graph history tracking (scanning capped at baseline snapshot). |
| **[Cyera](https://www.cyera.io/)** | **$12B Valuation** (Series G unicorn; ~$200M ARR) | AI-native data security platform unifying DSPM, DDR, and data access governance. Uses LLM-driven classification to detect real-time file exfiltration and anomalous access across multi-cloud and SaaS. | Starting at **$50,000/year** (AWS Marketplace Standard tier, covers up to 25 TB data capacity) | **No free tier**; interactive sandbox and custom **14-day guided Proof of Concept (PoC)** upon sales qualification. |
| **[Varonis Data Security Platform](https://www.varonis.com/)** | **$5.6B Market Cap** (NASDAQ: VRNS; ~$716M TTM Revenue) | Pioneer data security and behavior analytics platform covering cloud, SaaS, and on-premises environments. Features Managed DDR (MDDR) for proactive threat hunting and automated response. | Starting from **$50 – $95/user/year** (DSPM/SaaS baseline; managed DDR add-on +$25–$50/user/year; typical entry contract ~$15,000–$25,000/year) | **30-day Data Risk Assessment (free trial)**: Scans a designated enterprise environment (M365, AWS, or on-prem) to produce a comprehensive vulnerability and exposure report. |
| **[Druva Managed DDR (MDDR)](https://www.druva.com/)** | **$2.0B Valuation** (Private unicorn; ~$200M+ ARR) | 24/7 managed detection and response on backup repositories and SaaS data. Features **Safe Mode** to pause malicious restores, block deletions, and lock down compromised admin accounts. | Starting from **$2.50/user/month** (inSync SaaS) or **$450/TB/year** (Server Workloads on AWS Marketplace); MDDR included at no extra cost with Druva enterprise subscriptions | **30-day free trial**: Full access to configure server or SaaS workloads, backup automation, and live support (no credit card required). |
| **[Securiti](https://securiti.ai/)** | **$1.725B Valuation** (Acquired by Veeam; ~$100M+ ARR) | Unified Data Command Center delivering DDR, DSPM, privacy compliance, and LLM firewalls. Detects policy violations, unauthorized cross-border transfers, and shadow data movement. | Starting from **$50,000/year** (AWS Marketplace / modular contract baseline; ~$3,500–$5,000/month for initial suites) | **No self-serve free tier**; free access to PrivacyOps/AI Governance Academy certification courses, and custom **14-day assisted PoC** upon enterprise review. |
| **[BigID DDR](https://bigid.com/)** | **$1.0B+ Valuation** (Riverwood Capital; ~$100M ARR) | Enterprise data intelligence and DDR platform with 100+ connectors. Uses deep ML classification to track sensitive data access and trigger remediation via Microsoft Purview and SOAR tools. | Starting at **$175,000/year** (AWS Marketplace Discovery Foundation 12-month commitment) | **No free tier**; tailored **30-day enterprise Proof of Concept (PoC)** available via enterprise sales qualification. |
| **[Forcepoint DDR](https://www.forcepoint.com/)** | **~$800M Valuation** (Francisco Partners; ~$350M–$400M Revenue) | Cloud and endpoint DDR leveraging AI Mesh classification to track continuous data interactions (file reads, shares, renames, copies) and halt exfiltration across hybrid endpoints. | Starting from **$45 – $70/user/year** (Forcepoint ONE Cloud Security / DLP baseline suite) | **30-day free trial** for cloud security modules, or 14-day assisted trial through enterprise sales channel. |
| **[Sentra](https://sentra.io/)** | **~$350M – $450M Valuation** (Series C funded; tens of millions ARR) | Cloud-native DSPM and DDR platform designed to track sensitive data movement across AWS, Azure, GCP, and Snowflake, detecting rogue exfiltration channels and misconfigurations. | Starting at **$50,000/year** (AWS Marketplace Standard plan baseline) | **No free tier**; structured **14-day to 30-day guided Proof of Concept (PoC)** upon enterprise onboarding. |
| **[Theom](https://theom.ai/)** | **~$80M Valuation** (Series A; backed by Databricks, Snowflake & SentinelOne) | Data-centric DDR and posture management built specifically for cloud data warehouses and lakehouses (Snowflake, Databricks, BigQuery, AWS S3), monitoring insider risks and exfiltration queries. | Starting from **$25,000/year** (Cloud Lakehouse baseline tier) | **14-day free trial** via AWS Marketplace and direct cloud-connect demo with sample data lake audit. |

## Open-Source GitHub Projects

*Sorted by GitHub Star Count (Descending)*

| Project | Star Badge | Description |
|---|---|---|
| **[Gitleaks](https://github.com/gitleaks/gitleaks)** | [![Stars](https://img.shields.io/github/stars/gitleaks/gitleaks?style=social&color=white)](https://github.com/gitleaks/gitleaks/stargazers) | High-speed, lightweight static analysis scanner designed to detect hardcoded secrets, API tokens, passwords, and sensitive keys in git repositories, files, and CI/CD pipelines—preventing data exfiltration at commit time. |
| **[TruffleHog](https://github.com/trufflesecurity/trufflehog)** | [![Stars](https://img.shields.io/github/stars/trufflesecurity/trufflehog?style=social&color=white)](https://github.com/trufflesecurity/trufflehog/stargazers) | Secret detection and data leak scanner that analyzes git repos, file systems, and S3 buckets for exposed high-entropy secrets and sensitive tokens, verifying active keys against external service providers. |
| **[Osquery](https://github.com/osquery/osquery)** | [![Stars](https://img.shields.io/github/stars/osquery/osquery?style=social&color=white)](https://github.com/osquery/osquery/stargazers) | SQL-powered operating system instrumentation and monitoring framework. Allows security teams to query real-time process execution, file system integrity, socket connections, and sensitive file read events across endpoints. |
| **[Wazuh](https://github.com/wazuh/wazuh)** | [![Stars](https://img.shields.io/github/stars/wazuh/wazuh?style=social&color=white)](https://github.com/wazuh/wazuh/stargazers) | Comprehensive open-source SIEM and XDR security platform offering real-time file integrity monitoring (FIM), system audit logging, log analysis, and active automated response workflows across endpoints and cloud instances. |
| **[OpenMetadata](https://github.com/open-metadata/OpenMetadata)** | [![Stars](https://img.shields.io/github/stars/open-metadata/OpenMetadata?style=social&color=white)](https://github.com/open-metadata/OpenMetadata/stargazers) | Open-source metadata management platform featuring column-level data lineage, auto-classification, and data governance policies. Provides the data discovery and classification inventory required by DDR engines. |
| **[DataHub](https://github.com/datahub-project/datahub)** | [![Stars](https://img.shields.io/github/stars/datahub-project/datahub?style=social&color=white)](https://github.com/datahub-project/datahub/stargazers) | Extensible open-source data catalog and metadata platform created at LinkedIn. Delivers real-time data discovery, governance graphs, and dataset sensitivity profiling to map enterprise data landscapes. |
| **[Microsoft Presidio](https://github.com/microsoft/presidio)** | [![Stars](https://img.shields.io/github/stars/microsoft/presidio?style=social&color=white)](https://github.com/microsoft/presidio/stargazers) | Open-source context-aware PII detection, redaction, and anonymization engine from Microsoft. Uses Named Entity Recognition (NER) models and pattern analyzers to detect and mask sensitive data fields in text and document streams. |
| **[Panther Analysis](https://github.com/panther-labs/panther-analysis)** | [![Stars](https://img.shields.io/github/stars/panther-labs/panther-analysis?style=social&color=white)](https://github.com/panther-labs/panther-analysis/stargazers) | Open-source repository of detection-as-code rules, audit policies, and automated response scripts for cloud data platforms (AWS CloudTrail, Snowflake, Okta, Box) to detect anomalous data access and exfiltration in real time. |
| **[OpenCSPM](https://github.com/OpenCSPM/opencspm)** | [![Stars](https://img.shields.io/github/stars/OpenCSPM/opencspm?style=social&color=white)](https://github.com/OpenCSPM/opencspm/stargazers) | Open-source Cloud Security Posture Management engine providing a graph-based inventory of cloud assets, access control permissions, and exposed data stores across multi-cloud environments. |
| **[Privacy Firewall](https://github.com/privacyshield-ai/privacy-firewall)** | [![Stars](https://img.shields.io/github/stars/privacyshield-ai/privacy-firewall?style=social&color=white)](https://github.com/privacyshield-ai/privacy-firewall/stargazers) | Open-source client-side DLP tool that runs local AI models to inspect, detect, and intercept sensitive enterprise data or credentials before they are pasted into external LLM interfaces (like ChatGPT or Claude). |
| **[hitsz-ids/openDLP](https://github.com/hitsz-ids/openDLP)** | [![Stars](https://img.shields.io/github/stars/hitsz-ids/openDLP?style=social&color=white)](https://github.com/hitsz-ids/openDLP/stargazers) | Open-source sensitive data identification tool utilizing regular expressions, NLP classification, and verification rules to perform automated field-level sensitivity tagging across structured databases and JSON data. |

**Frameworks for building custom systems**: The open-source DDR path is **discovery + catalog + custom detection + response automation**. Use **Microsoft Presidio** or **hitsz-ids/openDLP** for sensitive data discovery, **OpenMetadata** or **DataHub** for the inventory of what is sensitive and where it lives, **Osquery** and cloud audit logs for real-time access telemetry, and **Wazuh** or **Panther Analysis** for behavioral detection and automated incident containment.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- DDR platforms monitor sensitive data access and user behavior; enforce privacy controls, audit logging, and compliance with applicable regulations (GDPR, CCPA, sector-specific mandates) when monitoring employee activity.
- **Open-source DDR does not exist as a single monolithic turnkey product.** The practical open-source path is assembling discovery/classification engines (Presidio, OpenMetadata), runtime system/cloud log monitors (Osquery, CloudTrail), and detection-as-code automation engines (Wazuh, Panther Analysis). Commercial DDR pricing features multi-tier subscriptions and AWS Marketplace private offers, with introductory starting tiers scaling based on data volume, user count, or cloud accounts.

---

**Made for security engineers, data protection officers, SOC analysts, and developers building data-centric detection infrastructure.**  
Let's make data detection and response more open, explainable, and actionable.
