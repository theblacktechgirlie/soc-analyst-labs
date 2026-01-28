# Brute-Force Attack Detection – Splunk Lab

## 📌 Objective
Detect potential brute-force authentication attacks by identifying high-volume failed login attempts across multiple user accounts from a single source IP.

---

## 🗂️ Data Source
- Authentication logs (simulated dataset)
- Ingested into Splunk for analysis

---

## 🔍 Detection Logic
This lab focuses on identifying:
- Excessive failed login attempts
- Multiple targeted user accounts
- Consistent source IP behavior
- Time-based attack patterns

---

## 🧪 Investigation Steps
1. Queried authentication logs for repeated failed login attempts
2. Grouped events by source IP and user
3. Identified IPs attempting logins across multiple accounts
4. Analyzed attempt volume and time window
5. Evaluated activity for brute-force indicators

---

## ⚠️ Findings
- One source IP generated a high volume of failed login attempts
- Multiple user accounts were targeted
- Activity occurred within a short time window
- Pattern aligned with brute-force behavior

---

## 🚨 Decision & Escalation
The activity was classified as a confirmed brute-force attack and escalated for containment, including IP blocking and account monitoring.

---

## 📝 Lessons Learned
- Brute-force attacks often target multiple accounts
- Time-window analysis is critical for detection
- Proper thresholds reduce false positives
- Clear documentation supports faster response
