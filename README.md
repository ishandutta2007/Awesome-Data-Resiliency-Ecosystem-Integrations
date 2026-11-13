# Awesome-Data-Resiliency-Ecosystem-Integrations

## Top Data Resiliency Ecosystem & Integrations

**Curated List of SaaS Marketplaces & Open-Source Integration Platforms**  
*Focused on Backup Orchestration, Security Automation & Cross-Platform Data Protection Connectors*  
**Last updated: March 2026**

This repository tracks notable **SaaS marketplaces** and **open-source projects** for **Data Resiliency Ecosystem & Integrations**. These platforms connect backup, disaster recovery, and cyber-resilience tools to the broader IT stack—SIEM, SOAR, ITSM, identity providers, and cloud services—so recovery workflows trigger automatically, alerts route to the right teams, and evidence lands where auditors expect it.

**Examples** include Druva Marketplace, ServiceNow Store, Salesforce AppExchange, AWS Marketplace, Microsoft Azure Marketplace, Google Cloud Marketplace, Splunkbase, Datadog Marketplace, Atlassian Marketplace, and Okta Integration Network (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted integration runtimes, open-source iPaaS, and community-driven connector frameworks—ideal for organizations seeking transparent, composable data protection pipelines without per-connector or per-task SaaS fees. Note that **purpose-built open-source marketplace equivalents do not exist**: the practical path is composing open-source integration runtimes (Apache Camel, n8n) with custom connectors for backup platforms.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Druva Marketplace](https://developer.druva.com/page/partner-integrations)** | Central integration hub for the Druva Data Security Cloud. Bridges Druva with security, identity, IT operations, SaaS ops, and eDiscovery tools via pre-built integrations, REST APIs, and webhooks. Partner integrations include ServiceNow (ticket creation from failed backups), Splunk, Microsoft Sentinel, CrowdStrike, Palo Alto XSOAR, Okta, Azure AD, and Slack webhooks for notifications [citation:1][citation:12]. | Included with Druva subscription (no extra charge for marketplace access) | No standalone free tier; integrations bundled with Druva platform |
| **[ServiceNow Store](https://www.servicenow.com/)** | Marketplace for free and paid certified apps and integrations built on the Now Platform. All apps are **certified for compatibility, security, and performance** through rigorous review. Trials available for 90 days on sub-production instances only; paid apps may require credit card or purchase order [citation:2]. | App prices set by partners (free to enterprise) | **90-day trial** for apps (sub-production instances only); no permanent free tier for paid apps |
| **[Salesforce AppExchange](https://appexchange.salesforce.com/)** | Enterprise cloud marketplace with thousands of apps extending Salesforce. Platform Plus subscription enables AppExchange access for building and distributing apps [citation:3][citation:14]. | App prices set by publishers; Platform Plus ~$100/user/month [citation:3] | Free to browse; paid apps priced individually |
| **[AWS Marketplace](https://aws.amazon.com/marketplace)** | Digital catalog for software, SaaS, and professional services. Supports multiple pricing models: **annual subscriptions (up to 40% savings vs. hourly)**, usage-based (users, hosts, bandwidth, data), contract pricing (1–36 months), and BYOL. AWS handles billing and disbursement [citation:4][citation:15]. | Variable by product; AWS bills to existing AWS invoice | **Free trials** available for many products; no permanent free tier for paid software |
| **[Microsoft Azure Marketplace](https://azuremarketplace.microsoft.com/)** | Commercial marketplace for Azure software and services. Microsoft charges a **3% standard store service fee** on transacted offers. SaaS subscriptions can be flat-rate or per-user; Azure infrastructure costs billed directly to publisher [citation:5]. | Variable by product; 3% Microsoft transaction fee | Free trials available for many offers |
| **[Google Cloud Marketplace](https://cloud.google.com/marketplace)** | Marketplace for SaaS and infrastructure products on Google Cloud. Pricing models include **flat monthly/annual subscriptions, usage-based, or combined subscription + usage**. Usage fees linked to auto-created Google Cloud projects [citation:6]. | Variable by product | Free trials available for many products |
| **[Splunkbase](https://splunkbase.splunk.com/)** | App marketplace for Splunk. Apps range from free (e.g., ThreatDown Nebula apps have **no cost**) to paid enterprise integrations [citation:7]. | App prices set by publishers (free to enterprise) | Free apps available; paid apps priced individually |
| **[Datadog Marketplace](https://www.datadoghq.com/)** | Integration marketplace for Datadog observability platform. Offers pay-for-what-you-use pricing with **Datadog Consumption Units at $0.01** for on-demand usage; private plans with custom pricing available via sales [citation:8]. | Consumption-based ($0.01/unit); private plans via sales | No permanent free tier; trial via Datadog |
| **[Atlassian Marketplace](https://marketplace.atlassian.com/)** | App marketplace for Jira, Confluence, and other Atlassian products. Cloud and Data Center pricing varies by user tier; apps can have annual list prices scaling from ~$250 (50 users) to $19,000+ (10,000 users) for premium apps [citation:9]. | Variable by app and user tier | Many apps offer 30-day free trials |
| **[Okta Integration Network](https://www.okta.com/integration-network/)** | Directory of pre-built integrations for Okta identity platform. **Listing is 100% free** for developers; integration pricing set by ISVs [citation:10]. | Free to browse; app pricing set by vendors | Free to list and browse |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Apache Camel](https://github.com/apache/camel)** | [![Stars](https://img.shields.io/github/stars/apache/camel?style=social&color=white)](https://github.com/apache/camel/stargazers) | **The most widely used open-source integration framework.** Implements Enterprise Integration Patterns with ~300 components. Java, YAML, or XML routes. Best when integrations live next to Spring Boot or Quarkus applications. No bundled API management or vendor support—you run and support it yourself [citation:11]. |
| **[n8n](https://github.com/n8n-io/n8n)** | [![Stars](https://img.shields.io/github/stars/n8n-io/n8n?style=social&color=white)](https://github.com/n8n-io/n8n/stargazers) | Fair-code workflow automation with visual editor and 400+ integrations. Self-hostable via Docker. Positioned as the open-source Zapier/Make alternative for small automations between SaaS apps—including backup platforms via webhooks and HTTP nodes [citation:11]. |
| **[Cameleer](https://github.com/pmsudhi/cameleer)** | [![Stars](https://img.shields.io/github/stars/pmsudhi/cameleer?style=social&color=white)](https://github.com/pmsudhi/cameleer/stargazers) | **Camel's routes as one native Rust binary** with an MCP server for AI agents. ~230 components. **2.5ms startup and 7MB peak memory** vs. Apache Camel's 1.1s and 399MB. Best for serverless, edge, sidecars, and agent tools with enforced approvals and hash-chained audit. Fewer connectors (no Salesforce component) [citation:11]. |
| **[WSO2 Integrator](https://github.com/wso2/product-integrator)** | [![Stars](https://img.shields.io/github/stars/wso2/product-integrator?style=social&color=white)](https://github.com/wso2/product-integrator/stargazers) | Open-source integration with a **VS Code designer and low-code profile**. WSO2 API Manager available as a separate product. JVM runtime; different flow model from Mule and Camel. Best when you want a designer and vendor subscription with open source [citation:11]. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Spring Integration](https://github.com/spring-projects/spring-integration)** | [![Stars](https://img.shields.io/github/stars/spring-projects/spring-integration?style=social&color=white)](https://github.com/spring-projects/spring-integration/stargazers) | Enterprise Integration Patterns inside the Spring ecosystem. Best when integrations live inside Spring Boot applications. **A library, not a product**—no designer or platform [citation:11]. |

**Frameworks for building custom systems**: Combine **Apache Camel** for EIP-based integration routes (Java teams), **Cameleer** for lightweight Rust-based edge/agent integrations, and **n8n** for visual SaaS-to-SaaS automations—creating a composable integration layer for backup platform connectors without per-connector marketplace fees. **None of these is a turnkey marketplace equivalent**; you build and maintain the specific connectors your data resiliency stack requires [citation:11].

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Marketplace integrations for data resiliency platforms handle sensitive backup metadata and potentially credentials; enforce least-privilege API scopes and audit logging for all connector activity.
- **Marketplace pricing models vary dramatically.** ServiceNow Store offers 90-day trials but requires purchase orders or credit cards for paid apps [citation:2]. AWS Marketplace supports annual subscriptions (up to 40% savings), usage-based dimensions, and contract pricing up to 36 months [citation:4]. Microsoft charges a **3% transaction fee** on marketplace sales [citation:5]. Atlassian app pricing scales by user tier—from ~$250/year (50 users) to $19,000+/year (10,000 users) for premium apps [citation:9]. Okta Integration Network listing is **free** for developers [citation:10]. **Open-source integration runtimes are genuinely viable but require engineering effort.** Apache Camel is mature but JVM-heavy (399MB, 1.1s startup); Cameleer is dramatically lighter (7MB, 2.5ms) but has fewer connectors [citation:11]. Validate connector coverage against your actual backup platform APIs before committing.

---

**Made for integration engineers, platform teams, backup administrators, and developers building data protection automation.**  
Let's make data resiliency integrations more open, composable, and cost-predictable.
