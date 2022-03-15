# 1_網路與通訊安全_CISSP.md
```
1. How does TKIP provide more protection for WLAN environments?
A. It uses the AES algorithm.
B. It decreases the IV size and uses the AES algorithm.
C. It adds more keying material.
D. It uses MAC and IP filtering.
```
```
解答: C
臨時金鑰完整性協定（英文：Temporal Key Integrity Protocol，縮寫：TKIP）是一種用於IEEE 802.11無線網路標準中的  替代性安全協定，由電氣電子工程師學會（IEEE）802.11i任務組和Wi-Fi聯盟設計，用以在不需要升級硬體的基礎上替代有線等效加密（WEP）協定。
由於WEP協定的薄弱造成了資料鏈路層安全被完全跳過，且由於已經應用的大量按照WEP要求製造的網路硬體急需更新更可靠的安全協定，
在此背景下臨時金鑰完整性協定應運而生。


需要注意的是，臨時金鑰完整性協定自2012年的802.11標準中，已不再視為安全，且即將廢棄
```

```
2. Which of the following is not a characteristic of the IEEE 802.11a standard?
A. It works in the 5-GHz range.
B. It uses the OFDM spread spectrum technology.
C. It provides 52 Mbps in bandwidth.
D. It covers a smaller distance than 802.11b.
```
```
解答: C
IEEE 802.11
IEEE 802.11a
IEEE 802.11b
IEEE 802.11n

1.工作頻率為5GHz
2.使用52個正交頻分多路復用副載波OFDM spread spectrum technology，
3.最大原始數據傳輸率為54Mb/s，
4.這達到了現實網絡中等吞吐量（20Mb/s）的要求。
5.如果需要的話，數據率可降為48，36，24，18，12，9或者6Mb/s。
6.802.11a擁有12條不相互重疊的頻道，8條用於室內，4條用於點對點傳輸。
7.它不能與IEEE 802.11b進行互操作，除非使用了對兩種標準都採用的設備。
```
```
IEEE 802.11b standard
 
 
```
```
下一代行動網路聯盟（Next Generation Mobile Networks Alliance）定義了5G網路的以下要求：

以10Gbps的資料傳輸速率支援數萬用戶；
以1Gbps的資料傳輸速率同時提供給在同一樓辦公的許多人員；
支援數十萬的並發連接以用於支援大規模傳感器網路的部署；
頻譜效率應當相比4G被顯著增強；
覆蓋率比4G有所提高；
信令效率應得到加強；
延遲應顯著低於LTE。
```

```
3. Why are switched infrastructures safer environments than routed networks?
A. It is more difficult to sniff traffic since the computers have virtual private connections.
B. They are just as unsafe as nonswitched environments.
C. The data link encryption does not permit wiretapping.
D. Switches are more intelligent than bridges and implement security mechanisms.
```
```
解答: A
 switched infrastructures ==> VLAN
  routed networks
```
# 4
```
4. Which of the following protocols is considered connection-oriented?
A. IP
B. ICMP
C. UDP
D. TCP
```
```
解答: D
connection vs connectionless

TCP的五項特性:
連線導向的(Connection Oriented)傳輸協定
同步傳輸(Synchronous Transmission)
可靠的(Reliable)傳輸協定
較無效率的(Inefficient)傳輸協定
流量控制(Flow Control)
```

```
5. Which of the following can take place if an attacker can insert tagging values 
into network- and switch-based protocols with the goal of manipulating traffic 
at the data link layer?
A. Open relay manipulation
B. VLAN hopping attack
C. Hypervisor denial-of-service attack
D. Smurf attack


Virtual LAN (VLAN) Attack 虛擬區域網絡攻擊
https://www.jannet.hk/zh-Hant/post/virtual-lan-vlan-attack/
```

```
6. Which of the following proxies cannot make access decisions based upon protocol commands?
A. Application
B. Packet filtering
C. Circuit
D. Stateful
```

