---
Title: SWS Cyber Security
categories: [SWS, networking]
tags: [SWS]
---

### Topic :networking

Networking forms the backbone of modern communication and information exchange systems. It enables computers, devices, and servers to connect and communicate with each other across local and global networks. In this journal entry, we will delve into the fundamentals of networking, focusing on the concepts of ping and IP addresses.

Networking Fundamentals:

At its core, networking involves the interconnection of devices to facilitate data transmission. Networks can be classified based on their geographical scope, such as Local Area Networks (LANs), Wide Area Networks (WANs), and the Internet.

IP Address:

An IP address serves as a unique identifier assigned to each device connected to a network. It enables devices to locate and communicate with each other in a networked environment. IP addresses come in two main versions: IPv4 (32-bit address) and IPv6 (128-bit address). IPv4 addresses are typically represented in decimal format (e.g., 192.168.1.1), while IPv6 addresses are expressed in hexadecimal notation (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).

Ping:

Ping is a networking utility used to test the reachability of a host on an Internet Protocol (IP) network. It also measures the round-trip time (RTT) it takes for data packets to travel from the source device to the destination and back. Ping operates by sending ICMP (Internet Control Message Protocol) echo request packets to the target host and waiting for ICMP echo reply packets in response.

How Ping Works:

Initiation: To initiate a ping command, a user typically opens a command prompt or terminal window and enters the ping command followed by the IP address or hostname of the target device.

Example: ping 192.168.1.1

Packet Transmission: Once the ping command is executed, the sender's device constructs ICMP echo request packets containing a timestamp and sends them to the destination device specified by the IP address.

Packet Reception: Upon receiving the ICMP echo request packets, the destination device processes them and generates ICMP echo reply packets. These reply packets contain the same timestamp as the request packets.

Round-Trip Time Calculation: After receiving the ICMP echo reply packets, the sender's device calculates the round-trip time by subtracting the timestamp in the echo reply packet from the current time.

Display Results: The ping utility displays the results to the user, including the round-trip time, packet loss (if any), and other statistics related to the ping operation.

