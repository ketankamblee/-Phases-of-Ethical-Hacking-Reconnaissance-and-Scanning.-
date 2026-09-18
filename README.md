# -Phases-of-Ethical-Hacking-Reconnaissance-and-Scanning.-
Reconnaissance and Scaning of the target in authorised lab environment.


# ⚠️ 1. Liability Disclaimer
I have performed these activities only on the systems & devices where I had secured written permission or the devices/systems that I own myself. All these materials are for education and research purpose only. Do not use anything from here to break the law. The instructor, the authors and Networkwalks are not responsible for what you do with this knowledge. Every action you take is your own responsibility. Misuse can lead to criminal charges, heavy fines, loss of your job and a permanent record. In most countries unauthorised access is a crime even when nothing is damaged.

# 📌 2. Project Overview
In this Repository documents contains the 2nd week's project of Cybersecurity Internship Program at Networkwalks. It covers the first 2 phases of Ethical Hacking,  
1. Footprinting and Reconnaissance
2. Scanning

# 🛠️ 3. Tools and Resources Used

| Tools/Resources | Description |
| --- | --- |
| Kali Linux | An Operating system used by Cyber Security professionals for various ethical hacking purposes,  |
| Windows 11 | Common software used in most of PCs for GUI and CLI purposes |
| theHarvester | OSINT(Open Source Intelligence) reconnaissance tool will be using in Kali Linux |
| Zenmap(Nmap GUI) | GUI based network mapping tool, used for network scanning and mapping |  

# ⚙️ 4. Execution Process
Phase 1: Footprinting $ Reconnaissance using theHarvester for information gathering.  
- Task 1: In the task 1 we executed target search agianst microsoft.com. We used "Baidu" module with the limit 1000 of the output.

- Note: In the command,
  -d is used to understand syntax flags like domain selection
  -l used to limit result limits
  -b is used for data sources.

-Command:
theHarvester -d microsoft.com -l 1000 -b baidu  
<img width="947" height="817" alt="Screenshot 2026-09-18 183608" src="https://github.com/user-attachments/assets/d012d4be-40e2-487e-8551-4bd5630e3f78" />

-Task 2: In the tast 2 we will execute broader search on microsoft.com.  
-Command  
theHarvester -d microsoft.com -l 50 -b all

<img width="947" height="962" alt="starting the harvester" src="https://github.com/user-attachments/assets/1f1ede97-1bd1-45c1-80fd-f799d2943c83" />

Phase 2: Scanning Networks.  
1. Open windows command prompt, type command ipconfig and hit enter:
   By doing this we can find our local IP address, Subnet mask, and Default gateway.

<img width="807" height="957" alt="Screenshot 2026-09-18 191926" src="https://github.com/user-attachments/assets/8d17f0bc-61ce-424f-b706-0631b4aabe4b" />

2. Open Zenmap enter local subnet range, select Ping scan profile and start the Scan:
   Zenmap will scan the local network and provide the available hosts and open ports on the network.
<img width="1917" height="728" alt="Screenshot 2026-09-18 192245" src="https://github.com/user-attachments/assets/7a2794ec-4e0d-4b86-888b-5a45f9ad030e" />

3. Locate the Topology tab and head to fisheye:
   In this tab we will find the topology of the network.

<img width="1917" height="1078" alt="Screenshot 2026-09-18 192738" src="https://github.com/user-attachments/assets/abb6e3b7-ab2b-47c1-ac18-dfe4cc2a72a1" />

# 🚩 Challenges Encountered and Soulutions
1. Problem:
   Due to slow network speed in the Kali Linux Lab theHarvester scan was dismissed and the terminal was freezed.

2. Solution:
   Reviewed the network settings and repaired the subnet range and restarted the Linux lab.

#  🛠️ Resource Used
- Kali Linux 2026.2 :- https://kali.org/get-kali
- theHarvester :- OSINT and Footprinting tool
- Zenmap :- https://nmap.org/download.html

# 👤 Author
Ketan Kamble  
Cyber Security and Forensics Student  
LinkedIn: https://www.linkedin.com/in/ketan-kamble-237a63316/

# 🗂️ Project Information
Program Name: Cybersecurity at Networkwalks | Week: 02 | Project: Penetration Testing Report: Footprinting & Network Scanning (theHarvester & Zenmap)| Repository: GitHub
