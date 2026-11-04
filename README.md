# NETWORKWALKS-DATUS-B084-WK1-PM1-SOC-LAB-WIRESHARK-EXTRA-
<div align="center">
🦈SOC LAB Wireshark (EXTRA)🦈

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

⨳The Lab Network topology was provides as per below diagram of the SOC LAB with Webserver (_IP 192.168.10.20_), SOC Analyst (_IP 192.168.10.10_), **Attacker (_IP Unknown_)**, Network switch  and other host which all are connected to the Switch thru Wired (_Ethernet_)/ Wireless(_Wi-fi_).
<img width="1250" height="676" alt="3 SOC LAB Identify Attacker I" src="https://github.com/user-attachments/assets/388b17ed-1064-45f9-bbb8-f1eb36d16604" />


⨳The Packet analysis was done and the Attacker was identified with Ip **(_192.168.10.66_)** with port **52311** who was try to access service from the server (_192.168.10.20_) through different ports as indicated in packet analysis shown below,
<img width="1366" height="784" alt="3 SOC LAB Identify Attacker II" src="https://github.com/user-attachments/assets/257f0649-79ab-44a4-9405-f827e3a2055d" />





# 👣 Following TCP Stream to Capture and find the  Hidden data
⨳The Lab Network topology was provides as per below diagram of the SOC LAB with Webserver (_IP 192.168.10.20_), SOC Analyst (_IP 192.168.10.10_), **Staff PC (_IP Unknown_)** , Network switch  and other host which all are connected to the Switch thru Wired (_Ethernet_)/ Wireless(_Wi-fi_).
<img width="1251" height="673" alt="4 SOC LAB Follow TCP Stream I" src="https://github.com/user-attachments/assets/aca22eaa-dc17-4e5d-9f63-65aa2dcfcea4" />

⨳By Following The TCP Stream on the Network packets collected using Wireshark the Staff PC's IP **_(192.168.10.45)_** was identified which was communicating thru the Server **(192.168.10.20)** Staff Chat App services TCP port **5000**.

<img width="1360" height="772" alt="4 SOC LAB Follow TCP Stream II" src="https://github.com/user-attachments/assets/e1b9470a-1fb6-426a-b592-8b43f8a2702b" />


⨳After analysis of the network packets collected using Wireshark thru TCP stream (_tcp.stream eq 5_) the hidden data was revealed/discoverd as shown on screenshot below,

<img width="1355" height="779" alt="4 SOC LAB Follwo TCP Stream III" src="https://github.com/user-attachments/assets/1f52a08f-af3e-4d3b-9c94-bf2f9cd1836b" />





# 📸 Capturing (Hidden Data on TCP Stream 
⨳(_Topology Diagram_) 
<img width="1247" height="675" alt="5 SOC LAB Follow TCP Stream 2 I" src="https://github.com/user-attachments/assets/a8722d06-3029-4faf-bc5b-d9c40703f26c" />

⨳ Capturing TCP stream (_tcp.stream eq 7_)
<img width="1358" height="782" alt="5 SOC LAB Follow TCP Stream 2 II" src="https://github.com/user-attachments/assets/ce9416e2-53c3-43a7-b545-6e9eaf76ca5a" />

⨳ Hidden Data
<img width="1357" height="779" alt="5 SOC LAB Follow TCP Stream 2 III" src="https://github.com/user-attachments/assets/1c7c2b09-c171-4157-b9f0-6f4972d7db3f" />





# 🪪To check & identify the unsecure Network protocols (HTTP)🔑
Checking and identifying unsecure Network protocols that show  username and password in clear text (_HTTP_) **port 80** 
which shown during or when a User on **Staff PC(_192.168.10.45_)** is login to the **Portal Server (_192.168.10.20_)**.
<img width="1249" height="681" alt="6 SOC LAB HTTP plain text credentials I" src="https://github.com/user-attachments/assets/16f17ac5-0b94-44e1-b74b-a35d0cd1edff" />

