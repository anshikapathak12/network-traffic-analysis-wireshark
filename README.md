 🌐 Network Traffic Analysis using Wireshark

## 📌 Project Overview
This project focuses on analyzing network traffic using Wireshark to identify suspicious and malicious activities.

The objective is to simulate a SOC Analyst's role in monitoring network packets and detecting anomalies such as unusual DNS queries, HTTP requests, and suspicious IP communication.

---

## 🎯 Objectives
- Capture and analyze network traffic
- Identify normal vs suspicious traffic
- Detect DNS anomalies and HTTP threats
- Investigate suspicious IP addresses
- Understand packet-level analysis

---

## 🛠 Tools Used
- Wireshark
- Kali Linux / Windows
- Public PCAP files (or captured traffic)

---

## 📂 Data Source
- Live network capture OR sample PCAP files

---

## 🔍 Key Filters Used

### 1. HTTP Traffic
```
http
```

### 2. DNS Traffic
```
dns
```

### 3. Suspicious Traffic (Unusual Ports)
```
tcp.port != 80 && tcp.port != 443
```

### 4. Filter by IP
```
ip.addr == 192.168.1.1
```

---

## ⚠️ Detection Techniques
- Unusual DNS queries (possible data exfiltration)
- Suspicious HTTP requests
- Traffic to unknown external IPs
- Uncommon port usage

---

## 📊 Analysis Findings
- Identified multiple DNS queries to suspicious domains
- Detected HTTP requests to unknown IP addresses
- Observed traffic on uncommon ports

---

## 🚨 Example Indicators of Compromise (IOCs)
- Suspicious IP: 203.0.113.5
- Unknown Domain: malicious-example.com
- Unusual Port: 8080 / 4444

---

## 🛡 Conclusion
This project demonstrates how packet analysis can help detect threats and improve network visibility for SOC operations.

---

## 📌 Future Improvements
- Integrate with IDS tools (Snort/Suricata)
- Automate alert generation
- Perform deep packet inspection (DPI)

---

## 👩‍💻 Author
Anshika Pathak
