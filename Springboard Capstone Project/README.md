


As part of a hands-on penetration testing lab, I conducted a full network vulnerability assessment using Kali Linux tools such as Nmap, Zenmap, and OpenVAS. The first phase involved reconnaissance and host discovery using Nmap commands like nmap -sn 192.168.1.0/24 to identify live hosts on the network, followed by more detailed scans using nmap -sV and nmap -A to enumerate open ports, services, and operating systems. Zenmap was also utilized to visualize scan results and manage scanning profiles via its GUI. In the second phase, I used OpenVAS (Open Vulnerability Assessment System) to perform in-depth vulnerability scans by first initializing the scanner with sudo gvm-setup and starting the web interface at https://127.0.0.1:9392. After updating the Greenbone Community Feed to include over 50,000 known vulnerabilities, I configured and launched scan tasks on discovered targets. The resulting reports provided detailed insights into detected vulnerabilities, including CVE identifiers, severity ratings, and remediation recommendations. Through this lab, I gained practical experience with the first two phases of the penetration testing lifecycle—reconnaissance and scanning—and developed skills in interpreting scan outputs, assessing network security posture, and identifying actionable steps for remediation.

<img width="544" height="373" alt="image" src="https://github.com/user-attachments/assets/8a6c6a57-15d7-4aca-a6c4-442118be5e10" />



<img width="560" height="314" alt="image" src="https://github.com/user-attachments/assets/9cdc6c0d-5651-4d24-8316-eeeaf04445ae" />