```
7. Which of the following is a bridge-mode technology that can monitor individual traffic links between virtual machines or can be integrated within a hypervisor component?
A. Orthogonal frequency division
B. Unified threat management modem
C. Virtual firewall
D. Internet Security Association and Key Management Protocol
```
# 8
```
8. Which of the following shows the layer sequence as layers 2, 5, 7, 4, and 3?
A. Data link, session, application, transport, and network
B. Data link, transport, application, session, and network
C. Network, session, application, network, and transport
D. Network, transport, application, session, and presentation
```
```
解答:A
```
```
9. Which of the following technologies integrates previously independent security solutions 
with the goal of providing simplicity, centralized control, and streamlined processes?
A. Network convergence
B. Security as a service
C. Unified threat management
D. Integrated convergence management
```

```
10. Metro Ethernet is a MAN protocol that can work in network infrastructures made up of access, aggregation, metro, and core layers. Which of the following best describes these network infrastructure layers?
A. The access layer connects the customer’s equipment to a service provider’s aggregation network. Aggregation occurs on a core network. The metro layer is the metropolitan area network. The core connects different metro networks.
B. The access layer connects the customer’s equipment to a service provider’s core network. Aggregation occurs on a distribution network at the core. The metro layer is the metropolitan area network.
C. The access layer connects the customer’s equipment to a service provider’s aggregation network. Aggregation occurs on a distribution network. The metro layer is the metropolitan area network. The core connects different access layers.
D. The access layer connects the customer’s equipment to a service provider’s aggregation network. Aggregation occurs on a distribution network. The metro layer is the metropolitan area network. The core connects different metro networks.
```

```
11. Which of the following provides an incorrect definition of the specific component or protocol that makes up IPSec?
A. Authentication Header protocol provides data integrity, data origin authentication, and protection from replay attacks.
B. Encapsulating Security Payload protocol provides confidentiality, data origin authentication, and data integrity.
C. Internet Security Association and Key Management Protocol provides a framework for security association creation and key exchange.
D. Internet Key Exchange provides authenticated keying material for use with encryption algorithms.
```

```
12. Systems that are built on the OSI framework are considered open systems. What does this mean?
A. They do not have authentication mechanisms configured by default.
B. They have interoperability issues.
C. They are built with internationally accepted protocols and standards so they can easily communicate with other systems.
D. They are built with international protocols and standards so they can choose what types of systems they will communicate with.
```

```
13. Which of the following protocols work in the following layers: application, data link, network, and transport?
A. FTP, ARP, TCP, and UDP
B. FTP, ICMP, IP, and UDP
C. TFTP, ARP, IP, and UDP
D. TFTP, RARP, IP, and ICMP

```

```

14. What takes place at the data link layer?
A. End-to-end connection
B. Dialog control
C. Framing
D. Data syntax
```

```
15. What takes place at the session layer?
A. Dialog control
B. Routing
C. Packet sequencing
D. Addressing
```

```
16. Which best describes the IP protocol?
A. A connectionless protocol that deals with dialog establishment, maintenance, and destruction
B. A connectionless protocol that deals with the addressing and routing of packets
C. A connection-oriented protocol that deals with the addressing and routing of packets
D. A connection-oriented protocol that deals with sequencing, error detection, and flow control
```

```
17. Which of the following is not a characteristic of the Protected Extensible Authentication Protocol?
A. Authentication protocol used in wireless networks and point-to-point connections
B. Designed to provide authentication for 802.11 WLANs
C. Designed to support 802.1X port access control and Transport Layer Security
D. Designed to support password-protected connections
```

```
18. The ______________ is an IETF-defined signaling protocol, widely used for controlling multimedia communication sessions such as voice and video calls over IP.
A. Session Initiation Protocol
B. Real-time Transport Protocol
C. SS7
D. VoIP
```

```
19. Which of the following is not one of the stages of the DHCP lease process?
i. Discover
ii. Offer
iii. Request
iv. Acknowledgment
A. All of them
B. None of them
C. i, ii
D. ii, iii
```

```
20. An effective method to shield networks from unauthenticated DHCP clients is through the use of _______________ on network switches.
A. DHCP snooping
B. DHCP protection
C. DHCP shielding
D. DHCP caching
```

