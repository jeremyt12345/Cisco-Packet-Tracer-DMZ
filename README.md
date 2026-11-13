# Cisco-Packet-Tracer-DMZ
Configuring a DMZ lab to better learn


The topology layout consists of three major zones:

Internal
DMZ
External

"Think of Internal and DMZ together as being our private network. This design strategy is a perfect example of significantly increasing security through network segmentation."


I will be following this guide here and referring to this.

"https://cybr.com/network-security-archives/project-dmz-and-network-hardening-tutorial-with-packet-tracer/"

<img width="826" height="519" alt="image" src="https://github.com/user-attachments/assets/8395bddf-fced-4b76-b6ce-fff5a60ff7aa" />



Step 1: Assign security level to each ASA interface



<img width="826" height="519" alt="image" src="https://github.com/user-attachments/assets/3e85b8b8-600f-400d-87ac-83b9849dc2c0" />


Set each interface and set for a different network

"description to WAN" a label for humans only with no effect to traffic

"nameif outside" gives the interface a logcial name and every NAT rule and ACL refers to interfaces by that name. 

security-level 0 / 100 / 50 / 20: how much the ASA trusts each zone. This sets the default traffic behavior before you write any rules:

Step 2: Configure ASA as an Internet gateway, enable Internet access

<img width="621" height="188" alt="image" src="https://github.com/user-attachments/assets/a3322495-c322-4c02-84cf-3f6b04c53ffc" />


