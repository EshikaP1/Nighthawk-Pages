---
toc: true
comments: true
layout: post
title: 4.1 - The Internet Homework
description: Internet and basic protocols
type: ccc
courses: { csp: {week: 14} }
---

## 4.1 The Internet


# Homework Questions
Please answer all of these questions on your personal blog and **explain**. Don't just give an answer. Homework is due Sunday night at 6 pm

#### IP Addresses
1. Which of the following IP Addresses are possible? Explain (yes/no) for each answer choice.
<br>
 - 1.1.1.1.1 - No, because an IP address is usually composed of four sets of 8-bit numbers (0-255), and this has an extra set.

 - 23.23.23.23 - Yes, because it follows the correct format of four sets of 8-bit numbers.

 - 134.492.100.0 - No, because the second set has a number outside the valid range (0-255).

 - 255.256.55.255 - No, because the third set has a number outside the valid range (0-255).

 - 2.93.255.19 - Yes, because it follows the correct format of four sets of 8-bit numbers.

2. If Dian Du is at home on his home network and sends a message to every computer on the network, what is this an example of? Explain.
<br>
- Multicast
- Unicast
- Broadcast

This is an example of broadcast because broadcast is used for communication within a Local Area Network (LAN), and the data stops at the router.

#### Models
1. Three of the four following protocols are on the same layer. Identify which ones and what layer they are on, and why they are on each layer:
    - ASCII (see above for information)
    - FTP (facilitates transfer of files over the internet)
    - TLS (see HTTPS section)
    - USB (permits data exchange between electronics)

ASCII - Presentation Layer (Layer 6): It translates data between the application layer and the lower layers.
FTP - Application Layer (Layer 7): Facilitates file transfer between systems.
TLS - Presentation Layer (Layer 6): It ensures that the data is presented in a readable format.
USB is not a protocol but rather a physical interface standard. It is not part of the OSI model.


2. Telnet is a internet protocol which allows remote access to other computers over a local network or the internet. What layer of the OSI model would this protocol be located on? What is the function of this layer?

Telnet would be located at the Application Layer (Layer 7) of the OSI model. This layer is responsible for providing network services directly to end-users or applications.

#### DNS

1. Bob wants to use the domain bob.is.the.best.com. What domain should he buy from a DNS provider (assume it is available)? What would be the subdomains?

Bob should buy the domain best.com from a DNS provider, and the subdomains could be:
bob.is.the (subdomain).best.com

#### HTTP and HTTPS
1. What is a difference between HTTP and HTTPS? 
<br>
 - What protocol does HTTPS use that HTTP doesn't?

HTTP transmits data in plain text, while HTTPS encrypts the data using SSL/TLS protocols.
Protocol used by HTTPS that HTTP doesn't use: SSL/TLS (Secure Sockets Layer/Transport Layer Security).
HTTP or HTTPS for Last Trimester Passion Projects:

2. Last trimester we sent HTTP requests for our passion projects
<br>
 - Did we use HTTP or HTTPS?
 - What are the benefits and disadvantages of this?

Last trimester we used HTTP.
Benefits: Simplicity, less resource-intensive.
Disadvantages: Lack of security, vulnerability to eavesdropping.

#### TCP and UDP

1. Bob is setting up a video streaming service, and he needs the stream to be real time. 
<br>
 - What protocol should he use, TCP or UDP? Why?
 - What are some cons of this protocol? Give an example of a potential issue.

For a real-time video streaming service, Bob should use UDP.
Reason: UDP is faster and more suitable for real-time applications.
Cons: Little data checking, generally unreliable.

2. TCP has error checking, which ensures that all packets arrive properly. Why is this important?
<br>
 - Give an example of how TCP ensures that there are no errors.

Importance of TCP Error Checking:
Why: TCP ensures reliable and error-free communication by checking if all packets are received properly.
Example: If a packet is not acknowledged (ACK) by the receiver, TCP will retransmit it.

3. Server A computer is communicating with Server B. They have already initiated communication and Server A is now attempting to send data to Server B.
<br>
 - How does Server B ensure that they have received any sent packets before Server A continues sending packets in TCP? In UDP?
 - What is another use of this?

TCP: Server B sends an ACK (Acknowledgment) back to confirm the received packets before Server A continues sending more packets.
UDP: UDP does not have such a mechanism; packets are sent without acknowledgment.
Another use: Ensures data integrity and reliability in TCP, while UDP might be used when real-time communication is more critical than data accuracy.
