# Analyzing-Packets-with-Wireshark

## Scenario
In this scenario, you’re a security analyst investigating traffic to a website.

You’ll analyze a network packet capture file that contains traffic data related to a user connecting to an internet site. The ability to filter network traffic using packet sniffers to gather relevant information is an essential skill as a security analyst.

You must filter the data in order to:
- Identify the source and destination IP addresses involved in this web browsing session.
- Examine the protocols used when the user makes the connection to the website.
- Analyze data packets to identify the type of information sent and received by the systems.

Here’s how you’ll do this: Open the packet capture file and explore the Wireshark interface, open a detailed view of a single packet and analyze the protocol and data layers, apply filters to inspect specific packets based on criteria, filter and inspect UDP DNS traffic for protocol data, and apply filters to TCP packet data to search for specific payload text.

![Echo Request Packet](https://github.com/user-attachments/assets/4aae2469-6573-4e3c-8cb1-bd72e1529e7a)  
**Description:** This screenshot displays an example of a packet in Wireshark where the `Info` column begins with "Echo (ping) request." It highlights the packet properties such as source IP, destination IP, protocol, and other key metadata, including the timestamp and length of the packet.

![Filtered TCP Packet Details](https://github.com/user-attachments/assets/f4a8e042-8178-4125-925e-2da468f88a52)  
**Description:** This screenshot shows the detailed analysis of a TCP packet filtered by the IP address `142.250.1.139`. It expands the `Frame`, `Ethernet II`, `IPv4`, and `TCP` subtrees to display details such as source and destination ports, sequence numbers, and MAC addresses.

![Filtered Source IP Packet](https://github.com/user-attachments/assets/e6ae0313-064b-40b8-ad6b-5ac3186a7aba)  
**Description:** This screenshot highlights a filtered list of packets where the source IP address matches `142.250.1.139`. It displays the packet summary, including protocol type, source, and destination information.

![DNS Query](https://github.com/user-attachments/assets/7b0663ee-a05a-4080-89c7-c57b63a6fbbd)  
**Description:** This screenshot displays a DNS query packet captured in Wireshark. The `Domain Name System (query)` subtree is expanded to reveal the queried domain, which is `opensource.google.com`.

![DNS Answer](https://github.com/user-attachments/assets/1786413b-561f-4463-8533-3099c2d465cb)  
**Description:** This screenshot shows a DNS answer packet. The `Domain Name System (query)` subtree is expanded to reveal the resolved IP address for the queried domain `opensource.google.com`.

![TCP Packet Analysis](https://github.com/user-attachments/assets/fe13ec10-73b4-4aea-a1c5-681905cb84f8)  
**Description:** This screenshot focuses on a TCP packet filtered by port `80`. Key details such as the `Time to Live` value (64), `Frame Length` (54 bytes), `Header Length` (20 bytes), and the destination address `169.254.169.254` are analyzed in this packet.
