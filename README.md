Network & Web Security Testing – Internship Project

📌 Overview

This project documents a structured security assessment performed on a web application during my cybersecurity internship. The assessment focused on network reconnaissance, directory enumeration, and traffic analysis.

⚠️ All testing was conducted in an authorized environment with proper permission.

🎯 Scope of Assessment

● Identify exposed network ports
● Discover hidden directories and endpoints
● Analyze unencrypted network traffic
● Document findings and remediation steps


🛠 Tools Used

● Nmap – Port Scanning
● Dirb – Directory Brute-forcing
● Wireshark – Network Traffic Analysis
● Kali Linux


🔎 Phase 1 – Port Enumeration

Method:
-> nmap -Pn -p- testphp.vulnweb.com

Findings:
● Open HTTP/HTTPS ports
● Additional exposed service (if any)
● Service version detection



📂 Phase 2 – Directory Brute Force
-> dirb http://testphp.vulnweb.com/

Findings:
● Hidden admin panel
● Backup directory
● Sensitive endpoints


📡 Phase 3 – Traffic Interception & Analysis

Analysis Focus:
● HTTP requests & responses
● Unencrypted credentials 
● Cookie/session data
● Packet-level inspection


🛑 Security Risks Identified
● Open unnecessary ports
● Exposed sensitive directories
● Transmission of data over HTTP (no encryption)


🛡 Remediation Recommendations
● Close unused ports
● Disable directory indexing
● Enforce HTTPS with TLS
● Implement WAF
● Restrict admin panel access


📊 Risk Summary

| Issue               | Severity | Impact                   |
| ------------------- | -------- | ------------------------ |
| Open Port Exposure  | Medium   | Attack surface increase  |
| Hidden Admin Panel  | High     | Unauthorized access risk |
| Unencrypted Traffic | Critical | Credential interception  |


⚖️ Ethical Disclaimer

This assessment was conducted under authorized internship supervision. The purpose of this project is educational documentation and defensive security awareness.


🚀 Step 4: VERY IMPORTANT – Protect Yourself

Never:
❌ Put real domain name
❌ Upload sensitive captured packets
❌ Upload real credentials
❌ Mention company name (unless permitted)







