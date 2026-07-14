# Vansh Bhardwaj  
Cloud Security · DevSecOps · Security Engineering · Cloud Infrastructure

📍 Austin, Texas  
📧 Scorpio.vansh@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/vanshbhardwaj1945/)

---

## About

I got into security the same way most people do — by breaking things and trying to figure out why they broke. That curiosity turned into a habit of building systems from scratch, tearing them apart, and rebuilding them with security baked in from the start rather than bolted on at the end.

Right now I'm focused on DevSecOps and cloud security engineering — building tools that automate security decisions, pipelines that enforce security gates before anything ships, and infrastructure that's observable enough to catch problems early.

**What I'm focused on:**
- Building security tooling in Python — scanners, analyzers, automation
- DevSecOps: CI/CD pipelines with real security gates, not checkbox scanning
- Cloud security on Azure and AWS
- Detection engineering and incident response automation

---

## Projects

| Project | Status | What I Built | Technologies |
|---|---|---|---|
| **[Job Tracker Automation](https://github.com/VanshBhardwaj1945/Job-Tracker-Automation)** | Complete | End-to-end job-hunt automation: multi-source job discovery, LLM matching against my profile, application tracking, and per-job AI-generated resumes / cover letters / interview prep. Jobs are tagged into a hierarchical, multi-membership category taxonomy that rolls up through an ancestor-closure column — driving tri-state tree filters and analytics at any level — alongside a cost-analytics center that charts spend over time by provider. Serverless full-stack on Cloudflare Workers + D1 + R2 behind zero-trust Access, entirely Terraform IaC; automation on GitHub Actions. Prompt caching, the Message Batches API, and a daily spend guardrail keep AI cost in pocket-change territory | Cloudflare (Workers, D1, R2, Zero Trust Access), TypeScript, Hono, Terraform, Python, GitHub Actions, Anthropic Claude (Haiku + Opus, Message Batches), Discord, IMAP |
| **[FlowSec — CI/CD Pipeline Security Analyzer](https://github.com/VanshBhardwaj1945/FlowSec)** | Complete | Published Python security tool (`pip install flowsec`) that scans GitHub Actions, GitLab CI, and Azure DevOps pipeline configurations for attack vectors. 25+ rules mapped to MITRE ATT&CK and OWASP CICD Top 10. Findings include AI-generated attack narratives, interactive HTML reports with PDF export, and a `--fail-on` flag that blocks PRs when critical issues are found. Platform-aware rule engine handles all three CI/CD platforms from a single codebase | Python, PyGithub, PyYAML, Anthropic Claude API, Jinja2, rich, Docker, hatch, ruff, mypy, bandit |
| **[Click Arena — DevSecOps Pipeline](https://github.com/VanshBhardwaj1945/Click-Arena-DevSecOps)** | Complete | Real-time multiplayer game built as a vehicle for a full DevSecOps pipeline on Azure. Jenkins runs secret scanning, SAST, dependency scanning, container scanning, and post-deploy verification on every push. Nothing reaches production without passing all stages | Python, Flask, Docker, Jenkins, Terraform, Ansible, SonarQube, Snyk, Trivy, Gitleaks, Azure Container Apps, Azure Container Registry, Cloudflare Workers, Grafana |
| **[Cloud Resume Challenge — Azure](https://github.com/VanshBhardwaj1945/cloud-resume-challenge-azure)** | Complete | Serverless resume site on Azure with a Python visitor counter API, Cosmos DB backend, Azure Front Door CDN, and full CI/CD via GitHub Actions. Infrastructure fully defined as Terraform with test-gated deployments | Azure (Storage, Front Door, Functions, Cosmos DB), Terraform, GitHub Actions, Python, pytest, Cloudflare |

---

## Labs

| Lab | Status | What I Did | Technologies |
|---|---|---|---|
| **[Cloudflare Security Hardening](https://github.com/VanshBhardwaj1945/cloudflare-security-hardening)** | Complete | Six-phase hardening of a live production site — custom WAF rules blocking SQLi/XSS/path traversal, Zero Trust access on protected routes, HTTP security headers via a Worker, bot protection, and rate limiting on the API endpoint. Everything managed as Terraform IaC against real traffic | Cloudflare (WAF, Access, Workers, Bot Protection, Page Shield), Terraform, JavaScript |
| **[Azure Labs](https://github.com/VanshBhardwaj1945/azure-labs)** | In Progress | Hands-on AZ-104 labs covering RBAC and Management Groups, Azure Policy enforcement, VNet peering and custom routing, VM and VMSS management, and IaC with ARM Templates and Bicep | Azure, Entra ID, Azure Policy, Bicep, ARM Templates, PowerShell, Azure CLI |
| **[Slowloris DoS Detection Lab](https://github.com/VanshBhardwaj1945/slowloris-dos-attack-lab-)** | Complete | Controlled Slowloris attack against Apache in an isolated VirtualBox lab, with Splunk ingesting Apache logs for detection. Built to understand how low-bandwidth application-layer attacks work and how to detect them at the SIEM level | Splunk, Wireshark, Nmap, Kali, Apache, pfSense |
| **[Network Segmentation Lab](https://github.com/VanshBhardwaj1945/Project-1-Sandbox-Firewall-Access-Control-CS4371-CS5378)** | Complete | Multi-subnet VirtualBox environment with pfSense as the router/firewall. Built and validated an access control matrix using Nmap scanning and Wireshark packet captures before and after rule deployment | VirtualBox, pfSense, iptables, Nmap, Wireshark |

---

## Tech Stack

| Domain | Technologies |
|---|---|
| **Programming & Scripting** | Python, PowerShell/Bash, JavaScript, C++, Java |
| **Cloud Platform** | Microsoft Azure (Portal, Storage, Front Door, Functions, Cosmos DB, Container Registry, Container Apps, Log Analytics) |
| **Identity & Governance** | Microsoft Entra ID, RBAC, Azure Policy, Management Groups, Service Principals |
| **Compute & Networking** | Azure VMs, VM Scale Sets, Load Balancer, NSG, VNet Peering, Network Watcher, Route Tables |
| **Infrastructure as Code** | Terraform, ARM Templates (JSON), Bicep |
| **Containers** | Docker, Azure Container Registry, Azure Container Apps |
| **CI/CD** | Jenkins, GitHub Actions, Azure CLI, Azure PowerShell |
| **Configuration Management** | Ansible |
| **Secret Detection** | Gitleaks (CI pipeline + pre-commit hooks) |
| **SAST** | SonarQube, Semgrep, Bandit |
| **Dependency Scanning** | Snyk |
| **Container Security** | Trivy |
| **Edge & Web Security** | Cloudflare (WAF, Access, Workers, Bot Protection, Page Shield), HTTP Security Headers |
| **Observability** | Grafana, Azure Monitor, Azure Log Analytics |
| **Detection & SIEM** | Splunk |
| **Network Analysis & Recon** | Wireshark, tcpdump, Nmap, Zenmap |
| **Firewall & Segmentation** | pfSense, iptables, WAF, NSG |
| **Virtualization & Imaging** | VirtualBox, VMware, Windows Sysprep |
| **Operating Systems** | Linux (Ubuntu/Kali), Windows Server, Windows, Mac OS |
| **Frontend & Testing** | HTML, CSS, pytest, ruff, mypy |
| **Security Tooling** | Custom rule engines, MITRE ATT&CK mapping, OWASP CICD Top 10, PyYAML, abstract base classes |
| **AI Integration** | Anthropic Claude API, prompt engineering, local response caching |
| **Package Publishing** | PyPI, hatch, pyproject.toml, trusted publishers, GitHub Actions CI/CD release automation |
| **Security Frameworks** | OWASP Top 10, OWASP CICD Top 10, MITRE ATT&CK, SLSA |

---

## Experience

- ***Security Engineer Intern*** | Upcoming - Fall 2026

  TBD

- **Security Engineer Intern — Cloudflare** | In Progress - Summer 2026

  Working on the Enterprise Identity and Access Management (EIAM) team. Automating internal employee access provisioning and deprovisioning across   enterprise software, ensuring the right people have the right access at the right time with no manual intervention.

- **Software Engineer Intern — Pitney Bowes** | Summer 2024

  Worked on cloud development and testing on Microsoft Azure. Helped build and validate APIs and backend services, participated in Agile ceremonies and code reviews, and documented test procedures to keep things reproducible.

---

## Certifications

- Microsoft Certified: Azure Administrator (AZ-104) — *In Progress*
- Microsoft Certified: Azure Fundamentals (AZ-900)
- CompTIA Security+ (SY0-701)
- Google Cybersecurity Professional Certificate

---

## Education

**B.S. Computer Science — Cybersecurity Concentration**  
Minor in Business Administration  
Texas State University | Expected May 2027
