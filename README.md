# snort-ids-evasion-research

## Overview

This project investigates network scanning techniques and IDS evasion methods against a simulated enterprise environment protected by Snort IDS.

The objective was to evaluate how different reconnaissance techniques are detected, logged, or bypass detection mechanisms in a controlled cybersecurity laboratory environment.

Testing was performed on an isolated and authorized lab network.

---

## Lab Environment

| Component | Description |
|---|---|
| Attacker Machine | Kali Linux |
| Target Machine | Metasploitable |
| IDS Sensor | Ubuntu running Snort IDS |
| Analysis Tools | Nmap, Hping3, Wireshark, tcpdump |

---

## Techniques Tested

The research evaluated:

- TCP SYN scanning
- TCP Connect scanning
- UDP scanning
- FIN/NULL/XMAS scans
- Packet fragmentation techniques
- MTU manipulation
- Decoy scanning
- Source IP spoofing
- SYN flood behavior

---

## Key Findings

The testing showed that Snort successfully detected many traditional reconnaissance techniques.

However, techniques involving source obfuscation, decoys, and spoofing affected attacker attribution and demonstrated limitations of signature-based detection.

---

## Security Recommendations

- Regularly tune Snort detection rules
- Enable packet reassembly capabilities
- Combine signature detection with behavioral analysis
- Monitor abnormal network patterns
- Perform continuous IDS validation testing

---

## Documentation

Full project report:

`documentation/Snort_IDS_Evasion_Research_Report.docx`

---

## Disclaimer

This project was conducted strictly for educational purposes within an authorized isolated laboratory environment.
