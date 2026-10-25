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


OWardenX is an offline, read-only host-firewall and access-control auditor covering iptables/nftables rulesets, firewalld zones and TCP wrappers. It parses saved rulesets and policy files, evaluating default policies, overly broad allow rules, exposed management ports and missing ingress restrictions. Findings are mapped to CWE and MITRE ATT&CK, scored and graded, and exported as TXT, Markdown, JSON, CSV or SARIF.

---

## ✨ Features


- Parsers for iptables-save/nftables rulesets, firewalld zone XML and hosts.allow/hosts.deny
- Default-policy posture checks (ACCEPT vs DROP) across INPUT/FORWARD chains and zones
- Detection of overly broad allow rules (0.0.0.0/0) and exposed management ports (SSH, RDP, DB)
- Missing ingress restriction and rule-ordering/shadowing analysis
- TCP-wrappers access-control review with permissive-entry detection
- CWE+ATT&CK mapping, offline --root trees, score/grade and TXT/MD/JSON/CSV/SARIF export

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage


```bash
./OWardenX --scan -f sarif -o firewall.sarif
./OWardenX --iptables /etc/iptables/rules.v4 --firewalld /etc/firewalld/zones
./OWardenX -r /mnt/image --fail-on high --json
./OWardenX --demo
./OWardenX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
