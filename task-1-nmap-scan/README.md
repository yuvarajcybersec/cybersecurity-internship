# Task 1 – Basic Network Scanning with Nmap

**Prepared by:** Yuvaraj S
**Internship:** Cybersecurity Internship
**Environment:** Kali Linux (Virtual Machine)
**Target:** Localhost (`127.0.0.1`)

---

## Objective

The objective of this task was to perform basic network reconnaissance on a local machine using Nmap, identify open ports and services, attempt operating system detection, and document the findings with a security analysis.

---

## Tools Used

* Nmap 7.99
* Kali Linux
* Linux Terminal

---

## Commands Executed

```bash
nmap 127.0.0.1
nmap -sV 127.0.0.1
sudo nmap -O 127.0.0.1
```

---

## Scan Results Summary

| Scan Type            | Result                              |
| -------------------- | ----------------------------------- |
| Basic Scan           | No open TCP ports found             |
| Service Version Scan | No services detected                |
| OS Detection Scan    | OS could not be reliably identified |

---

## Security Analysis

### Basic Scan

All 1000 common TCP ports were closed. No network services were listening for incoming connections on localhost, which reduces the attack surface.

### Service Version Scan

Because no ports were open, Nmap could not identify any service versions. This indicates that unnecessary network services were not exposed during the assessment.

### OS Detection Scan

Nmap could not determine a specific operating system fingerprint because all scanned ports were closed. The scan confirmed that the target was the local machine (network distance: 0 hops).

---

## Evidence Files

### Screenshots

* `screenshots/ip_address.png`
* `screenshots/basic_scan.png`
* `screenshots/service_scan.png`
* `screenshots/os_scan.png`

### Output File

* `nmap_scan_results.txt`

---

## Ethical Considerations

This assessment was performed only against the local machine (`127.0.0..1`) in a controlled Kali Linux virtual machine environment. No external systems were scanned.

---

## Learning Outcome

This task improved my understanding of:

* Network reconnaissance
* Port states in Nmap
* Service detection
* Operating system fingerprinting
* Security analysis of exposed services
* Ethical use of scanning tools