```
Use the following scenario to answer Questions 21–23. 
Don is a security manager of a large medical institution. 
One of his groups develops proprietary software that provides distributed computing 
through a client/server model. 
He has found out that some of the systems that 
maintain the proprietary software have been experiencing half-open denial-of-service attacks. 
Some of the software is antiquated and still uses basic remote procedure calls, 
which has allowed for masquerading attacks to take place.

21. What type of client ports should Don make sure the institution’s software is using 
when client-to-server communication needs to take place?
A. Well known
B. Registered
C. Dynamic
D. Free

22. Which of the following is a cost-effective countermeasure 
that Don’s team should implement?
A. Stateful firewall
B. Network address translation
C. SYN proxy
D. IPv6

23. What should Don’s team put into place to stop the masquerading attacks 
that have been taking place?
A. Dynamic packet filter firewall
B. ARP spoofing protection
C. Disable unnecessary ICMP traffic at edge routers
D. SRPC

```

```
Use the following scenario to answer Questions 24–26. 
Grace is a security administrator for a medical institution 
and is responsible for many different teams. 
One team has reported that when their main FDDI connection failed, 
three critical systems went offline even though the connection was supposed 
to provide redundancy. 
Grace has to also advise her team on the type of fiber 
that should be implemented for campus building-to-building connectivity. 

Since this is a training medical facility, 
many surgeries are video recorded and that data must continuously travel 
from one building to the next. 
One other thing that has been reported to Grace is that 
periodic DoS attacks take place against specific servers within the internal network. 
The attacker sends excessive ICMP Echo Request packets to all the hosts on a specific subnet, 
which is aimed at one specific server.

24. Which of the following is most likely the issue that Grace’s team experienced 
when their systems went offline?
A. Three critical systems were connected to a dual-attached station.
B. Three critical systems were connected to a single-attached station.
C. The secondary FDDI ring was overwhelmed with traffic and dropped the three critical systems.
D. The FDDI ring is shared in a metropolitan environment and 
only allows each company to have a certain number of systems connected to both rings.

25. Which of the following is the best type of fiber that should be implemented in this scenario?
A. Single mode
B. Multimode
C. Optical carrier
D. SONET

26. Which of the following is the best and most cost-effective countermeasure 
for Grace’s team to put into place?
A. Network address translation
B. Disallowing unnecessary ICMP traffic coming from untrusted networks
C. Application-based proxy firewall
D. Screened subnet using two firewalls from two different vendors
```

```
Use the following scenario to answer Questions 27–29. 
John is the manager of the security team within his company. 
He has learned that attackers have installed sniffers throughout the network 
without the company’s knowledge. 
Along with this issue his team has also found out that 
two DNS servers had no record replication restrictions put into place 
and the servers have been caching suspicious name resolution data.

27. Which of the following is the best countermeasure to put into 
place to help reduce the threat of network 
sniffers viewing network management traffic?
A. SNMP v3
B. L2TP
C. CHAP
D. Dynamic packet filtering firewall

28. Which of the following unauthorized activities have most likely 
been taking place in this situation?
A. DNS querying
B. Phishing
C. Forwarding
D. Zone transfer

29. Which of the following is the best countermeasure that John’s team should implement 
to protect from improper caching issues?
A. PKI
B. DHCP snooping
C. ARP protection
D. DNSSEC

```

```
Use the following scenario to answer Questions 30–32. Sean is the new 
security administrator for a large financial institution. 
There are several issues that Sean is made aware of the first week he is in his new position. 
First, spurious packets seem to arrive at critical servers 
even though each network has tightly configured firewalls at each gateway position 
to control traffic to and from these servers. 
One of Sean’s team members complains that the current firewall logs 
are excessively large with useless data. 
He also tells Sean that the team needs to be 
using less permissive rules instead of the current “any-any” rule type in place. 
Sean has also found out that some team members want to 
implement tarpits on some of the most commonly attacked systems.

30. Which of the following is most likely taking place to allow spurious packets 
to gain unauthorized access to critical servers?
A. TCP sequence hijacking is taking place.
B. Source routing is not restricted.
C. Fragment attacks are underway.
D. Attacker is tunneling communication through PPP.

31. Which of the following best describes the firewall configuration issues 
Sean’s team member is describing?
A. Clean-up rule, stealth rule
B. Stealth rule, silent rule
C. Silent rule, negate rule
D. Stealth rule, silent rule

32. Which of the following best describes why Sean’s team wants to 
put in the mentioned countermeasure for the most commonly attacked systems?
A. Prevent production system hijacking
B. Reduce DoS attack effects
C. Gather statistics during the process of an attack
D. Increase forensic capabilities
```