⨳After Analyzing the packets captured from the Wireshark through the HTTP Protocol the User from the **Staff PC(_192.168.10.45_)** credentials was discover to be sent to the **Portal server (_192.168.10.20_)**  through **_port 80_** in cleat text as displayed below,
<img width="1363" height="780" alt="6 SOC LAB HTTP plain text credentials II" src="https://github.com/user-attachments/assets/2356538c-18ec-4e12-bbfa-565c06cc12b0" />





# 🤾‍♂️🪝Catching the Brute Force Attacker
⨳To identifying and catching the **Attacker(_IP Unknown_)** who is try to make a way to the **FTP server (_192.168.10.20_)** **port 21** by try different combination of username and passwords by sending multiple login request trying to access stored resources on the server.
<img width="1248" height="685" alt="7 SOC LAB Catch the Bruteforce Attacker I" src="https://github.com/user-attachments/assets/089b9221-2d26-4435-ada1-74838b82088e" />

⨳ After the analysis of the packet collected by Wireshark The Attacker's IP **(_192.168.10.66_)** was identified  because it was sending too many  FTP login request on within a short period of time on FTP server **(_192.168.10.20_)** thru **_port 21_** try to guess the  username and password  as per below screenshot,
<img width="1361" height="779" alt="7 SOC LAB Catch the Bruteforce Attacker II" src="https://github.com/user-attachments/assets/91f40313-3fc1-4380-94e5-3d8b5b1b8dfb" />

⨳(_tcp.stream eq 6_)
<img width="1364" height="725" alt="7 SOC LAB Catch the Bruteforce Attacker III" src="https://github.com/user-attachments/assets/2431e457-ebc3-4a1f-a106-6c69e85cc27f" />

⨳After many guess or attempt the Attacker was successfully login on the FTP server with the suer name and password shown,
<img width="1366" height="784" alt="7 SOC LAB Catch the Bruteforce Attacker IV" src="https://github.com/user-attachments/assets/6737b7b5-6523-4e17-b4c3-954538627da0" />

⨳(_tcp.stream eq 13_)
<img width="1365" height="781" alt="7 SOC LAB Catch the Bruteforce Attacker V" src="https://github.com/user-attachments/assets/c8cff474-4886-4e7d-8750-a16edc93237d" />





# 📞☎️😥Catching the Call Scammer on VOIP in the Network
To investigate ,capture traffic the call and identifying the scammer who was on the call with user on the network who was using the VoIP (_Voice over IP_) phone **(_192.168.10.45_)** thru the Phone Server **(_192.168.10.20_)**.Also playing it back to hear voice conversation during the call
the below is the topology
<img width="1253" height="676" alt="8 SOC LAB VOIP Call I" src="https://github.com/user-attachments/assets/3aee6697-d259-4c47-a686-b8b144144b2b" />

⨳ After capturing the packets during the analysis **Session initiation Protocol (SIP)** packet was captured and the Scammer **IP (_192.168.10.52_)** was discovered and captured.
<img width="1360" height="781" alt="8 SOC LAB VOIP Call II" src="https://github.com/user-attachments/assets/ea504ede-a247-4aff-a865-c099d63981ff" />

⨳Then the establishment of **Real-time Transport Protocol (RTP)** between user and scammer stream was captured for playback.
<img width="1358" height="774" alt="8 SOC LAB VOIP Call III" src="https://github.com/user-attachments/assets/11cbf9c7-0007-4088-8cef-75e1815ccce0" />

⨳VoIP Call ready for Play Stream,
<img width="1364" height="780" alt="8 SOC LAB VOIP Call IV" src="https://github.com/user-attachments/assets/38c30e8e-64ac-44d7-8b51-5cd7999c9a83" />

⨳The playback stream was Played thru **RTP Player** on Wireshark and audio conversation was heard. as below where scammer IP (_192.168.10.25_) and User IP phone (_192.168.10.45_).
<img width="1359" height="781" alt="8 SOC LAB VOIP Call V" src="https://github.com/user-attachments/assets/150fd883-df28-44b3-9b2a-c6c331d0ebdd" />















 
