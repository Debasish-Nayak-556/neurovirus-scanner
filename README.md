# neurovirus-scanner
🛡️ Full-stack AI-powered virus &amp; malware scanner with cyberpunk UI — Flask + ClamAV + YARA + VirusTotal
# 🛡️ NeuroVirus — Advanced Threat Intelligence Platform

![Platform](https://img.shields.io/badge/Platform-Docker-blue?style=for-the-badge&logo=docker)
![Python](https://img.shields.io/badge/Python-3.12-green?style=for-the-badge&logo=python)
![React](https://img.shields.io/badge/React-18-cyan?style=for-the-badge&logo=react)
![ClamAV](https://img.shields.io/badge/ClamAV-Integrated-red?style=for-the-badge)
![YARA](https://img.shields.io/badge/YARA-Rules-orange?style=for-the-badge)
![VirusTotal](https://img.shields.io/badge/VirusTotal-API-purple?style=for-the-badge)

> A full-stack virus and malware scanner with a cyberpunk-themed interface.
> Upload any file and get a deep multi-engine threat analysis in seconds.

---

## ⚡ Features

- 🦠 **ClamAV** — Real-time signature-based malware detection
- 🧬 **YARA Rules** — Custom rule engine for behavioral pattern matching
- 🌐 **VirusTotal API** — 70+ AV engines via cloud intelligence
- 🔬 **Entropy Analysis** — Detects packed, encrypted or obfuscated files
- 📡 **Network IOC Extraction** — Finds C2 URLs, suspicious IPs, Tor domains
- ⚙️ **PE Header Analysis** — Deep inspection of Windows executables
- 🔤 **Suspicious String Detection** — 23+ dangerous API and command patterns
- 📋 **Scan History** — Full audit trail of all previous scans
- 🔒 **Quarantine System** — Isolate flagged files instantly
- 💻 **Cyberpunk UI** — Immersive dark interface with live scan console

---

## 🖥️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React 18 + Axios |
| Backend | Python 3.12 + Flask |
| AV Engine | ClamAV |
| Rule Engine | YARA 4.x |
| Threat Intel | VirusTotal API v3 |
| Containers | Docker + Docker Compose |
| Web Server | Nginx |

---

## 🚀 Quick Start

### Prerequisites
- Docker Desktop installed and running

### Run in 3 commands

\`\`\`bash
git clone https://github.com/Debasish-Nayak-556/neurovirus-scanner
cd neurovirus-scanner
cp .env.example .env
docker compose up --build
\`\`\`

Open browser at **http://localhost:3000**

> ⚠️ First run takes 3–5 minutes — ClamAV downloads ~350MB signature database

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/scan` | Upload and scan files |
| GET | `/api/scan/<id>` | Get scan result by ID |
| DELETE | `/api/scan/<id>` | Delete scan result |
| GET | `/api/history` | List recent scans |
| POST | `/api/quarantine` | Quarantine a file |
| GET | `/api/status` | Engine health status |

---

## 📁 Project Structure

\`\`\`
neurovirus/
├── docker-compose.yml
├── backend/
│   ├── app/
│   │   ├── scanner.py      ← Core scan engine
│   │   ├── routes.py       ← REST API
│   │   └── config.py
│   └── yara_rules/         ← Custom YARA rules
└── frontend/
    └── src/
        ├── App.js          ← Cyberpunk UI
        └── api.js          ← API client
\`\`\`

---

## ⚙️ Environment Variables

\`\`\`env
VIRUSTOTAL_API_KEY=your_key_here
SECRET_KEY=your_secret_here
CLAMD_HOST=127.0.0.1
CLAMD_PORT=3310
\`\`\`

Get a free VirusTotal API key at https://www.virustotal.com/gui/join-us

---

## 📜 License

MIT License — Free to use and modify

---

## ⭐ If you found this useful, please star the repo!
```

---

## GitHub Topics to add
```
virus-scanner malware-detection cybersecurity flask react docker clamav yara virustotal threat-intelligence cyberpunk
