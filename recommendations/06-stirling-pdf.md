# Recommendation 06: Stirling PDF vs. Adobe Acrobat

A comparison of open-source document processing vs. proprietary subscription models.

**TL;DR:** Stirling-PDF is a highly popular, 100% open-source, self-hosted PDF manipulation platform. Originally designed for military-grade, air-gapped environments, it has evolved into a full enterprise-grade alternative to Adobe Acrobat, used by approximately 75% of the Fortune 500.

## The 90/10 Rule & Economic Impact
*   **OSS as an Economic Driver:** Open-source software provides an estimated $8.8 trillion in replacement value. Stirling-PDF is a prime example, offering a localized, privacy-respecting alternative to expensive cloud services.
*   **The 90% (Stirling PDF):** Deploy Stirling-PDF globally for the majority of users who only need core tools. It eliminates the "shadow IT" risk of employees uploading sensitive data to "free" online converters.
*   **The 10% (Adobe Acrobat):** Reserve Adobe licenses strictly for power users who require specific prepress or proprietary legal workflows.

## Architecture & Raw Specs
*   **Tech Stack:** Built on a Java 21+ backend and TypeScript.
*   **The Engine:** Orchestration layer over proven open-source engines like **PDFium** (rendering/redaction), **LibreOffice** (conversion), and **Tesseract** (OCR).
*   **Deployment:** Officially distributed via Docker. Supports air-gapped, bare-metal, or private VPC deployments to ensure total data sovereignty and compliance (HIPAA, SOC 2).
*   **V2 Multi-Platform:** Now includes native desktop applications for Windows, macOS, and Linux.

## Core Feature Detail
*   **Document Operations:** 50+ operations including merge, split, rotate, compress, and digital signatures.
*   **Automate Pipeline:** The V2 "Automate" feature acts like macros for PDFs, allowing users to chain multiple operations (e.g., upload -> OCR -> compress) and automatically process batches via folder scanning.
*   **Security & Redaction:** Offers *true* content-stripping redaction that drops underlying text data from the file architecture, rather than just masking it.
*   **Stateful Processing:** Upload once into a workspace and run consecutive tools without re-uploading between steps.

## Licensing & Scale
Stirling-PDF operates on an open-core model to support enterprise needs while remaining free for individuals.

| Plan | Pricing | Target | Features |
|------|---------|--------|----------|
| **Community** | $0 | Individuals / Small Teams | All core PDF tools, Docker deployment. |
| **Server** | Flat-rate | Mid-sized Organizations | **Unlimited users**, OAuth2 SSO, external DB support. |
| **Enterprise** | Custom | Large Enterprises | SAML2 SSO, priority support, advanced monitoring. |

## The Reality Check
With over 25 million downloads and deployment in 55,000+ companies, Stirling-PDF is the definitive tool for reducing "license tax." It provides military-grade security and automated processing pipelines that actually outperform proprietary alternatives in privacy and infrastructure control.
