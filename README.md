# UEFI Attack Surface Research

> Bootkits · Secure Boot Bypasses · Pre-OS Exploitation · Firmware Rootkits · SMM Security Research

![Status](https://img.shields.io/badge/Status-Research-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Classification](https://img.shields.io/badge/TLP-WHITE-green)

## Overview

This repository contains research materials related to modern UEFI security threats, firmware attack surfaces, and detection methodologies.

The project focuses on:

- UEFI bootkits and firmware persistence
- Secure Boot bypass techniques
- DXE driver abuse and boot service hooking
- System Management Mode (SMM) attack vectors
- Runtime variable manipulation
- Firmware forensic analysis
- Enterprise detection and mitigation strategies

---

## White Paper

**UEFI Attack Surface Research**

The included white paper provides an overview of:

- UEFI architecture and boot phases
- Real-world UEFI malware families
- BlackLotus analysis
- MoonBounce analysis
- Detection methodologies
- CHIPSEC auditing techniques
- Enterprise hardening recommendations
- Firmware forensic workflows

---

## Topics Covered

### UEFI Boot Phases

- SEC
- PEI
- DXE
- BDS
- TSL
- Runtime Services

### Threat Categories

- UEFI Bootkits
- Firmware Rootkits
- Secure Boot Bypasses
- Option ROM Attacks
- ACPI Manipulation
- Runtime Variable Abuse
- SMM Exploitation

### Known Threats

- BlackLotus
- MoonBounce
- LoJax
- ESPecter
- Bootkitty
- Cuttlefish
- MosaicRegressor
- CosmicStrand

---

## Detection Tooling

The research references the following tools:

- CHIPSEC
- UEFITool
- Binwalk
- ME Analyzer
- Ghidra
- FwHunt
- sbctl
- mokutil

---

## Example Detection Workflow

1. Verify Secure Boot state.
2. Enumerate UEFI variables.
3. Dump and analyze SPI flash.
4. Inspect DXE drivers.
5. Validate SMM integrity.
6. Compare firmware hashes against known-good baselines.
7. Investigate persistence mechanisms.

---

## Internal Research Tooling

### FindBootServices.py

Ghidra-based helper script designed to identify suspicious modifications to EFI Boot Services tables.

Potential detections include:

- ExitBootServices hooks
- Runtime Service hooks
- Unexpected pointer redirections
- Indicators associated with known UEFI malware families

---

## Intended Audience

This repository is intended for:

- Security researchers
- Incident responders
- DFIR specialists
- Firmware analysts
- Red teams
- Blue teams
- Enterprise security architects

---

## Disclaimer

The information contained in this repository is provided solely for educational, defensive, and research purposes.

No offensive tooling intended for unauthorized access is included. Users are responsible for complying with all applicable laws and regulations.

---

## References

- ESET Research
- Microsoft Security Response Center
- MITRE ATT&CK
- Intel CHIPSEC Framework
- Binarly Research
- Google Project Zero
- NIST SP 800-193
- US-CERT

---

## Author

**Maciej Gojny**

GG Advanced IT Security 

Website: https://ggsec.de

Specialization:

- Firmware Security
- Embedded Systems Auditing
- Supply Chain Security
- Advanced Threat Research

---

## Citation

If you use this research in academic work or professional publications, please cite:

```text
Gojny, M. (2026).
UEFI Attack Surface Research.
GGSEC Research White Paper.
Version 1.0.
