Practical labs and reconnaissance exercises completed during Week 2 of my Cybersecurity Internship at Networkwalks, covering OSINT, passive/active reconnaissance, and network scanning.
# Cybersecurity Internship – Week 2: Reconnaissance & Network Scanning
This repository documents the practical labs and exercises I completed during Week 2 of my Cybersecurity Internship with Networkwalks. Throughout the week, I progressed step-by-step from setting up my testing environment to performing passive OSINT, command-line reconnaissance, and active local network scanning.

## Practical Module 1 (PM1): Footprinting & Reconnaissance with Multiple Kali Tools
In this module, I footprinted the live website `networkwalks.com` using multiple built-in Kali Linux command-line tools to gather domain registration details, web server technologies, DNS records, headers, and firewall status.

* **Task 1: WHOIS Lookup** – Queried public domain registration records to find ownership, registrar info, and name servers (`whois networkwalks.com`).
Whois Scan Part 1 : <img width="1364" height="667" alt="ss1" src="https://github.com/user-attachments/assets/da97a099-a5ea-498e-9beb-40f3c51052d9" />
Whois Scan Part 2: <img width="1365" height="663" alt="ss2" src="https://github.com/user-attachments/assets/85870cbc-7bb0-4976-b0fc-a9e299d5b6a4" />
Whois Scan Part 3: <img width="1365" height="664" alt="ss3" src="https://github.com/user-attachments/assets/d8885bd8-6c20-4419-83e5-c353e15f05ec" />
Whois Scan Part 4: <img width="1364" height="663" alt="ss4" src="https://github.com/user-attachments/assets/e6709220-0134-4e48-b168-413137c8ab8f" />

* **Task 2: WhatWeb Fingerprinting** – Identified web technologies, CMS versions, and server headers (`whatweb networkwalks.com`).
  Whatweb Scan: <img width="1365" height="669" alt="ss5" src="https://github.com/user-attachments/assets/d4084ce2-045c-4d98-b683-8b03331fbe51" />
  
* **Task 3: NSLookup** – Resolved the target domain name to its corresponding IP address (`nslookup networkwalks.com`).
  Nslookup Result: <img width="1364" height="668" alt="ss6" src="https://github.com/user-attachments/assets/1934abe0-b06f-4ebf-8f42-49902f3d9a34" />
* **Task 4: Curl Header Inspection** – Inspected raw HTTP response headers (`curl -I https://networkwalks.com`).
  Curl Command: <img width="1361" height="669" alt="ss7" src="https://github.com/user-attachments/assets/dd557bbc-f0e6-4a43-a1b6-b687e1127bc3" />

* **Task 5: WafW00F Firewall Detection** – Detected whether the target website is protected by a Web Application Firewall (`wafw00f networkwalks.com`).
  Wafw00f Scan: <img width="1365" height="668" alt="ss8" src="https://github.com/user-attachments/assets/639a56e8-f288-4849-bf75-81d15de2bd23" />

* **Task 6: DNSRecon Enumeration** – Enumerated all DNS records, name servers, mail servers, and service records (`dnsrecon -d networkwalks.com`).
 Dnsrecon Result: <img width="1361" height="637" alt="ss9(b)" src="https://github.com/user-attachments/assets/a6c8ad68-4f55-46fd-8130-0db60c5a9ee0" />
<img width="1362" height="644" alt="ss 9(a)" src="https://github.com/user-attachments/assets/d3a16d1d-f7e9-498d-99bc-47d18feefac5" />

## Practical Module 2 (PM2): Footprinting & Reconnaissance Attacks with GHDB
In this module, I explored the Google Hacking Database (GHDB) hosted on Exploit-DB to perform passive reconnaissance using advanced search operators (Google Dorks).
* Practiced finding exposed live vulnerable security cameras and open web directories containing downloadable mathematics ebooks in PDF format.

GHDB Interface: <img width="1363" height="726" alt="pm2 ss1" src="https://github.com/user-attachments/assets/dbf48ffe-7057-4fdd-a0be-9f6e7cc2c535" />
 Open Directory Search: <img width="1358" height="763" alt="pm2 ss2" src="https://github.com/user-attachments/assets/fbac8034-a805-47a0-adce-6737b85d1265" />
 Directory Contents: <img width="1359" height="767" alt="pm2 ss4" src="https://github.com/user-attachments/assets/65d55523-0e3c-496d-b5a5-f24ff0a64ed4" />
<img width="1365" height="767" alt="pm2 ss3" src="https://github.com/user-attachments/assets/0e69c520-b5c8-470e-bc02-277168db8d47" />

---

## Practical Module 3 (PM3): Footprinting & Reconnaissance with Maltego
In PM3, I installed and configured **Maltego** on a Windows environment to perform visual link analysis and OSINT gathering.
* Created a Maltego ID, ran initial transforms on `networkwalks.com`, and mapped domain relationships, infrastructure records, and associated email addresses.

 Maltego Setup Workspace: <img width="1365" height="716" alt="pm 3 ss2" src="https://github.com/user-attachments/assets/91448a33-80da-4d40-9dcc-a76dc4cd8a92" />

 Domain Entity Drag and Drop: <img width="1357" height="720" alt="pm3 ss1" src="https://github.com/user-attachments/assets/bdbba9c5-a22f-4f9c-9d22-25a14bd2a1e1" />

 Maltego Transform Graph Output: <img width="1365" height="718" alt="pm3 ss3" src="https://github.com/user-attachments/assets/5980176a-a11e-4ff2-b1ee-743c0b72fd6c" />
 
---
## Practical Module 4 (PM4): Footprinting & Reconnaissance with theHarvester
In this module, I used **theHarvester** in Kali Linux to collect emails, sub-domains, and host details from public search engines without directly touching the target.
* Ran searches against Microsoft using Baidu (`-b baidu -l 1000`) and all available public sources (`-b all -l 50`).

 theHarvester Baidu Search Result: <img width="1362" height="664" alt="pm4 ss2" src="https://github.com/user-attachments/assets/6bff3eb2-24c0-45e8-ba8e-07023cd420c6" />

 theHarvester All Sources Execution: <img width="1365" height="663" alt="pm4 ss1" src="https://github.com/user-attachments/assets/683c11dc-7f49-4203-acd8-bd80521d2d0f" />

---
## Practical Module 5 (PM5): Local Network Scanning with Nmap & Zenmap
In the final module of the week, I shifted from external OSINT to active local subnet scanning and configuration verification:
* Inspected Windows local network configuration, IP address, subnet mask, and physical MAC address using `ipconfig` and `ipconfig /all`.
* Installed **Nmap/Zenmap** and executed Ping Scans across the local subnet to discover active hosts.
* Exported the visual **Network Topology** map as a PDF (`zenmap-topology.pdf`).

Windows IP Config and MAC Address Check: <img width="1308" height="612" alt="ss cmd" src="https://github.com/user-attachments/assets/20476d5a-e36e-41b3-95f3-40d4f9b6ae21" />
 
Zenmap Subnet Scan and GUI Workspace: <img width="1365" height="715" alt="pm5 ss3" src="https://github.com/user-attachments/assets/3ea8d3b1-395b-45db-92f1-bc4cf4d72aba" />

---
## Repository Contents
* `/Screenshots` – Organized lab proofs corresponding to PM1 through PM5.
* `zenmap-topology.pdf` – Network topology map exported from Zenmap.

---
*Disclaimer: All reconnaissance, OSINT, and scanning activities were performed strictly for educational purposes within authorized environments.*
