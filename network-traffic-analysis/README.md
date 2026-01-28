# Network Traffic Analysis – Wireshark Lab

## 📌 Objective
Analyze network traffic using Wireshark to identify suspicious behavior, including abnormal DNS queries and HTTP activity.

---

## 📁 Data Source
- Packet capture (PCAP file)
- Analyzed using Wireshark

---

## 🔍 Investigation Steps
1. Opened the PCAP file in Wireshark
2. Applied display filters to isolate DNS and HTTP traffic
3. Reviewed DNS queries for suspicious domains
4. Analyzed HTTP requests and responses for anomalies
5. Identified indicators of potential malicious activity

---

## 🛠 Tools Used
- Wireshark
- PCAP analysis
- Network protocol analysis (DNS, HTTP)

---

## ⚠️ Findings
- Observed repeated DNS queries to uncommon domains
- Identified clear-text HTTP traffic containing suspicious requests
- Traffic patterns suggested possible command-and-control behavior

---

## 🚨 Decision & Escalation
The activity was classified as suspicious and would be escalated to a Tier 2 SOC analyst for deeper investigation.

---

## 📚 Lessons Learned
- Importance of filtering traffic to reduce noise
- Value of DNS analysis in detecting malicious activity
- Reinforced understanding of network protocol behavior

