<!-- ========================================================= -->

<!-- Vib Tools — GitHub Organization Profile                  -->

<!-- Repository: github.com/vibtools/.github                  -->

<!-- File: profile/README.md                                  -->

<!-- ========================================================= -->

<div align="center">

<a href="https://vib.tools">
  <img
    src="https://raw.githubusercontent.com/vibtools/vibtools.github.io/main/public/brand/vibtools-horizontal-light.png"
    width="420"
    alt="Vib Tools"
  >
</a>

<br>
<br>

# Open-Source Infrastructure for Modern Developers

### Build products. Automate infrastructure. Deploy with confidence.

Vib Tools creates developer-first platforms for deployment automation,
identity, infrastructure tooling, and portable software.

<br>

[![Website](https://img.shields.io/badge/Website-vib.tools-111827?style=for-the-badge\&logo=googlechrome\&logoColor=white)](https://vib.tools)
[![YGIT](https://img.shields.io/badge/Deploy-ygit.net-2563EB?style=for-the-badge\&logo=git\&logoColor=white)](https://ygit.net)
[![Developer Portal](https://img.shields.io/badge/Developers-ygit.dev-0F172A?style=for-the-badge\&logo=readthedocs\&logoColor=38BDF8)](https://ygit.dev)
[![Authentication](https://img.shields.io/badge/Identity-auth.vib.tools-7C3AED?style=for-the-badge\&logo=keycloak\&logoColor=white)](https://auth.vib.tools)

<br>

[About](#about-vib-tools) ·
[Ecosystem](#the-vib-tools-ecosystem) ·
[Projects](#open-source-projects) ·
[Technology](#technology-foundation) ·
[Principles](#engineering-principles)

</div>

---

## About Vib Tools

**Vib Tools** is an open-source developer ecosystem focused on removing operational complexity from software development.

We build modern tools for:

```text
Deployment Automation
Identity and Authentication
Developer Infrastructure
Open-Source Web Platforms
Portable Desktop Applications
SDKs and Developer Tooling
```

Our objective is straightforward:

> **Build professional open-source software that makes complex infrastructure feel simple.**

Developers should spend their time building products—not manually configuring deployment pipelines, authentication systems, servers, or fragmented infrastructure.

---

## The Vib Tools Ecosystem

<table>
<tr>
<td width="50%" valign="top">

### 🚀 YGIT

**Git-native deployment automation**

Deploy supported Git repositories to infrastructure owned by the user.

```text
Repository
    ↓
Analyze
    ↓
Connect
    ↓
Deploy
    ↓
Website Live
```

[Open YGIT](https://ygit.net) ·
[Developer Portal](https://ygit.dev) ·
[Repository](https://github.com/vibtools/ygit)

</td>
<td width="50%" valign="top">

### 🔐 Vib ID

**Identity and access platform**

A centralized authentication foundation for Vib Tools products and connected applications.

```text
Identity
    ↓
Authentication
    ↓
Authorization
    ↓
Secure Sessions
```

[Authentication Portal](https://auth.vib.tools) ·
[Account Portal Repository](https://github.com/vibtools/vib-id-account-portal)

</td>
</tr>

<tr>
<td width="50%" valign="top">

### 🧰 Vib Tools

**Open-source developer software**

A growing collection of web platforms, desktop applications, infrastructure components, and developer utilities.

```text
Web Platforms
Desktop Applications
Infrastructure Tools
Developer SDKs
Documentation
```

[Official Website](https://vib.tools) ·
[Website Repository](https://github.com/vibtools/vibtools.github.io)

</td>
<td width="50%" valign="top">

### ✉️ VibMail

**Open-source mail infrastructure**

Mail infrastructure and tooling designed for transparent, extensible, and independently managed deployments.

```text
Mail Infrastructure
Open Architecture
Developer Tooling
Self-Managed Systems
```

[Repository](https://github.com/vibtools/vibmail-open-source)

</td>
</tr>
</table>

---

## YGIT: Deployment Without Infrastructure Lock-In

YGIT is the flagship deployment platform within the Vib Tools ecosystem.

It is an **open-source deployment automation platform**—not a hosting company, website builder, CMS, or traditional control panel.

<div align="center">

```text
Paste Repository  →  Analyze Repository  →  Connect Accounts  →  Deploy  →  Website Live
```

</div>

### Core Capabilities

| Capability             | Description                                                                 |
| ---------------------- | --------------------------------------------------------------------------- |
| Repository Analysis    | Detect frameworks, build commands, package managers, and output directories |
| GitHub Integration     | Connect repositories through controlled provider access                     |
| Cloudflare Integration | Deploy projects to the user’s own Cloudflare infrastructure                 |
| Project Management     | Organize repositories, deployment settings, and project configuration       |
| Deployment Automation  | Queue and execute deployments through a controlled pipeline                 |
| Deployment History     | Review deployment states, logs, provider summaries, and failures            |
| Connected Accounts     | Manage GitHub and Cloudflare provider connections                           |
| Domain Management      | Reserve and manage YGIT-generated project addresses                         |

### Ownership Model

YGIT is built around infrastructure ownership.

```text
The user owns the repository.
The user owns the Cloudflare account.
The user owns the code.
The user owns the domain.
The user owns the infrastructure.

YGIT automates the workflow.
```

No forced infrastructure ownership.
No hidden hosting dependency.
No unnecessary vendor lock-in.

---

## Product Architecture

Vib Tools products are designed around clear architectural boundaries.

```text
Presentation Layer
        ↓
API Layer
        ↓
Engine Layer
        ↓
Provider Layer
        ↓
User-Owned Infrastructure
```

For YGIT, the browser dashboard and CLI are clients of the same platform API.

```text
Dashboard ─┐
           ├── YGIT API → Engines → Worker → Deploy Pipeline → Providers
YGIT CLI ──┘
```

Business logic remains inside independent engines. Provider operations remain behind controlled provider and pipeline boundaries.

---

## Technology Foundation

<table>
<tr>
<td width="33%" valign="top">

### Backend

* Python
* FastAPI
* PostgreSQL
* Redis
* SQLAlchemy
* Alembic
* Pydantic

</td>
<td width="33%" valign="top">

### Frontend

* React
* TypeScript
* Tailwind CSS
* Modern JavaScript
* Responsive Web UI

</td>
<td width="33%" valign="top">

### Identity

* Keycloak
* OpenID Connect
* OAuth 2.0
* PKCE
* Secure server sessions
* Role-based access

</td>
</tr>

<tr>
<td width="33%" valign="top">

### Infrastructure

* Docker
* Coolify
* Cloudflare
* Cloudflare Pages
* Cloudflare R2
* Nginx

</td>
<td width="33%" valign="top">

### Source Control

* Git
* GitHub
* GitHub Apps
* GitHub Actions
* Automated release gates

</td>
<td width="33%" valign="top">

### Desktop Tooling

* Python
* CustomTkinter
* Playwright
* Cross-platform utilities

</td>
</tr>
</table>

---

## Open-Source Projects

### [`vibtools/ygit`](https://github.com/vibtools/ygit)

The core YGIT deployment automation platform.

```text
FastAPI API
Engine Modules
Background Worker
Deploy Pipeline
GitHub Provider
Cloudflare Provider
Dashboard
Operations Console
```

---

### [`vibtools/ygit-cli`](https://github.com/vibtools/ygit-cli)

The official command-line client for the YGIT platform.

```bash
ygit login
ygit init https://github.com/user/repository
ygit deploy --subdomain my-project
```

The CLI communicates exclusively with the YGIT API and does not implement a separate deployment system.

---

### [`vibtools/vib-id-account-portal`](https://github.com/vibtools/vib-id-account-portal)

Account and identity management interface for the Vib ID ecosystem.

---

### [`vibtools/vibmail-open-source`](https://github.com/vibtools/vibmail-open-source)

Open-source mail infrastructure and supporting developer tools.

---

### [`vibtools/vibtools.github.io`](https://github.com/vibtools/vibtools.github.io)

The official Vib Tools website, developer entry point, and product information platform.

---

## Engineering Principles

<table>
<tr>
<td width="50%" valign="top">

### Developer First

Interfaces, APIs, workflows, and documentation are designed for developers from the beginning.

</td>
<td width="50%" valign="top">

### Documentation First

Architecture and contracts are documented before implementation begins.

</td>
</tr>

<tr>
<td width="50%" valign="top">

### Open by Default

We prefer transparent systems, open standards, and inspectable software.

</td>
<td width="50%" valign="top">

### Ownership by Design

Repositories, accounts, domains, code, and infrastructure remain under user control.

</td>
</tr>

<tr>
<td width="50%" valign="top">

### Modular Architecture

Each platform capability has a clear responsibility, public contract, tests, and documentation.

</td>
<td width="50%" valign="top">

### Mature Infrastructure

We reuse reliable open-source infrastructure instead of rebuilding solved systems unnecessarily.

</td>
</tr>
</table>

---

## Product Philosophy

Every Vib Tools product follows a shared principle:

> **Hide infrastructure complexity behind clean, fast, and intuitive developer experiences.**

Our products aim to be:

```text
Dark First
Developer First
Git Native
Cloud Native
Minimal
Professional
Fast
Responsive
Keyboard Friendly
Open Source
```

---

## Organization Map

```text
Vib Tools
│
├── vib.tools
│   └── Company, products, and ecosystem
│
├── ygit.net
│   └── Deployment automation platform
│
├── ygit.dev
│   └── Developer portal and documentation
│
├── auth.vib.tools
│   └── Authentication and identity services
│
├── YGIT CLI
│   └── Terminal client for the YGIT API
│
└── Open-Source Projects
    ├── Web platforms
    ├── Infrastructure tooling
    ├── Desktop applications
    └── Developer SDKs
```

---

## Platform Status

| Product           | Current Stage           |
| ----------------- | ----------------------- |
| Vib Tools Website | Active                  |
| YGIT Platform     | MVP Development         |
| YGIT CLI          | Foundation Development  |
| Vib ID            | Active Development      |
| VibMail           | Open-Source Development |
| YGIT Marketplace  | Planned                 |
| Plugin Platform   | Planned                 |
| AI Builder        | Planned                 |
| Analytics         | Planned                 |
| Teams             | Planned                 |

---

## Contributing

We welcome developers who care about open-source infrastructure, deployment automation, identity systems, developer experience, and maintainable software architecture.

Before contributing:

1. Review the repository documentation.
2. Read the architecture and contribution rules.
3. Search existing issues and discussions.
4. Open an issue before proposing major architectural changes.
5. Keep pull requests focused, documented, and testable.

Explore the organization:

[![GitHub Organization](https://img.shields.io/badge/GitHub-vibtools-181717?style=for-the-badge\&logo=github)](https://github.com/vibtools)

---

<div align="center">

<br>

<img
src="https://raw.githubusercontent.com/vibtools/vibtools.github.io/main/public/brand/vibtools-icon.png"
width="56"
alt="Vib Tools Icon">

## Build Better. Deploy Faster.

**Open-source infrastructure for developers who want to own their stack.**

[Website](https://vib.tools) ·
[YGIT](https://ygit.net) ·
[Developer Portal](https://ygit.dev) ·
[GitHub](https://github.com/vibtools)

<br>

<sub>Built by Vib Tools · Open source · Developer first</sub>

</div>
