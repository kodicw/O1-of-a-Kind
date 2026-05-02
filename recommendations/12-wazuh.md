# Recommendation 12: Wazuh - Enterprise Open-Source SIEM & XDR

A unified platform for Security Information and Event Management (SIEM) and Extended Detection and Response (XDR).

**TL;DR:** Wazuh eliminates the licensing trap of proprietary SIEMs (Splunk, QRadar) by providing enterprise-grade security monitoring with zero volume-based fees. It provides deep endpoint visibility, active threat response, and automated compliance tracking.

## 1. Architecture: Lightweight & Highly Scalable
Wazuh is designed for extreme flexibility across public clouds, private clouds, and on-premise data centers.
*   **Wazuh Agent:** A single, lightweight multi-platform agent (Linux, Windows, macOS) for real-time data collection and automated response.
*   **Wazuh Manager:** Central analysis engine that decodes data against 3,000+ rules and MITRE ATT&CK.
*   **Wazuh Indexer:** High-performance full-text search and analytics engine.
*   **Wazuh Dashboard:** Flexible web UI for threat hunting, compliance, and incident analysis.
*   **Agentless Support:** Full monitoring for firewalls and routers via Syslog, SSH, or APIs.

## 2. Core Capabilities
Wazuh integrates features that typically require expensive third-party add-ons:
*   **File Integrity Monitoring (FIM):** Detects changes in content, permissions, and attributes, logging the specific user and process responsible.
*   **Security Configuration Assessment (SCA):** Continuous scanning against CIS benchmarks to eliminate exploitable misconfigurations.
*   **Active Response:** Executes automated scripts to block IPs, disable accounts, or isolate endpoints upon threat detection.
*   **Vulnerability Detection:** Cross-correlates system inventory against CVE databases and integrates with VirusTotal/YARA.
*   **Container Security:** Native monitoring for Docker and Kubernetes APIs.

## 3. The Compliance Engine
Out-of-the-box rule mapping and dashboards for global standards:
*   **Supported Standards:** PCI DSS, HIPAA, GDPR, NIST 800-53, TSC, NIS2, and DORA.
*   **Automation:** Ensures continuous auditing and proves system hardening compliance for regulated sectors.

## Scale, Cost, & Efficiency
*   **TCO Advantage:** $0 software license fee. Replaces unpredictable volume-based pricing with predictable options:
    *   **Self-Managed:** Leverage internal engineering to run for free.
    *   **Wazuh Cloud (SaaS):** Fully vendor-managed, PCI DSS and SOC 2 certified. Predictable pricing starting at roughly **$571/month for up to 100 agents**.
*   **Performance:** Scalability testing proves Wazuh handles up to **500 Events Per Second (EPS)** with 95% of events processed in under 500 milliseconds.
*   **Deployment Flexibility:** "All-in-one" for small shops or "Multi-node Cluster" for high availability in enterprises.

**The Strategic Choice:**
Wazuh is the definitive choice for organizations requiring deep security visibility without vendor lock-in, providing a scalable, secure-by-design foundation for modern infrastructure.
