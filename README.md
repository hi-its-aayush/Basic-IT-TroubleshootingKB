# 🖥️ Basic IT Troubleshooting Knowledge Base

A searchable, single-file IT troubleshooting wiki built with vanilla HTML, CSS, and JavaScript — no frameworks, no backend, no dependencies. Designed for L1/L2 IT Support environments.

**[→ View Live](https://hi-its-aayush.github.io/Basic-IT-TroubleshootingKB/)**

---

## What It Does

A fast, offline-capable reference tool for IT support scenarios. Each article includes:

- **Symptoms** — what the user reports and what you observe
- **Root cause** — why it's happening
- **Step-by-step fix** — numbered steps with copy-to-clipboard commands
- **Escalation notes** — when to escalate and to whom
- **Related articles** — quick links to connected issues

---

## Coverage

35+ articles across 10 categories:

| Category | Example Articles |
|---|---|
| **Networking** | No internet, Wi-Fi connected but no access, mapped drives, VPN |
| **Accounts & Access** | Account lockout, password reset, MFA issues, domain trust failure |
| **Email & Microsoft 365** | Outlook crashing, emails not arriving, Teams login loop, shared mailbox |
| **Windows OS** | Slow PC, BSOD, won't boot, temporary profile, Windows Update stuck |
| **Printing** | Printer offline, print spooler crashing |
| **Hardware** | PC won't power on, no display, USB not recognised, no audio |
| **Security** | Phishing response, ransomware IR, mass account lockout storm |
| **Linux / Server** | SSH refused, disk full, systemd service failures |
| **Active Directory** | GPO not applying, replication failures |
| **Cloud & Azure** | Azure AD sync errors, NSG-blocked VMs |

---

## Features

- **Live search** — searches titles, descriptions, tags, symptoms, and keywords (`Ctrl+K`)
- **Category sidebar** — filter by topic area
- **Severity filter** — HIGH / MEDIUM / LOW priority
- **Active filter badges** — see and clear active filters at a glance
- **Copy commands** — one-click copy for every PowerShell, CMD, and Bash command
- **Zero dependencies** — single HTML file, works offline after first load

---

## How to Add an Article

Find the `ARTICLES` array in the `<script>` section of `index.html` and add a new entry following this structure:

```javascript
{
  id: 36,                          // Unique ID
  cat: 'windows',                  // Category key (see list below)
  severity: 'medium',              // 'high' | 'medium' | 'low'
  title: 'Outlook calendar not syncing',
  desc: 'One-line description shown on the card.',
  tags: ['Outlook', 'Calendar', 'Exchange'],
  keywords: 'calendar not syncing outlook appointments missing',  // Extra search terms
  symptoms: 'What the user reports and what you observe.',
  cause: 'Why this happens.',
  fix: 'High-level resolution approach.',
  escalate: 'When and who to escalate to (optional).',
  steps: [
    {
      text: 'Description of what to do.',
      note: 'Optional tip or warning shown in italic.',   // optional
      code: 'Get-MailboxCalendarConfiguration -Identity user@company.com',
      lang: 'powershell'   // 'cmd' | 'powershell' | 'bash' | 'ios' | 'portal'
    },
    {
      text: 'A prose-only step with no command.',
      text_only: true
    }
  ],
  related: [10, 11]   // IDs of related articles
}
```

**Available category keys:**

| Key | Sidebar Label |
|---|---|
| `networking` | Networking |
| `accounts` | Accounts & Access |
| `email` | Email & Microsoft 365 |
| `windows` | Windows OS |
| `printing` | Printing |
| `hardware` | Hardware |
| `security` | Security |
| `linux` | Linux / Server |
| `cloud` | Cloud & Azure |
| `activedirectory` | Active Directory |

---

## Tech Stack

- **HTML5 / CSS3 / Vanilla JS** — no build step, no framework
- **JetBrains Mono** + **DM Sans** via Google Fonts
- **GitHub Pages** for hosting

---

## Deployment

This repo is deployed via GitHub Pages from the `main` branch root. Any commit to `main` automatically updates the live site within ~60 seconds.

To deploy your own fork:
1. Fork this repo
2. Go to **Settings → Pages → Source → Deploy from branch → main / root**
3. Access at `https://[your-username].github.io/Basic-IT-TroubleshootingKB/`

> **Note:** The copy-to-clipboard feature requires HTTPS and will not work when opening `index.html` directly from the filesystem (`file://`). It works correctly on GitHub Pages.

---

## Author

**Aayush** — IT Support professional based in Sydney, Australia.

[GitHub Profile](https://github.com/hi-its-aayush)
