# Python Security Scripts

A collection of Python utilities developed during hands-on security training. Scripts cover data encoding, protocol basics, and lightweight network reconnaissance — written for learning-by-doing and applied in lab environments.

---

## Repository Structure

```
python-security-scripts/
├── pre-security/        # Scripts developed during TryHackMe Pre Security path
│   ├── data_encoding/   # Base64, hex, binary encoding/decoding utilities
│   ├── sql_basics/      # SQL query demo: SELECT, filtering, basic injection patterns
│   └── port_checker/    # Simple TCP port checker using socket module
└── tools/               # Standalone reusable utilities
    ├── log_parser/      # Parse and filter common log formats
    └── ip_checker/      # IP geolocation and reputation lookup
```

---

## Scripts Overview

### `pre-security/data_encoding/`
Demonstrates encoding schemes used across web and network protocols: Base64, hexadecimal, and binary representation. Covers encoding vs encryption distinction — a common point of confusion in early security work.

### `pre-security/sql_basics/`
SQL query demonstration: constructing SELECT statements, filtering with WHERE clauses, and illustrating how improper input handling leads to SQL injection. Used as a conceptual foundation before studying web application attacks.

### `pre-security/port_checker/`
A minimal TCP port scanner using Python’s `socket` module. Accepts a target IP and a list of ports, returns open/closed status. Built to understand the mechanics behind tools like Nmap at the protocol level.

### `tools/log_parser/`
Parses common log formats (Apache, Windows Event Log, syslog). Extracts timestamps, source IPs, status codes, and event types. Useful as a lightweight pre-processing step before feeding logs into a SIEM.

### `tools/ip_checker/`
Looks up IP address metadata using public APIs (geolocation, ASN, abuse reputation). Intended for quick triage of suspicious IPs during incident investigation.

---

## Skills Demonstrated

- Python 3 standard library (`socket`, `re`, `json`, `base64`)
- Log parsing and pattern matching with regex
- Basic network programming concepts
- SQL fundamentals applied to security context
- CLI-style tool design

---

## Certifications & Training

| Credential | Platform | Date |
|---|---|---|
| Pre Security Path | TryHackMe | Jul 2026 |
| Cyber Security 101 | TryHackMe | In progress |

Certificate: [THM-DRP2APT1BY](https://tryhackme.com/certificate/THM-DRP2APT1BY)
