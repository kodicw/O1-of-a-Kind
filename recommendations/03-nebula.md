# Recommendation 03: Nebula

A scalable overlay networking tool for true cross-datacenter and multi-cloud connectivity.

## Scale
*   **True Cross-Datacenter:** Designed by Slack to handle tens of thousands of nodes across globally distributed datacenters and cloud providers.
*   **Lighthouse Architecture:** Uses "Lighthouses" only for node discovery. Once nodes find each other, traffic is encrypted and sent directly, avoiding the bottlenecks of centralized gateways.

## Cost & ROI
*   **Open Source:** $0 licensing cost. Reduces dependencies on expensive MPLS circuits or managed SD-WAN providers.
*   **Low Overhead:** Extremely lightweight binary that runs on everything from small IoT devices to high-end servers.

## Security
*   **Identity-Based Connectivity:** Communication is based on certificates (PKI). Each node is identified by its identity (e.g., "web-server", "db-cluster") rather than just an IP address.
*   **Encrypted by Default:** Uses high-performance encryption (Noise Protocol) for all peer-to-peer traffic.
*   **Micro-Segmentation:** Native firewall capabilities allow for granular control over which nodes can talk to each other based on their certificate identities.

## Efficiency & Management
*   **Infrastructure as Code:** Nebula configurations and certificates can be easily managed and deployed via tools like Ansible, Terraform, or SaltStack.
*   **Seamless Roaming:** Nodes can change IP addresses or move between networks (e.g., from an AWS VPC to a private DC) without losing connectivity.

## Use Case: Nebula vs. Tailscale
*   **Nebula:** Best for **machine-to-machine (M2M)** traffic at massive scale, especially in complex cloud/on-prem hybrid environments. Ideal for backend infrastructure.
*   **Tailscale:** Best for **user-to-machine (U2M)** or employee access where ease of use and SSO integration are the primary drivers.
