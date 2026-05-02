# Recommendation 08: HashiCorp Nomad

Lightweight, flexible, and highly scalable workload orchestration.

**TL;DR:** Nomad is a simple and powerful alternative to Kubernetes. It provides the same core benefits (scheduling, self-healing, scaling) but with a fraction of the complexity and overhead.

## Nomad vs. Kubernetes
While Kubernetes has become the industry default, it is often "too much machine" for many organizations, requiring a dedicated team just to manage the control plane. Nomad is a single binary that is significantly easier to deploy and maintain.

| Feature | Kubernetes (K8s) | HashiCorp Nomad |
|---------|-------------------|-----------------|
| **Complexity** | High (Requires many components) | Low (Single binary) |
| **Workloads** | Containers only (mostly) | Containers, Binaries, Java, QEMU |
| **Learning Curve** | Steep | Shallow |
| **Resource Overhead** | Significant | Minimal |
| **Multi-Region** | Complex (Federation) | Native & Simple |

## Core Pillars
*   **Single Binary:** One tool for both server and client. Easy to deploy on NixOS or any other distribution.
*   **Workload Agnostic:** Orchestrate Docker containers alongside raw executables, standalone Java JARs, or even full VMs via QEMU.
*   **Simple Federation:** Native support for multi-region and multi-datacenter deployments without complex networking overlays.
*   **Tight Integration:** Works seamlessly with the rest of the HashiCorp stack (Consul for service discovery, Vault for secrets).

## Efficiency & ROI
*   **Lower Compute Costs:** Nomad's control plane uses far fewer resources than a Kubernetes control plane, leaving more CPU and RAM for your actual applications.
*   **Reduced Training Costs:** Engineering teams can learn and master Nomad in days, not months.
*   **Operational Simplicity:** Dramatically reduces the number of "moving parts" in your infrastructure, leading to higher reliability and fewer man-hours spent on maintenance.

## Scale
Nomad is built for massive scale. It powers some of the largest workloads on the internet (including parts of Cloudflare and Roblox), handling tens of thousands of nodes across global datacenters with ease.
