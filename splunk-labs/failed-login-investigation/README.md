# Failed Login Investigation – Splunk Lab

## 📌 Objective  
Investigate multiple failed login attempts to determine whether the activity represents a potential brute-force attack or a false positive.

---

## 🗂️ Data Source  
- Authentication logs (simulated dataset)  
- Ingested into Splunk for analysis  

---

## 🔎 Investigation Steps  
1. Reviewed alert indicating multiple failed login attempts from a single IP address  
2. Verified whether the account was a user account or service account  
3. Checked whether a successful login occurred after the failed attempts  
4. Identified source IP address and determined whether it was internal or external  
5. Correlated authentication events to identify attack patterns  

---

---

## 🧪 SPL Queries Used  

```spl
index=security action=failure
| stats count by user, src_ip

```
📄 Full query set: [queries.txt](queries.txt)

## ⚠️ Findings  
- Multiple failed login attempts detected targeting a single user account  
- Source IP identified as external  
- No successful login observed following the failed attempts  

---

## 🚨 Decision & Escalation  
Based on the volume and pattern of failed attempts, the activity was classified as suspicious and escalated according to incident response procedures.

---

## 📝 Lessons Learned  
- Importance of validating context before escalation  
- Value of correlating authentication events with IP sources
- Reinforced proper documentation and evidence preservation
