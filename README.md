# Awesome-Data-Detection-And-Response-DDR

# Top Data Detection and Response (DDR) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Data-Centric Threat Detection, Behavioral Analytics & Automated Exfiltration Response*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Data Detection and Response (DDR)**. These tools monitor how sensitive data is actually accessed, moved, and used across cloud, SaaS, on-premises, and endpoint environments—then trigger automated responses when behavior deviates from normal, catching insider exfiltration, compromised accounts, and ransomware staging that perimeter defenses miss.

**Examples** include Druva MDDR, Forcepoint DDR, Securiti, Normalyze, Cyera, Sentra, Varonis, BigID, Theom, and Polar Security (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted data discovery, open-source DSPM/DDR, and community-driven classification—ideal for organizations seeking data sovereignty and predictable costs over per-user or per-data-source enterprise licensing. Note that **purpose-built open-source DDR is genuinely nascent**: the search results surfaced almost no direct open-source DDR equivalents to Druva or Forcepoint, so the practical path is composing open-source DSPM (data discovery/classification) with custom behavioral detection and response automation.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Druva Managed DDR (MDDR)](https://www.druva.com/)** | Managed 24/7 monitoring of backups for threat indicators (snapshot deletion, backup set deletion, admin deletion of users/devices), with expert analysis by Druva Incident Response. **Safe Mode** provides an instant "emergency brake" to pause restores, restrict admin access, stop backups, and block deletions during an active threat. MDDR is available to Druva customers at no additional charge . | Included with Druva subscription (no extra charge for MDDR)  | No standalone free tier; MDDR included with Druva backup subscription. Not available for GovCloud or SFDC customers . |
| **[Forcepoint DDR](https://www.forcepoint.com/)** | AI-powered Data Detection and Response for cloud and endpoint. Uses **AI Mesh** classification to detect file activity (reads, shares, renames, movement) and surface prioritized, explainable alerts with remediation steps. Integrates with Forcepoint DSPM for posture context. Mindshare in DDR category: ~7–10% (Sept 2026) . | Quote-only (enterprise contract) | No free tier; demo via sales |
| **[Securiti](https://securiti.ai/)** | **Ranked #1 in Data Detection & Response** with 20–25% mindshare (PeerSpot, 2026). Unified Data Command Center covering data security, privacy, governance, and AI safety. Automated sensitive data discovery, classification, consent management, and zero trust architecture. Users note occasional slowness in large environments . | Quote-only (enterprise contract) | No free tier; demo via sales |
| **[Normalyze](https://www.normalyze.com/)** | DSPM/DDR platform focused on data security posture across cloud and SaaS. Identifies sensitive data exposure and prioritizes risk based on data sensitivity and access context. | Quote-only | No free tier; demo via sales |
| **[Cyera](https://www.cyera.io/)** | AI-native data security platform covering DSPM, DDR, and data governance. Uses LLM-based classification for high accuracy across structured and unstructured data. | Quote-only | No free tier; demo via sales |
| **[Sentra](https://sentra.io/)** | Cloud data security platform with DSPM and DDR capabilities. Focuses on discovering and classifying sensitive data across cloud environments with automated remediation workflows. | Quote-only | No free tier; demo via sales |
| **[Varonis Data Security Platform](https://www.varonis.com/)** | Long-established data security platform covering data discovery, classification, behavior analytics, and threat detection. Strong on-premises and file share heritage, expanding to SaaS and cloud. | Quote-only (per-data-source or per-user) | No free tier; demo via sales |
| **[BigID DDR](https://bigid.com/)** | Data intelligence platform with DDR capabilities. Strong on data discovery, classification, and privacy compliance across 100+ data sources. Integrates with Microsoft Purview Information Protection . | Enterprise quote-only; Marketplace listings show $525,000+ for Foundation packages (from prior research) | No free tier; demo via sales |
| **[Theom](https://theom.ai/)** | Data security posture and DDR focused on cloud data stores. Detects risky access patterns and enforces policies based on data sensitivity. | Quote-only | No free tier; demo via sales |
| **[Polar Security (IBM)](https://www.ibm.com/)** | DSPM/DDR platform acquired by IBM. Focused on discovering and classifying sensitive data across cloud environments with policy-driven protection. | Quote-only (IBM enterprise contract) | No free tier; demo via sales |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[OpenDLP](https://github.com/ezra100/OpenDLP)** | [![Stars](https://img.shields.io/github/stars/ezra100/OpenDLP?style=social&color=white)](https://github.com/ezra100/OpenDLP/stargazers) | **The closest open-source building block for DDR's discovery layer.** Open-source data loss prevention scanner that identifies sensitive data (credit cards, SSNs, PII) across file shares and databases. Can be adapted to scan contract repositories and cloud storage for sensitive content exposure—the "discovery and classification" phase that precedes DDR detection. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[OpenMetadata](https://github.com/open-metadata/OpenMetadata)** | [![Stars](https://img.shields.io/github/stars/open-metadata/OpenMetadata?style=social&color=white)](https://github.com/open-metadata/OpenMetadata/stargazers) | Open-source metadata platform with **column-level lineage, classification, and data contracts**. Provides the data inventory and sensitivity labels that DDR detection would consume. **Not DDR**—it is the catalog that tells you where sensitive data lives, not who is exfiltrating it right now . |
| **[DataHub](https://github.com/datahub-project/datahub)** | [![Stars](https://img.shields.io/github/stars/datahub-project/datahub?style=social&color=white)](https://github.com/datahub-project/datahub/stargazers) | Open-source metadata platform with search, lineage, and governance. Same caveat as OpenMetadata: catalog, not detection-and-response . |

**Frameworks for building custom systems**: The open-source DDR path is **discovery + catalog + custom detection + response automation**. Use **OpenDLP** (or equivalent scanners) for sensitive data discovery, **OpenMetadata** or **DataHub** for the inventory of what is sensitive and where it lives, then build behavioral detection on top by analyzing cloud access logs (CloudTrail, Azure Activity Logs, GCP Audit Logs) for anomalies—bulk downloads, unusual access times, permission changes. Response automation can be wired through n8n or a SOAR platform. **This is not a turnkey DDR product**; it is a DIY assembly that requires significant engineering.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- DDR platforms monitor sensitive data access and user behavior; enforce privacy controls, audit logging, and compliance with applicable regulations (GDPR, CCPA, sector-specific mandates) when monitoring employee activity.
- **Open-source DDR does not exist as a mature, turnkey category.** The search results surfaced no direct open-source equivalents to Druva MDDR, Forcepoint DDR, or Securiti. The practical open-source path is assembling DSPM/discovery tools (OpenDLP, OpenMetadata) with custom behavioral detection and response automation—significant engineering effort. **Commercial DDR pricing is almost universally quote-only** with no public list rates. Druva MDDR is notable for being **included at no additional charge** with Druva backup subscriptions, making it the most accessible entry point for existing Druva customers . Forcepoint and Securiti are enterprise contracts with no free tiers.

---

**Made for security engineers, data protection officers, SOC analysts, and developers building data-centric detection infrastructure.**  
Let's make data detection and response more open, explainable, and actionable.
