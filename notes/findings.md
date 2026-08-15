# Findings & Analysis

## 01 — Host Discovery

### What I Learned:

- How to determine whether a host is reachable.
- What Nmap's `-sn` option does.
- How host discovery can be performed before examining individual ports.
- How Nmap reports whether a target appears to be up.

### Security Relevance:

Host discovery helps identify active systems within an authorized network before further security assessment.

---

## 02 — Port Scanning

### What I Learned:

- How to scan all TCP ports using Nmap's `-p-` option.
- How Nmap identifies different port states.
- The difference between **open, closed, and filtered** ports.
- How firewalls and network filtering can affect scan results.

### Security Relevance:

Port scanning helps security analysts identify potentially accessible network services and understand the attack surface of an authorized system.

---

## 03 — Service & Version Detection

### What I Learned:

- How to use Nmap's `-sV` option.
- How Nmap attempts to identify services and their versions.
- That filtered ports can prevent service and version information from being obtained.

### Security Relevance:

Service and version identification can help security analysts understand what software is exposed on a system and identify areas that may require further security assessment.

---

## 04 — OS Detection

### What I Learned:

- How to use Nmap's `-O` option for OS fingerprinting.
- How Nmap uses network responses to generate possible OS/device fingerprints.
- That OS detection may be unreliable when suitable open and closed ports are unavailable.

### Security Relevance:

OS identification can help analysts understand the technology environment of an authorized system and determine appropriate areas for further assessment.

---

## 05 — Comprehensive Scan

### What I Learned:

- How to use Nmap's `-A` option for broader reconnaissance.
- How Nmap can combine OS detection, service/version detection, NSE scripts, and traceroute.
- That comprehensive scans can still produce limited results when network ports are filtered.
- The importance of interpreting automated scan results carefully.

### Security Relevance:

Comprehensive scanning can provide security analysts with a broader view of an authorized target and help identify information that may require further investigation.

---

## Overall Learning

This lab helped me understand the progression of network reconnaissance using Nmap, from **host discovery to port scanning, service detection, OS fingerprinting, and comprehensive scanning**.

The exercises also demonstrated that scan results depend on how the target responds and that Nmap output should be **interpreted rather than treated as definitive**.
