# 🦉 OBTClassic

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-Security-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OBTClassic** — part of the OwlSec Toolkit.

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OBTClassic analyzes Bluetooth Classic (BR/EDR) device-discovery data you have already collected. It decodes each device's Class-of-Device (major/minor type and service classes), parses EIR records and resolves the vendor from the OUI. It then flags devices that expose too much. It reads CSV files only and never scans, pairs with or transmits to any device.

---

## ✨ Features

- Parses BR/EDR discovery CSVs (BDADDR, COD, Name, RSSI, EIR)
- Decodes Class-of-Device: major/minor device class and service classes
- EIR record parsing and OUI vendor lookup
- Device enumeration, classification and exposure flags
- Synthetic discovery-CSV generator for testing; findings graded A+ to F with MITRE ATT&CK mapping
- Reports in TXT / JSON / Markdown / CSV / SARIF; exits with code 3 on CRITICAL/HIGH findings

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OBTClassic                                 # interactive menu
./OBTClassic --analyze discovery.csv
./OBTClassic --generate --out synth.csv
./OBTClassic --demo
```

Run `./OBTClassic --help` for the full list of options.

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled.s.Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
