# NETWORKWALKS-DATUS-B084-WK1-PM1-SOC-LAB-WIRESHARK-EXTRA-
<div align="center">
#🦈SOC LAB Wireshark (EXTRA)🦈

**Capturing  and Analyzing the Packets in the Network using Tool know as Wireshark to  in order to identify the attackers , hidden data, Username & passwords,Catch the Brute Force Attacker and and scam call**
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ver-Virtualbox%20v7.2-0070C0?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Penetration%20Testing-C00000?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Virtualization-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/GitHub-404040?style=flat-square&labelColor=0070C0&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/NetworkWalks-404040?style=flat-square&labelColor=C00000" />
  
</p>

## 🛡️ Project Overview

This project focuses on **Capturing and analyzing Network Packets on the Network in the Pre-established Lab as SOC analyst** using a Tool know as **_Wireshark_** which is commonly used by the Network Engineers on troubleshooting and Cyber security Engineer to check the vulnerabilities in the systems connected on the network.

## Wireshark

🔗 Wireshark https://www.wireshark.org/download.html
<img width="918" height="623" alt="Lab" src="https://github.com/user-attachments/assets/8b75916c-cce3-46e0-99ea-b568cc74ccd2" />


## 🔭 Objectives
The main objectives of this SOC Labs project are to:
- To identify the attacker's IP.
- To Follow TCP Stream to Capture and find the  Hidden data in the packets on the Network.
- To check & identify the unsecure Network protocols that's reveal/show the Username and password.
- To Catch the Brute Force Attacker.
- To Catch the Call Scammer on VOIP in the Network.

# 🔎Identify the attacker's IP

The Lab Network topology was provides as per below diagram of the SOC LAB with Webserver (_IP 192.168.10.20_), SOC Analyst (_IP 192.168.10.10_), **Attacker (_IP Unknown_)**, Network switch  and other host which all are connected to the Switch thru Wired (_Ethernet_)/ Wireless(_Wi-fi_).
<img width="1250" height="676" alt="3 SOC LAB Identify Attacker I" src="https://github.com/user-attachments/assets/388b17ed-1064-45f9-bbb8-f1eb36d16604" />


The Packet analysis was done and the Attacker was identified with Ip **(_192.168.10.66_)** with port **52311** who was try to access service from the server (_192.168.10.20_) through different ports as indicated in packet analysis shown below,
<img width="1366" height="784" alt="3 SOC LAB Identify Attacker II" src="https://github.com/user-attachments/assets/257f0649-79ab-44a4-9405-f827e3a2055d" />

# 👣 Following TCP Stream to Capture and find the  Hidden data
The Lab Network topology was provides as per below diagram of the SOC LAB with Webserver (_IP 192.168.10.20_), SOC Analyst (_IP 192.168.10.10_), **Staff PC (_IP Unknown_)** , Network switch  and other host which all are connected to the Switch thru Wired (_Ethernet_)/ Wireless(_Wi-fi_).
![Uploading 4.SOC LAB Follow TCP Stream I.png…]()
