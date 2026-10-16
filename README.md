# 🦉 OWardenX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OPass-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OWardenX** — Vaultwarden Deployment Hardening Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

Vaultwarden deployment hardening auditor (offline, read-only)

---

## ✨ Features

- Parsers: .env, docker-compose, data-dir config.json
- Admin token (plaintext / Argon2 PHC / "$$" trap), signups, TLS, SMTP, KDF, rate limits, IP_HEADER, DATABASE_URL, icon / outbound SSRF guards
- nginx / Caddy hints, data-dir perms, backups
- Score + grade A+…F, CWE + MITRE ATT&CK per rule
- TXT / MD / JSON / CSV / SARIF, --demo, --fail-on

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OWardenX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
