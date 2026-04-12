Hands-on-cybersecurity project demonstrating real-time intrusion detection using packet analysis

Network Intrusion Detection using Wireshark

Project Overview
This project demonstrates real-time network traffic analysis and intrusion detection using Wireshark. The objective is to identify suspicious activities such as SYN scan attacks by analyzing packet-level data.

Objectives
- Capture and analyze live network traffic
- Understand TCP/IP protocols and packet structure
- Detect malicious activities like port scanning
- Analyze TCP flags and abnormal behaviors

Tools Used
- Wireshark
- Nmap
- Windows 10

Methodology
1. Packet Capture
Captured live network traffic using Wireshark on Wi-Fi interface.

3. Traffic Analysis
Analyzed protocols such as:
- TCP
- DNS
- TLS/HTTPS

3. Attack Simulation
Used Nmap to perform SYN scan:
nmap -sS 127.0.0.1

4. Intrusion Detection
Applied Wireshark filter:
tcp.flags.syn == 1
Detected multiple SYN packets indicating port scanning.

Key Observations
- High number of SYN packets → Possible scan activity
- TCP Retransmissions → Network instability
- RST packets → Connection termination

Screenshots
Normal Traffic
"Normal Traffic" 
![Normal traffic](Screenshot%20(5).png)

SYN Scan Detection
"SYN Scan" 
![SYN scan](Screenshot%20(2).png)

TCP Analysis
"TCP Analysis" 
![TCP analysis](Screenshot%20(6).png)

Conclusion

This project demonstrates how packet-level analysis can be used to detect suspicious activities in a network. It provides practical exposure to intrusion detection techniques used in real-world cybersecurity environments.

Future Scope
- Implement automated alert system
- Integrate machine learning for anomaly detection
- Expand to real network environments

Author
Mohd Ehsan Muzammil
