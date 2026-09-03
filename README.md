# Vansh Bhardwaj

📍 Austin, Texas &nbsp;•&nbsp; 📧 scorpio.vansh@gmail.com &nbsp;•&nbsp; 🌐 [vanshbhardwaj.com](https://vanshbhardwaj.com) &nbsp;•&nbsp; 🔗 [LinkedIn](https://www.linkedin.com/in/vanshbhardwaj1945/)

Security engineer who builds. Cloudflare Enterprise IAM last summer, security co-op at MISO (the power grid) right now, and a pile of security tools, cloud projects, and AI agents I've shipped in between. I like taking things apart, figuring out how they break, and putting them back together harder to break.

<p align="left">
  <a href="https://pypi.org/project/flowsec/"><img src="https://img.shields.io/pypi/v/flowsec?label=flowsec%20on%20PyPI&color=2f7d5b" alt="flowsec on PyPI" /></a>
  <img src="https://img.shields.io/badge/Security%2B-SY0--701-b7791f" alt="Security+" />
  <img src="https://komarev.com/ghpvc/?username=VanshBhardwaj1945&label=profile%20views&style=flat&color=blue" alt="profile views" />
</p>


> **Currently:** defending the power grid at MISO by day, sharpening for Summer 2027 security-engineering internships by night.


---

## Projects

**[FlowSec — CI/CD Pipeline Security Scanner](https://github.com/VanshBhardwaj1945/FlowSec)** &nbsp;·&nbsp; `pip install flowsec`
A published Python tool that scans GitHub Actions, GitLab CI, and Azure DevOps pipelines for attack vectors. 25+ rules mapped to MITRE ATT&CK and the OWASP CI/CD Top 10, AI-generated attack narratives, a `--fail-on` flag that blocks risky PRs, and SARIF export straight into GitHub's Security tab.
`Python · PyGithub · Anthropic Claude API · SARIF · Docker · PyPI`

**[Job Tracker Automation](https://github.com/VanshBhardwaj1945/Job-Tracker-Automation)**
The platform that runs my whole job hunt. Hourly workflows discover jobs, Claude scores each one against my profile, and it writes tailored resumes/cover letters — generated on my own laptop by a headless Claude Code agent reached over a Cloudflare Tunnel, at $0 API cost. Serverless on Cloudflare Workers + D1 + R2 behind Zero Trust, fully Terraform.
`Cloudflare (Workers, D1, R2, Zero Trust, Tunnel) · TypeScript · Terraform · Python · Claude API`

**[Browser Render Service](https://github.com/VanshBhardwaj1945/browser-render)**
A small, security-dense AWS service that fetches JavaScript-rendered pages. A URL fetcher is a textbook SSRF target, so the whole design is built around that threat — CIDR blocklists, pre-flight DNS resolution, and per-request interception keep attacker-supplied URLs away from private and cloud-metadata addresses. SSRF guard fails closed, threat blocklist fails open. Zero static AWS keys (GitHub OIDC), fully Terraform, scale-to-zero.
`AWS Lambda · puppeteer-core · Terraform · GitHub OIDC · S3`

**[Click Arena — DevSecOps Pipeline](https://github.com/VanshBhardwaj1945/Click-Arena-DevSecOps)**
A real-time multiplayer game I built as a vehicle for a full DevSecOps pipeline on Azure. Jenkins runs secret scanning, SAST, dependency scanning, container scanning, and post-deploy checks on every push — nothing ships without passing all of it.
`Python · Flask · Jenkins · Terraform · Ansible · SonarQube · Snyk · Trivy · Gitleaks · Azure · Grafana`

**[Cloud Resume Challenge — Azure](https://github.com/VanshBhardwaj1945/cloud-resume-challenge-azure)**
A serverless resume site on Azure with a Python visitor-counter API, Cosmos DB, Front Door CDN, and full CI/CD. Infra fully defined as Terraform with test-gated deploys.
`Azure (Functions, Cosmos DB, Front Door) · Terraform · GitHub Actions · Python`

---

## Labs

**[Cloudflare Security Hardening](https://github.com/VanshBhardwaj1945/cloudflare-security-hardening)**
Six-phase hardening of a live production site — custom WAF rules blocking SQLi/XSS/path traversal, Zero Trust on protected routes, security headers via a Worker, bot protection, and API rate limiting. All Terraform, against real traffic.
`Cloudflare (WAF, Access, Workers, Bot Protection, Page Shield) · Terraform`

**[Network Segmentation & Slowloris DoS Lab](https://github.com/VanshBhardwaj1945/slowloris-dos-attack-lab-)**
A two-part VirtualBox sandbox: built a multi-subnet network segmented by a pfSense firewall and validated an access-control matrix with Nmap and Wireshark, then ran a controlled Slowloris DoS against Apache inside it and detected it with Splunk.
`VirtualBox · pfSense · iptables · Splunk · Nmap · Wireshark · Kali`

**[Azure Labs](https://github.com/VanshBhardwaj1945/azure-labs)**
Hands-on labs covering RBAC and Management Groups, Azure Policy, VNet peering and custom routing, VMs/VMSS, and IaC with ARM Templates and Bicep.
`Azure · Entra ID · Azure Policy · Bicep · ARM · PowerShell`

---

## Tech Stack

| Domain | Tools |
|---|---|
| **Languages** | Python, TypeScript/JavaScript, SQL, Bash/PowerShell, C++, Java |
| **Security Engineering** | IAM (Entra ID, OAuth/OIDC, SCIM), SIEM (Splunk), EDR/IDS, OWASP Top 10, MITRE ATT&CK, XSS/SSRF remediation, vuln scanning (Snyk, Trivy, Gitleaks, Bandit, FlowSec) |
| **Cloud & Infra** | AWS (Lambda, S3, IAM), Azure (Functions, Cosmos DB, Log Analytics), Cloudflare (Workers, Zero Trust, Tunnel), Docker, Kubernetes |
| **IaC & CI/CD** | Terraform, ARM/Bicep, GitHub Actions, GitLab CI, Jenkins, Ansible, OPA/Rego policy-as-code |
| **Detection & Networking** | pfSense/iptables, Wireshark, tcpdump, Nmap, detection playbooks, DISA STIGs, CIS benchmarks |
| **AI Integration** | Anthropic Claude API, headless Claude Code agents, MCP servers, prompt caching, spend guardrails & telemetry |
| **Observability** | Grafana, Azure Monitor/Log Analytics (KQL), Splunk |

---

## Experience

**Security Engineer Co-op — MISO (Midcontinent Independent System Operator)** · Aug – Dec 2026
Defending the bulk electric grid serving 45 million customers in a NERC CIP environment — SIEM/EDR/IDS monitoring and triage, hardening Windows and Linux against DISA STIGs and CIS benchmarks, and automating security workflows in Python and PowerShell.

**Security Engineer Intern — Cloudflare** · Jun – Aug 2026
Enterprise Identity & Access Management (EIAM) team. Built access-review and deprovisioning tooling, wrote access policy as code, and shipped an AI feature kept structurally barred from making destructive decisions.

**Software Engineer Intern — Pitney Bowes** · Jun – Jul 2024
Cloud & DevOps rotation on Azure. Built and validated APIs and backend services, deployed Docker to Kubernetes, and worked in Agile with code reviews.

---

## Certifications

CompTIA Security+ (SY0-701) &nbsp;·&nbsp; Microsoft Azure Fundamentals (AZ-900) &nbsp;·&nbsp; Google Cybersecurity Professional Certificate

---

## Education

**B.S. Computer Science — Cybersecurity Concentration** · Minor in Business Administration
Texas State University · Expected December 2027

---

### A few things I'm into right now
- **Agent security** — what happens when an AI agent has real access, and how you put it on a short leash
- **Identity as the perimeter** — non-human identity, short-lived creds, workload attestation
- **Self-hosting** — running my own AI stack (RAG + local models) instead of renting everyone else's
- **Breaking my own stuff** — I attack the things I build before anyone else gets to
