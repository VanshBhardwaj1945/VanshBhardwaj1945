# Vansh Bhardwaj

📍 Austin, Texas &nbsp;•&nbsp; 📧 scorpio.vansh@gmail.com &nbsp;•&nbsp; 🌐 [vanshbhardwaj.com](https://vanshbhardwaj.com) &nbsp;•&nbsp; 🔗 [LinkedIn](https://www.linkedin.com/in/vanshbhardwaj1945/)

Security engineer who builds. Cloudflare Enterprise IAM last summer, security co-op at MISO (the power grid) right now, and a pile of security tools, cloud projects, and AI agents I've shipped in between. I like taking things apart, figuring out how they break, and putting them back together harder to break.

**What I build:** security tooling & detection · identity/access platforms · cloud & CI/CD security.

<p align="left">
  <a href="https://pypi.org/project/flowsec/"><img src="https://img.shields.io/pypi/v/flowsec?label=flowsec%20on%20PyPI&color=2f7d5b" alt="flowsec on PyPI" /></a>
  <img src="https://img.shields.io/badge/Security%2B-SY0--701-b7791f" alt="Security+" />
  <img src="https://komarev.com/ghpvc/?username=VanshBhardwaj1945&label=profile%20views&style=flat&color=blue" alt="profile views" />
</p>


> **Currently:** defending the power grid at MISO by day, sharpening for Summer 2027 security-engineering internships by night.
>
> **Exploring right now:** eBPF and runtime security, AI-agent identity and security, and detection engineering.


---

## Projects

**[MISO Copilot](https://github.com/VanshBhardwaj1945/miso-copilot)** &nbsp;·&nbsp; ◐ in progress
An AI assistant for MISO's public grid data, built for the **Fall 2026 MISO Xtern hackathon challenge**. Ask a question in plain English, get an answer in seconds with a source link and a timestamp. The design rule that shaped everything: it never calls MISO's API while answering — a background job keeps a fresh local copy (capped at MISO's published rate limit), so the app keeps working even if the API goes down. 627 poller tests at 100% branch coverage, security CI, React demo UI with a Streamlit backup, and a Terraform cloud deployment already sketched.
`React · FastAPI · Claude · LlamaIndex · Chroma`

**[FlowSec — CI/CD Pipeline Security Scanner](https://github.com/VanshBhardwaj1945/FlowSec)** &nbsp;·&nbsp; `pip install flowsec`
Most teams scan their code but never scan the pipelines that build it. FlowSec fills that gap: a published Python tool that scans GitHub Actions, GitLab CI, and Azure DevOps pipelines for risky configuration. 25+ rules, each mapped to MITRE ATT&CK and the OWASP CI/CD Top 10, a `--fail-on` flag that blocks risky builds, and findings that land straight in GitHub's Security tab.
`Python · PyGithub · Anthropic Claude API · SARIF · Docker · PyPI`

**[Job Tracker Automation](https://github.com/VanshBhardwaj1945/Job-Tracker-Automation)**
The platform that runs my whole job hunt for me. Every hour it finds new roles, Claude scores each one against my profile, and it writes tailored resumes and cover letters. The writing happens on my own laptop through a Cloudflare Tunnel, so it costs $0 in API fees. Serverless on Cloudflare Workers behind Zero Trust login, with everything defined in Terraform.
`Cloudflare (Workers, D1, R2, Zero Trust, Tunnel) · TypeScript · Terraform · Python · Claude API`

**[Browser Render Service](https://github.com/VanshBhardwaj1945/browser-render)**
A small AWS service that fetches pages that need a real browser to render. A URL fetcher is a textbook target for server-side request forgery, so the whole design is built around that threat: it checks where every URL really points before fetching, and blocks anything aimed at private or cloud-internal addresses. The safety guard fails closed. No static AWS keys, fully Terraform, and it scales to zero when idle.
`AWS Lambda · puppeteer-core · Terraform · GitHub OIDC · S3`

**[Click Arena — DevSecOps Pipeline](https://github.com/VanshBhardwaj1945/Click-Arena-DevSecOps)**
A real-time multiplayer game I built as an excuse to build the pipeline around it. On every push, Jenkins runs secret scanning, static analysis, dependency and container scanning, and post-deploy checks. If any of them fail, nothing ships.
`Python · Flask · Jenkins · Terraform · Ansible · SonarQube · Snyk · Trivy · Gitleaks · Azure · Grafana`

**[Cloud Resume Challenge — Azure](https://github.com/VanshBhardwaj1945/cloud-resume-challenge-azure)**
A serverless resume site on Azure with a Python visitor-counter API, a database, a CDN, and full CI/CD. All the infrastructure is defined in Terraform, and failing tests block the deploy.
`Azure (Functions, Cosmos DB, Front Door) · Terraform · GitHub Actions · Python`

---

## Labs

**[Cloudflare Security Hardening](https://github.com/VanshBhardwaj1945/cloudflare-security-hardening)**
A six-phase hardening of my own live site, driven by the real traffic hitting it. Custom firewall rules blocking injection and scanner traffic, Zero Trust login on protected pages, security headers injected at the edge, bot protection, and API rate limiting. All defined in Terraform, all against real traffic.
`Cloudflare (WAF, Access, Workers, Bot Protection, Page Shield) · Terraform`

**[Network Segmentation & Slowloris DoS Lab](https://github.com/VanshBhardwaj1945/slowloris-dos-attack-lab-)**
A sandbox network I built from scratch, then attacked. First I segmented it with a pfSense firewall and proved the traffic rules held using Nmap and Wireshark. Then I ran a controlled Slowloris denial-of-service attack against a web server inside it and caught the attack with Splunk.
`VirtualBox · pfSense · iptables · Splunk · Nmap · Wireshark · Kali`

**[Azure Labs](https://github.com/VanshBhardwaj1945/azure-labs)**
Hands-on Azure administration labs: who-can-do-what (RBAC and management groups), guardrail policies, virtual networking and routing, VMs at scale, and everything written as code with ARM templates and Bicep.
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
Helping defend the electrical grid that serves 45 million people. Day to day that means monitoring and triaging security alerts, hardening Windows and Linux systems against military-grade baselines, and automating the repetitive parts in Python and PowerShell.

**Security Engineer Intern — Cloudflare** · Jun – Aug 2026
On the Enterprise Identity & Access Management team. Built tooling that finds and safely removes access nobody uses anymore, shipped an access-review platform, wrote access policy as code, and built an AI feature deliberately designed so it can never make a destructive decision on its own.

**Software Engineer Intern — Pitney Bowes** · Jun – Jul 2024
A cloud and DevOps rotation on Azure. Built and tested APIs and backend services, deployed containers to Kubernetes, and shipped an AI chatbot with a team of interns.

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
