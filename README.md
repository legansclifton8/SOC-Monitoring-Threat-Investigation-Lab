<h1>SOC Monitoring & Threat Investigation Lab</h1>

<h2>Description</h2>
This project focused on building a controlled cybersecurity lab environment using Kali Linux, Windows 10, VirtualBox, Nmap, Wireshark, and Windows Event Viewer to simulate real-world reconnaissance, network traffic monitoring, remote connection attempts, and Windows security log investigation techniques commonly performed by SOC analysts.

The lab environment was configured using isolated VirtualBox internal networking and static IP addressing to safely simulate attacker activity, monitor exposed services, analyze packet captures, and investigate Windows authentication events within a contained environment.
<br />

<h2>Languages and Utilities Used</h2>

- <b>Kali Linux</b>
- <b>Windows 10</b>
- <b>VirtualBox</b>
- <b>Nmap</b>
- <b>Wireshark</b>
- <b>Windows Event Viewer</b>
- <b>RDP (Remote Desktop Protocol)</b>
- <b>ICMP</b>

<h2>Environments Used</h2>

- <b>Kali Linux Virtual Machine</b>
- <b>Windows 10 Virtual Machine</b>
- <b>VirtualBox Internal Network</b>

<h2>Project Walk-through:</h2>

<p align="center">

Configured a static IP address on the Kali Linux virtual machine to establish reliable communication within the isolated internal network: <br/>
<img src="https://i.imgur.com/HOezLkp.png"/>
<br />
<br />

Configured a static IP address on the Windows virtual machine to maintain stable internal network communication between systems: <br/>
<img src="https://i.imgur.com/XHKALaR.png"/>
<br />
<br />

Modified Windows Firewall inbound rules to allow ICMP traffic and internal network communication between the Kali Linux and Windows virtual machines: <br/>
<img src="https://i.imgur.com/bGADJNx.png"/>
<br />
<br />

Verified successful network connectivity between Kali Linux and the Windows virtual machine using ICMP ping requests across the VirtualBox internal network: <br/>
<img src="https://i.imgur.com/b6pfUqh.png"/>
<br />
<br />

Performed reconnaissance and service enumeration using Nmap to identify exposed services and open ports running on the Windows virtual machine: <br/>
<img src="https://i.imgur.com/BBD0BNQ.png"/>
<br />
<br />

Executed an aggressive Nmap scan using service detection and OS fingerprinting to gather additional information about the target Windows system and generate network activity for monitoring purposes: <br/>
<img src="https://i.imgur.com/DiO59rK.png"/>
<br />
<br />

Simulated a real-world remote desktop connection attempt from the Kali Linux machine to the Windows virtual machine using RDP in order to generate authentication and remote access events for analysis: <br/>
<img src="https://i.imgur.com/YoqUYlA.png"/>
<br />
<br />

Filtered Windows Security Event logs using Event ID 4625 to identify failed authentication attempts generated during the simulated remote connection activity: <br/>
<img src="https://i.imgur.com/sV02Nc7.png"/>
<br />
<br />

Captured live network traffic using Wireshark to monitor ICMP communication and packet flow between the Kali Linux and Windows virtual machines: <br/>
<img src="https://i.imgur.com/YM3zUFx.png"/>
<br />
<br />

Started a live Wireshark packet capture session to analyze reconnaissance traffic and monitor network communication occurring within the isolated cybersecurity lab environment: <br/>
<img src="https://i.imgur.com/pOMru4h.png"/>
<br />
<br />

Analyzed TCP SYN packets and network handshakes generated during reconnaissance activity to observe low-level communication between systems during the Nmap scanning process: <br/>
<img src="https://i.imgur.com/V2djdCn.png"/>
<br />
<br />

Filtered Wireshark traffic using IP-based display filters to isolate communication between the Kali Linux and Windows virtual machines during reconnaissance and network monitoring activity: <br/>
<img src="https://i.imgur.com/OTfoHvb.png"/>
<h2>Conclusion</h2>

This lab provided hands-on experience with network reconnaissance, traffic analysis, Windows event monitoring, and simulated threat investigation techniques commonly used within Security Operations Center (SOC) environments. The project strengthened practical understanding of network communication, service exposure, authentication monitoring, and packet-level traffic analysis within an isolated virtualized lab environment.
