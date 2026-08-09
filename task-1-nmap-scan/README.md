# Task 1 – Basic Network Scanning with Nmap

**Prepared by:** Yuvaraj S
**Internship:** Cybersecurity Internship
**Environment:** Kali Linux Virtual Machine
**Target System:** Localhost (`127.0.0.1`)
**Task Type:** Practical – Network Reconnaissance
**Status:** Completed

---

# Objective

The objective of this task was to perform basic network reconnaissance using Nmap on a controlled local environment. The assessment involved identifying open ports, detecting running services, attempting operating system identification, and documenting the results with a professional security analysis. The activity was conducted entirely within a Kali Linux virtual machine using the localhost address (`127.0.0.1`) to ensure safe and ethical testing.

---

# Introduction

Network scanning is one of the first steps in a security assessment. It helps security professionals understand which services are exposed on a system and whether those services could increase the attack surface. Nmap (Network Mapper) is a widely used open-source tool for network discovery and security auditing. In this task, Nmap was used to perform a basic TCP scan, a service version scan, and an operating system detection scan against the local machine.

---

# Tools and Environment

The following tools and environment were used during the assessment:

* **Operating System:** Kali Linux
* **Tool:** Nmap 7.99
* **Interface:** Linux Terminal
* **Target:** `127.0.0.1`

The assessment was performed in a virtual machine environment to maintain isolation from external networks.

---

# Commands Executed

The following Nmap commands were executed:

```bash
nmap 127.0.0.1
nmap -sV 127.0.0.1
sudo nmap -O 127.0.0.1
```

Each command served a different purpose:

* `nmap` performs a basic port scan.
* `-sV` attempts service and version detection.
* `-O` attempts operating system fingerprinting.

---

# Scan Results

## Basic TCP Scan

The basic scan reported that all 1000 commonly scanned TCP ports were closed.

### Result

* Host status: **Up**
* Open ports found: **0**
* Closed ports: **1000**

This indicates that no network services were listening for incoming TCP connections on the localhost interface at the time of the scan.

---

## Service Version Detection

The service version scan did not identify any running services because no ports were open.

### Result

* Services detected: **None**
* Version information: **Not available**

Since there were no listening services, Nmap could not perform service fingerprinting.

---

## Operating System Detection

The operating system detection scan was executed with root privileges. Nmap reported that too many fingerprints matched the target to provide a reliable operating system identification.

### Result

* OS identification: **Inconclusive**
* Network distance: **0 hops**

Because all scanned ports were closed, Nmap had insufficient fingerprinting data to identify the operating system with confidence.

---

# Security Analysis

The scan results suggest that the localhost interface had a minimal exposed network surface during the assessment. No open TCP ports were discovered, which reduces the likelihood of remote network-based attacks against services such as SSH, HTTP, FTP, or database servers.

The absence of detectable services is generally a positive security indicator because unnecessary services are not exposed. However, a secure system depends on multiple factors including patch management, local access controls, authentication mechanisms, and system configuration. Port closure alone does not guarantee overall system security.

The inconclusive OS detection result is expected when scanning a localhost interface with no open ports, as Nmap relies heavily on responses from network services for accurate fingerprinting.

---

# Evidence Collected

The following evidence files are included in this task folder.

## Screenshots

* `screenshots/ip_address.png`
* `screenshots/basic_scan.png`
* `screenshots/service_scan.png`
* `screenshots/os_scan.png`

## Output Files

* `nmap_scan_results.txt`

These files provide verifiable proof of the commands executed and the results obtained during the assessment.

---

# Ethical Considerations

This activity was performed exclusively against the local machine (`127.0.0.1`) within a personal Kali Linux virtual machine environment. No external systems, public IP addresses, institutional networks, or third-party services were scanned. The task was conducted in accordance with ethical cybersecurity practices and the internship guidelines.

---

# Learning Outcome

This task improved my understanding of:

* Network reconnaissance methodology
* TCP port states in Nmap
* Service version detection
* Operating system fingerprinting
* Security interpretation of scan results
* Evidence collection and technical documentation
* Ethical use of security assessment tools

The exercise also provided practical experience with Kali Linux and command-line security tools.

---

# Conclusion

The Nmap assessment successfully demonstrated the process of conducting a basic network scan in a controlled environment. All scanned TCP ports on localhost were closed, no services were detected, and operating system identification was inconclusive due to the absence of fingerprintable network responses. The task provided valuable hands-on experience with network reconnaissance techniques and reinforced the importance of ethical testing, evidence collection, and professional cybersecurity reporting.

---

# Personal Reflection

Completing this task strengthened my practical cybersecurity skills and increased my confidence in using Nmap for network reconnaissance. I learned how to interpret scan results professionally and how to document technical findings in a clear and structured manner suitable for internship and academic submissions.
