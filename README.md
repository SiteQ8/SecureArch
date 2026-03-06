# 🔐 SecureArch

**A zero-dependency, browser-based security architecture design and threat modeling tool.**

> Design secure system architectures, model threats with STRIDE, assess risk, and export professional reports — entirely in your browser. No backend, no installation, no data leaves your machine.

[![License: MIT](https://img.shields.io/badge/License-MIT-00d4aa.svg)](LICENSE)
[![HTML5](https://img.shields.io/badge/Built%20with-HTML5-ff6b35.svg)]()
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-Zero-2ed573.svg)]()

---

## ✨ Features

### 🏗 Architecture Designer
- **30+ security components** across 6 categories: Network, Compute, Data, Identity, External, Monitoring
- **Drag-and-drop canvas** — pull components from the library onto the canvas
- **Security zones** — visually segment architecture into External, DMZ, Internal Network, and Cloud zones
- **Connection mapping** — draw encrypted/unencrypted, trusted/untrusted connections between components
- **Protocol labeling** — annotate each connection with its protocol (HTTPS, SQL/TLS, gRPC, etc.)
- **Pan & zoom** — smooth canvas navigation with mouse wheel zoom and middle-click pan
- **Minimap** — live overview of your architecture
- **Keyboard shortcuts** — `V` Select · `C` Connect · `Z` Add Zone · `F` Fit to screen · `Del` Delete

### 🎯 Threat Modeling (STRIDE)
- **Automated threat identification** — threats are auto-mapped from component types
- **STRIDE framework** — full coverage of Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege
- **Risk classification** — threats categorized as Critical / High / Medium / Low
- **Live updates** — threat model reflects your current architecture in real time

### 📊 Risk Assessment Report
- **Interactive risk matrix** — 4×4 impact/likelihood grid
- **Component inventory** — full table with zone, risk level, controls, and threat count
- **Security controls compliance** — gaps against NIST, ISO 27001, CIS Controls, SOC2, OWASP
- **Vulnerability database** — pre-mapped CVEs and vulnerability patterns per component type, with mitigations

### 💾 Save / Load / Export
- Save architecture as `.secarch.json` — version-controllable, shareable
- Load previously saved architectures
- Export professional HTML security reports

---

## 🚀 Quick Start

### Option 1: GitHub Pages (Recommended)
Fork this repo, then enable GitHub Pages on `main` branch. Your tool will be live at:
```
https://SiteQ8.github.io/SecureArch/
```

### Option 2: Run Locally
```bash
git clone https://github.com/SiteQ8/SecureArch.git
cd SecureArch
# Open index.html in any modern browser — no server needed
open index.html
```

### Option 3: Direct Download
Download `index.html` and open it. That's it. Zero dependencies, zero build step.

---

## 🧩 Component Library

| Category | Components |
|---|---|
| **Network** | Firewall, WAF, IDS/IPS, Load Balancer, VPN Gateway, Router |
| **Compute** | Web Server, App Server, API Gateway, Container, Serverless |
| **Data** | Database, Cache/Redis, Object Store, Backup Store, Secret Manager |
| **Identity** | Identity Provider (SSO), MFA Service, PAM/IAM |
| **External** | Internet, Client Browser, Mobile App, 3rd Party API |
| **Monitoring** | SIEM, SOAR, Log Aggregator |

---

## 🗺 Security Zones

| Zone | Color | Purpose |
|---|---|---|
| **External** | 🔴 Red | Internet-facing, untrusted zone |
| **DMZ** | 🟡 Yellow | Demilitarized zone — public-facing services |
| **Internal Network** | 🟢 Green | Private application and data tier |
| **Cloud** | 🔵 Blue | Cloud-hosted services |

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|---|---|
| `V` | Select tool |
| `C` | Connect tool |
| `Z` | Add security zone |
| `F` | Fit architecture to screen |
| `Del` / `Backspace` | Delete selected component |
| `Esc` | Cancel operation / close modal |
| `Alt + Drag` | Pan canvas |
| `Scroll` | Zoom in/out |

---

## 📁 File Format

Architecture files are plain JSON with `.secarch.json` extension:

```json
{
  "_version": "1.0",
  "_tool": "SecureArch",
  "_author": "Ali AlEnezi",
  "nodes": [...],
  "connections": [...],
  "zones": [...]
}
```

These are fully version-controllable and diff-friendly for tracking architecture changes in Git.

---

## 🛡 Security Frameworks Covered

- **STRIDE** — Threat classification model (Microsoft)
- **NIST SP 800-53** — Security and privacy controls
- **NIST SP 800-63** — Identity and authentication
- **ISO/IEC 27001** — Information security management
- **CIS Controls v8** — Cybersecurity best practices
- **OWASP Top 10** — Web application security risks
- **SOC 2** — Trust services criteria

---

## 🤝 Contributing

Contributions welcome! Ideas for future features:

- [ ] Export to PNG / PDF diagram
- [ ] Import from draw.io / Visio XML
- [ ] Custom component definitions (via JSON)
- [ ] Collaboration mode (WebRTC)
- [ ] MITRE ATT&CK integration
- [ ] Compliance mapping (PCI-DSS, HIPAA, GDPR)
- [ ] Architecture version diffing

To contribute:
1. Fork the repo
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m 'Add my feature'`
4. Push and open a Pull Request

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

## 👤 Author

**Ali AlEnezi**  
GitHub: [@SiteQ8](https://github.com/SiteQ8)  
Email: site@hotmail.com

---

<div align="center">
<sub>Built with ❤️ for the security community · No tracking · No telemetry · Your data stays on your machine</sub>
</div>
