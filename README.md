# 🔐 Data Exfiltration Detection

Hands-on analysis of data exfiltration techniques including **DNS, FTP, HTTP, and ICMP traffic** in a controlled cybersecurity lab environment.

This project focuses on identifying suspicious network behavior, analyzing traffic with security tools, and understanding how SOC analysts can detect potential data exfiltration.

---

## 📌 Topics Covered

### 🌐 DNS Exfiltration

Analysis of suspicious DNS traffic and indicators that may suggest data exfiltration through DNS queries.

➡️ [View DNS Analysis](./DNS-Exfiltration/analysis.md)

**Tools:** Wireshark, Splunk

---

### 📁 FTP Exfiltration

Analysis of FTP traffic to identify suspicious file transfer and authentication activity.

➡️ [View FTP Analysis](./FTP-Exfiltration/analysis.md)

**Tools:** Wireshark

---

### 🌍 HTTP Exfiltration

Analysis of HTTP POST requests and unusually large HTTP transfers that may indicate data uploads to external destinations.

➡️ [View HTTP Analysis](./HTTP-Exfiltration/analysis.md)

**Tools:** Wireshark, Splunk

---

### 📡 ICMP Exfiltration

Analysis of unusually large ICMP packets and investigation of potentially encoded payload data.

➡️ [View ICMP Analysis](./ICMP-Exfiltration/analysis.md)

**Tools:** Wireshark, CyberChef

---

## 🔎 Detection Perspective

The project demonstrates several network indicators that can help a SOC analyst investigate potential data exfiltration:

* Unusually large network packets.
* High volumes of specific protocol traffic.
* Suspicious DNS queries.
* Large HTTP POST requests.
* Suspicious FTP file-transfer activity.
* Encoded or unusual payload content.
* Unexpected external destinations.
* Repeated communication patterns.

Detection should rely on correlating multiple indicators and understanding the normal behavior of the environment.

---

## 🛡️ Defensive Measures

Organizations can reduce the risk of data exfiltration by implementing:

* Network traffic monitoring.
* DNS monitoring and logging.
* HTTP/HTTPS traffic inspection where appropriate.
* Egress filtering.
* Firewall and proxy controls.
* IDS/IPS monitoring.
* SIEM-based detection and alerting.
* Monitoring unusual outbound data transfers.
* Endpoint and network behavioral analysis.

---

## 🧠 What I Learned

Through this lab, I practiced:

* Network traffic analysis with Wireshark.
* DNS traffic investigation.
* FTP traffic analysis.
* HTTP POST and large-transfer detection.
* ICMP traffic analysis.
* Log analysis using Splunk.
* Payload investigation using CyberChef.
* Identifying indicators of potential data exfiltration.
* Thinking from a SOC detection perspective.
* Correlating network and log-based evidence.

---

## 🧪 Lab Environment

| Item        | Details                      |
| ----------- | ---------------------------- |
| Platform    | TryHackMe                    |
| Room        | Data Exfiltration Detection  |
| Focus       | Network Traffic Analysis     |
| Tools       | Wireshark, Splunk, CyberChef |
| Environment | Controlled Cybersecurity Lab |

---

## 📂 Project Structure

```text
Data-Exfiltration-Detection/
│
├── README.md
│
├── DNS-Exfiltration/
│   ├── analysis.md
│   ├── dns-frame-len.png
│   ├── dns-no-response.png
│   ├── splunk-analysis-dns.png
│   └── splunk-dns-2.png
│
├── FTP-Exfiltration/
│   ├── analysis.md
│   ├── ftp-stor.png
│   └── ftp-user-pass.png
│
├── HTTP-Exfiltration/
│   ├── analysis.md
│   ├── http-logs.png
│   ├── http-large-post-splunk.png
│   └── http-large-post-wireshark.png
│
└── ICMP-Exfiltration/
    ├── analysis.md
    ├── icmp-large-packets.png
    └── icmp-cyberchef.png
```

---

## ⚠️ Disclaimer

This project was performed in a controlled cybersecurity learning environment for educational and defensive security purposes.

The techniques and analysis presented here are intended to improve network monitoring, threat detection, and SOC investigation skills.

