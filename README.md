Here is an updated version of your README based on the code in your `index.html`. It accurately reflects the expanded content (150+ articles) and the refined categorization system you've implemented.

# 🖥️ Basic IT Troubleshooting Knowledge Base

A searchable, single-file IT troubleshooting wiki built with vanilla HTML, CSS, and JavaScript — no frameworks, no backend, no dependencies. Designed for L1/L2 IT Support environments.

**[→ View Live](https://hi-its-aayush.github.io/Basic-IT-TroubleshootingKB/)**

---

## What It Does

A high-performance, offline-capable reference tool for IT support scenarios. Each article provides a structured breakdown:

- **Symptoms** — what the user reports and what you observe
- **Root Cause** — why the issue is occurring
- **Resolution Approach** — the high-level fix strategy
- **Step-by-Step Fix** — numbered steps with integrated copy-to-clipboard code blocks for PowerShell, CMD, Bash, and Registry
- **Escalation Notes** — critical warnings and when to involve specialized teams
- **Related Articles** — quick links to interconnected troubleshooting paths

---

## Coverage

**150+ comprehensive articles** across 12 categories:

| Category | Coverage Areas |
|---|---|
| **Networking & VPN** | Connectivity, DNS, MTU adjustment, captive portals, firewall exceptions |
| **Accounts & AD** | Lockouts, trust relationships, LAPS, MFA resets, and provisioning |
| **Email & Exchange** | Outlook performance, OST repair, mailbox conversion, delivery traces |
| **Windows OS** | Performance, BSOD, boot recovery, registry fixes, system file repairs |
| **Teams & OneDrive** | Cache clearing, sync conflicts, presence issues, SharePoint recovery |
| **Hardware** | POST failure, display issues, docking stations, peripherals, BIOS updates |
| **Security & IR** | Phishing triage, compromised accounts, malware isolation, VirusTotal checks |
| **Intune / MDM** | Policy sync, compliance, app deployment, Autopilot, remote wipes |
| **Linux / Server** | SSH troubleshooting, disk space management, systemd |
| **Cloud & Azure** | Entra ID (Azure AD) sync errors, attribute conflicts, license management |

---

## Features

- **Blazing Fast Search** — Instant filtering across titles, descriptions, tags, and symptoms (`Ctrl+K`)
- **Categorical Navigation** — Sidebar filtering by functional area or severity level
- **Severity Awareness** — Visual indicators for HIGH, MEDIUM, and LOW priority issues
- **Dynamic Filter Badges** — Manage complex search/filter combinations at a glance
- **Command Integration** — One-click copy functionality for every terminal command
- **Zero Dependencies** — Single HTML file architecture; works offline once loaded

---

## Technical Reference

### Available Category Keys
To extend the knowledge base, use these category keys in the `ARTICLES` array:

- `networking`, `accounts`, `email`, `teams`, `windows`, `hardware`, `intune`, `security`, `linux`, `activedirectory`, `cloud`

### Tech Stack
- **HTML5 / CSS3 / Vanilla JS** — No build step or frameworks required
- **Typography** — JetBrains Mono (Code) and DM Sans (UI) via Google Fonts
- **Deployment** — Optimized for GitHub Pages

---

## Author

**Aayush Acharya** — IT Support professional based in Sydney, Australia.

[GitHub Profile](https://github.com/hi-its-aayush)