```
Use the following scenario to answer Questions 33–35. 
Tom’s company has been experiencing many issues with unauthorized sniffers being installed on the network. One reason is because employees can plug their laptops, smartphones, and other mobile devices into the network, any of which may be infected and have a running sniffer that the owner is not aware of. Implementing VPNs will not work because all of the network devices would need to be configured for specific VPNs, and some devices, as in their switches, do not have this type of functionality available. Another issue Tom’s team is dealing with is how to secure internal wireless traffic. While the wireless access points can be configured with digital certificates for authentication, pushing out and maintaining certificates on each wireless user device is cost prohibitive and will cause too much of a burden on the network team. 
Tom’s boss has also told him that the company needs to move from a landline metropolitan 
area network solution to a wireless solution.

33. What should Tom’s team implement to provide source authentication and data encryption at the data link level?
A. IEEE 802.1AR
B. IEEE 802.1AE
C. IEEE 802.1AF
D. IEEE 802.1X

34. Which of the following solutions is best to meet the company’s need to protect wireless traffic?
A. EAP-TLS
B. EAP-PEAP
C. LEAP
D. EAP-TTLS

35. Which of the following is the best solution to meet the company’s need for broadband wireless connectivity?
A. WiMAX
B. IEEE 802.12
C. WPA2
D. IEEE 802.15
```

```
Use the following scenario to answer Questions 36–38. 
Lance has been brought in as a new security officer for a large medical equipment company. 
He has been told that many of the firewalls and IDS products have not been configured 
to filter IPv6 traffic; thus, many attacks have been taking place 
without the knowledge of the security team. 
While the network team has attempted to implement an automated tunneling feature to take care of this issue, they have continually run into problems with the network’s NAT device. Lance has also found out that caching attacks have been successful against the company’s public-facing DNS server. He has also identified that extra authentication is necessary for current LDAP requests, but the current technology only provides password-based authentication options.

36. Based upon the information in the scenario, what should the network team implement as it pertains to IPv6 tunneling?
A. Teredo should be configured on IPv6-aware hosts that reside behind the NAT device.
B. 6to4 should be configured on IPv6-aware hosts that reside behind the NAT device.
C. Intra-Site Automatic Tunnel Addressing Protocol should be configured on 
IPv6-aware hosts that reside behind the NAT device.
D. IPv6 should be disabled on all systems.

37. Which of the following is the best countermeasure for the attack type addressed in the scenario?
A. DNSSEC
B. IPSec
C. Split server configurations
D. Disabling zone transfers

38. Which of the following technologies should Lance’s team investigate for increased authentication efforts?
A. Challenge Handshake Authentication Protocol
B. Simple Authentication and Security Layer
C. IEEE 802.2AB
D. EAP-SSL
```

```
39. Wireless LAN technologies have gone through different versions over the years to address some of the inherent security issues within the original IEEE 802.11 standard. Which of the following provides the correct characteristics of Wi-Fi Protected Access 2 (WPA2)?
A. IEEE 802.1X, WEP, MAC
B. IEEE 802.1X, EAP, TKIP
C. IEEE 802.1X, EAP, WEP
D. IEEE 802.1X, EAP, CCMP
```

```
40. Alice wants to send a message to Bob, who is several network hops away from her. What is the best approach to protecting the confidentiality of the message?
A. PPTP
B. S/MIME
C. Link encryption
D. SSH
```

```
41. Charlie uses PGP on his Linux-based email client. His friend Dave uses S/MIME on his Windows-based email. Charlie is unable to send an encrypted email to Dave. What is the likely reason?
A. PGP and S/MIME are incompatible
B. Each has a different secret key
C. Each is using a different CA
D. There is not enough information to determine the likely reason
```
