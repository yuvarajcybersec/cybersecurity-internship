# Common Network Security Threats Report

**Prepared by:** Yuvaraj S
**Internship:** Cybersecurity Internship
**Task:** Task 4 – Research Report
**Date:** August 2026

---

# Introduction

Modern organizations depend heavily on computer networks for communication, cloud services, financial transactions, and business operations. As networks become more connected, they also become more exposed to cyber threats. Attackers target networks to steal data, disrupt services, intercept communications, or gain unauthorized access. Understanding common network security threats and their mitigation strategies is essential for maintaining confidentiality, integrity, and availability of information systems.

---

# 1. Denial-of-Service (DoS) and Distributed Denial-of-Service (DDoS) Attacks

## How the Attack Works

A DoS attack attempts to make a system or network service unavailable by overwhelming it with excessive traffic or resource requests. A DDoS attack uses many compromised devices (a botnet) to generate traffic simultaneously, making the attack more powerful and difficult to block.

## Real-World Example

In 2016, the Mirai botnet launched a major DDoS attack against Dyn, a DNS service provider. The attack disrupted access to popular websites and online services across multiple countries.

## Impact

* Website and application outages
* Financial losses from downtime
* Loss of customer trust
* Increased operational costs

## Mitigation Strategies

1. Use DDoS protection services and content delivery networks (CDNs).
2. Implement rate limiting and traffic filtering.
3. Maintain scalable infrastructure and redundancy.

---

# 2. Man-in-the-Middle (MITM) Attacks

## How the Attack Works

In a MITM attack, an attacker intercepts communication between two parties and may read, modify, or inject data without the users noticing.

## Real-World Example

Attackers have used rogue Wi-Fi hotspots in public places to intercept user traffic and steal login credentials from unencrypted sessions.

## Impact

* Credential theft
* Session hijacking
* Data manipulation
* Privacy violations

## Mitigation Strategies

1. Use HTTPS and TLS encryption.
2. Avoid connecting to untrusted public Wi-Fi networks.
3. Use VPNs when accessing sensitive services on public networks.

---

# 3. IP Spoofing

## How the Attack Works

IP spoofing involves forging the source IP address in network packets to impersonate another device or hide the attacker's identity.

## Real-World Example

IP spoofing has been widely used in reflection and amplification DDoS attacks, where attackers send requests with a forged victim IP address to third-party servers.

## Impact

* Difficulty tracing attackers
* Unauthorized network access attempts
* Participation in larger DDoS attacks

## Mitigation Strategies

1. Implement ingress and egress filtering on routers.
2. Use packet filtering and anti-spoofing controls.
3. Monitor network traffic for abnormal source addresses.

---

# 4. DNS Poisoning (DNS Spoofing)

## How the Attack Works

DNS poisoning corrupts DNS records so that users are redirected to malicious websites even when they type legitimate domain names.

## Real-World Example

Attackers have compromised DNS infrastructure to redirect users of legitimate websites to phishing pages designed to steal credentials.

## Impact

* Credential theft
* Malware distribution
* Loss of trust in online services

## Mitigation Strategies

1. Deploy DNSSEC (Domain Name System Security Extensions).
2. Use secure DNS resolvers from trusted providers.
3. Monitor DNS records and infrastructure for unauthorized changes.

---

# Comparison of Threats

| Threat        | Attack Vector             | Primary Target         | Difficulty | Ease of Mitigation |
| ------------- | ------------------------- | ---------------------- | ---------- | ------------------ |
| DoS/DDoS      | Excessive traffic         | Servers and websites   | Medium     | Medium             |
| MITM          | Intercepted communication | Users and applications | Medium     | High               |
| IP Spoofing   | Forged packets            | Networks and services  | Medium     | Medium             |
| DNS Poisoning | Manipulated DNS records   | Internet users         | Medium     | Medium             |

---

# Key Takeaways for Network Administrators

1. Encrypt network communications whenever possible.
2. Monitor network traffic continuously for anomalies.
3. Keep DNS infrastructure and network devices securely configured and updated.
4. Implement layered security controls rather than relying on a single defense.
5. Prepare incident response procedures for network-based attacks.

---

# Conclusion

Network security threats such as DDoS attacks, MITM attacks, IP spoofing, and DNS poisoning can significantly disrupt business operations and compromise sensitive information. While each threat uses different techniques, they can all be mitigated through a combination of secure network design, encryption, monitoring, filtering, and administrative controls. A proactive defense strategy and regular security assessments are essential for protecting modern network environments.

---

# References

1. National Institute of Standards and Technology (NIST). https://www.nist.gov
2. Cybersecurity and Infrastructure Security Agency (CISA). https://www.cisa.gov
3. SANS Institute Reading Room. https://www.sans.org/reading-room
4. MITRE ATT&CK Framework. https://attack.mitre.org
5. Krebs on Security. https://krebsonsecurity.com

