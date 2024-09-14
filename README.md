# SAMPLE TEST

## CAB222 Networks

### Example of Assessment: Laboratory/Practical – Part 1

**Addressing and Routing**

This is an individual assessment.

**Assessment Duration**: 50 minutes

The sample specifications are designed to assist you in preparation for the actual Practical Assessment 1.

**Instructions**:
- You have 50 minutes to complete the actual assessment. This exam is an open-book, individual exam.
- You may use Cisco Packet Tracer to validate your answers as well as to exercise your problem-solving skills. However, Packet Tracer files will not be marked and should not be uploaded.
- In the actual test, there are three (3) sections including addressing, routing and troubleshooting. In this sample test, there are only two (2) sections including addressing and routing.
- You can use this sample test to test yourself with the time limits challenge.

### Scenario

You have been given a block of IPv4 addresses 193.168.0.0/24 to create 8 subnets. Based on the addressing instructions and routing specifications, you are required to assign designated IP addresses for the hosts and router interfaces.

#### Section A - Addressing

This scenario involves with three generic routers (Router-PT). The routers are connected through a point-to-point serial link as shown in Figure 1:
- R1 – R2 and R1 – R3 are connected through serial links. R3 is the ISP’s router.
- R1’s Serial2/0 interface connects to R2’s Serial2/0 interface.
- R1’s Serial3/1 interface connects to R3’s Serial2/0 interface.
- R1 connects to Subnets 1, 2 and 3.
- R2 connects Subnets 1, 5, 6, 7 and 8.
- The addresses of Subnet 1 are reserved for the link between R1 and R2.
- Each FastEthernet interface of the router is connected to a generic switch. Add one server to each subnet (except Subnet 1) via a switch.

**Figure 1: Topology Diagram.**

Use Table 1 to list the subnetting details of the 8 subnets.

**Table 1: Subnetting Table**
| Subnet | Network Subnet Address | Subnet Mask | First Usable IP Address | Last Usable IP Address | Broadcast Address |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] |
| 2 | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] |
| 3 | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] |
| 4 | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] |
| 5 | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] |
| 6 | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] |
| 7 | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] |
| 8 | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] | [To be calculated] |

**(1) IP Addressing Instructions**
- 2 usable addresses 100.0.0.0/24 are used for the link between routers R1 and R3:
    - Assign the first usable IP address of 100.0.0.0/30 on the interface Se3/0 of R1.
    - Assign the second usable IP address of 100.0.0.0/30 on the interface Se2/0 of R3.
- Two addresses of Subnet 1 are used for the link between routers R1 and R2:
    - Assign the first usable IP address of Subnet 1 on the interface Se2/0 of R1.
    - Assign the second usable IP address of Subnet 1 on the interface Se2/0 of R2.
- Subnet 2 connects to router R1:
    - Assign the first usable IP address of Subnet 2 on the interface Fa0/0 of R1.
    - Assign the last usable IP address of Subnet 2 on SERVER2.
- Subnet 3 connects to router R1:
    - Assign the first usable IP address of Subnet 3 on the interface Fa1/0 of R1.
    - Assign the last usable IP address of Subnet 3 on SERVER3.
- Subnet 4 is reserved for future use.
- Subnet 5 connects to router R2:
    - Assign the first usable IP address of Subnet 5 on the interface Fa0/0 of R2.
    - Assign the last usable IP address of Subnet 5 on SERVER5.
- Subnet 6 connects to router R2:
    - Assign the first usable IP address of Subnet 6 on the interface Fa1/0 of R2.
    - Assign the last usable IP address of Subnet 6 on SERVER6.
- Subnet 7 connects to router R2:
    - Assign the first usable IP address of Subnet 7 on the interface Fa4/0 of R2.
    - Assign the last usable IP address of Subnet 7 on SERVER7.
- Subnet 8 connects to router R2:
    - Assign the first usable IP address of Subnet 8 on the interface Fa5/0 of R2.
    - Assign the last usable IP address of Subnet 8 on SERVER8.

Complete the addressing table (Table 2) based on the above addressing specifications.

**Table 2: Addressing Table**
| Device | Interface | IP Address | Subnet Mask |
| ---- | ---- | ---- | ---- |
| R1 | Se2/0 | [To be calculated] | [To be calculated] |
| R1 | Se3/0 | [To be calculated] | [To be calculated] |
| R1 | Fa0/0 | [To be calculated] | [To be calculated] |
| R1 | Fa1/0 | [To be calculated] | [To be calculated] |
| R2 | Se2/0 | [To be calculated] | [To be calculated] |
| R2 | Fa0/0 | [To be calculated] | [To be calculated] |
| R2 | Fa1/0 | [To be calculated] | [To be calculated] |
| R2 | Fa4/0 | [To be calculated] | [To be calculated] |
| R2 | Fa5/0 | [To be calculated] | [To be calculated] |
| R3 (ISP) | Se2/0 | [To be calculated] | [To be calculated] |
| Device | IP Address | Subnet Mask | Default Gateway |
| SERVER2 | [To be calculated] | [To be calculated] | [To be calculated] |
| SERVER3 | [To be calculated] | [To be calculated] | [To be calculated] |
| SERVER5 | [To be calculated] | [To be calculated] | [To be calculated] |
| SERVER6 | [To be calculated] | [To be calculated] | [To be calculated] |
| SERVER7 | [To be calculated] | [To be calculated] | [To be calculated] |
| SERVER8 | [To be calculated] | [To be calculated] | [To be calculated] |

#### Section B - Routing

This section provides the routing specifications. Your routing must follow these specifications accordingly.
- From R1, configure one default route pointing to R3.
- From R1, configure one static route to reach the subnets 5-8 that are attached to R2.
- From R2, configure one default route pointing to R1.
- From R3, configure one static route to reach all other subnets that are attached to R1 and R2.

**Routing recording**: Use the following tables to record static routes for R1, R2, and R3.

**Table 3: R1’s Routing Table**
| Router 1 | Network Address | Subnet Mask | Next Hop |
| ---- | ---- | ---- | ---- |
| Internal network facing route | [To be calculated] | [To be calculated] | [To be calculated] |
| External network facing route | [To be calculated] | [To be calculated] | [To be calculated] |

**Table 4: R2’s Routing Table**
| Router | Network Address | Subnet Mask | Next Hop |
| ---- | ---- | ---- | ---- |
| R2 | [To be calculated] | [To be calculated] | [To be calculated] |

**Table 5: R3’s Routing Table**
| Router | Network Address | Subnet Mask | Next Hop |
| ---- | ---- | ---- | ---- |
| R3 (ISP) | [To be calculated] | [To be calculated] | [To be calculated] |

### Network Topology and Configuration Tasks

**I. Network Topology**
Task 1: Build a Network Topology
You may use Cisco Packet Tracer to build a network topology and label the routers and workstations accordingly as shown in Figure 1.

**II. IP Addressing Configuration**
Task 2: Subnet the Address Space
Use Table 1 to record the subnet information.

Task 3: Configure IP Addressing
Use Table 2 Addressing Table to assign the specified IP addresses to workstations and router interfaces, according to the IP addressing specifications.

Task 4: Test and Troubleshoot
You may use Cisco Packet Tracer to validate your answers as well as to exercise your problem-solving skills. After configuring your addressing assignment with Packet Tracer, you can Ping utility to verify your answer and exercise your troubleshooting skills.

**III. Routing Configuration**
Task 5: Record Static Routing Tables
Use Tables 3-5 to record static routing information for R1, R2 and R3.

Task 6: Configure Static Routing
Implement static routing for each router.

Task 7: Test and Troubleshoot
Once again, after you have configured static routing with Packet Tracer, you can use Ping utility to verify your routing configuration and exercise your troubleshooting skills.


# SAMPLE TEST SOLUTIONS

## CAB222 Networks

### Example of Assessment: Laboratory/Practical – Part 1

**Addressing and Routing**

This is an individual assessment.

**Assessment Duration**: 50 minutes

The sample test solutions are designed to assist you in preparation for the actual Practical Assessment 1.

**Instructions**:
- You have 50 minutes to complete the actual assessment. This exam is an open-book, individual exam.
- You may use Cisco Packet Tracer to validate your answers as well as to exercise your problem-solving skills. However, Packet Tracer files will not be marked and should not be uploaded.
- In the actual test, there are three (3) sections including addressing, routing and troubleshooting. In this sample test, there are only two (2) sections including addressing and routing.
- You can use this sample test to test yourself with the time limits challenge.

### Scenario

You have been given a block of IPv4 addresses 193.168.0.0/24 to create 8 subnets. Based on the addressing instructions and routing specifications, the designated IP addresses for the hosts and router interfaces have been assigned.

#### Section A - Addressing

This scenario involves three generic routers (Router-PT). The routers are connected through a point-to-point serial link as shown in Figure 1:
- R1 – R2 and R1 – R3 are connected through serial links. R3 is the ISP’s router.
- R1’s Serial2/0 interface connects to R2’s Serial2/0 interface.
- R1’s Serial3/1 interface connects to R3’s Serial2/0 interface.
- R1 connects to Subnets 1, 2 and 3.
- R2 connects Subnets 1, 5, 6, 7 and 8.
- The addresses of Subnet 1 are reserved for the link between R1 and R2.
- Each FastEthernet interface of the router is connected to a generic switch. Add one server to each subnet (except Subnet 1) via a switch.

**Table 1: Subnetting Table**
| Subnet | Network Subnet Address | Subnet Mask | First Usable IP Address | Last Usable IP Address | Broadcast Address |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | 193.168.0.0 | 255.255.255.224 | 193.168.0.1 | 193.168.0.30 | 193.168.0.31 |
| 2 | 193.168.0.32 | 255.255.255.224 | 193.168.0.33 | 193.168.0.62 | 193.168.0.63 |
| 3 | 193.168.0.64 | 255.255.255.224 | 193.168.0.65 | 193.168.0.94 | 193.168.0.95 |
| 4 | 193.168.0.96 | 255.255.255.224 | 193.168.0.97 | 193.168.0.126 | 193.168.0.127 |
| 5 | 193.168.0.128 | 255.255.255.224 | 193.168.0.129 | 193.168.0.158 | 193.168.0.159 |
| 6 | 193.168.0.160 | 255.255.255.224 | 193.168.0.161 | 193.168.0.190 | 193.168.0.191 |
| 7 | 193.168.0.192 | 255.255.255.224 | 193.168.0.193 | 193.168.0.222 | 193.168.0.223 |
| 8 | 193.168.0.224 | 255.255.255.224 | 193.168.0.225 | 193.168.0.254 | 193.168.0.255 |

**Table 2: Addressing Table**
| Device | Interface | IP Address | Subnet Mask |
| ---- | ---- | ---- | ---- |
| R1 | Se2/0 | 193.168.0.1 | 255.255.255.224 |
| R1 | Se3/0 | 100.0.0.1 | 255.255.255.252 |
| R1 | Fa0/0 | 193.168.0.33 | 255.255.255.224 |
| R1 | Fa1/0 | 193.168.0.65 | 255.255.255.224 |
| R2 | Se2/0 | 193.168.0.2 | 255.255.255.224 |
| R2 | Fa0/0 | 193.168.0.129 | 255.255.255.224 |
| R2 | Fa1/0 | 193.168.0.161 | 255.255.255.224 |
| R2 | Fa4/0 | 193.168.0.193 | 255.255.255.224 |
| R2 | Fa5/0 | 193.168.0.225 | 255.255.255.224 |
| R3 (ISP) | Se2/0 | 100.0.0.2 | 255.255.255.252 |
| Device | IP Address | Subnet Mask | Default Gateway |
| SERVER2 | 193.168.0.62 | 255.255.255.224 | 193.168.0.33 |
| SERVER3 | 193.168.0.94 | 255.255.255.224 | 193.168.0.65 |
| SERVER5 | 193.168.0.158 | 255.255.255.224 | 193.168.0.129 |
| SERVER6 | 193.168.0.190 | 255.255.255.224 | 193.168.0.161 |
| SERVER7 | 193.168.0.222 | 255.255.255.224 | 193.168.0.193 |
| SERVER8 | 193.168.0.254 | 255.255.255.224 | 193.168.0.225 |

#### Section B - Routing

The routing specifications have been followed as follows:

**Table 3: R1’s Routing Table**
| Router 1 | Network Address | Subnet Mask | Next Hop |
| ---- | ---- | ---- | ---- |
| Internal network facing route | 193.168.0.128 | 255.255.255.128 | 193.168.0.2 |
| External network facing route | 0.0.0.0 | 0.0.0.0 | 100.0.0.2 |

**Table 4: R2’s Routing Table**
| Router | Network Address | Subnet Mask | Next Hop |
| ---- | ---- | ---- | ---- |
| R2 | 0.0.0.0 | 0.0.0.0 | 193.168.0.1 |

**Table 5: R3’s Routing Table**
| Router | Network Address | Subnet Mask | Next Hop |
| ---- | ---- | ---- | ---- |
| R3 (ISP) | 193.168.0.0 | 255.255.255.0 | 100.0.0.1 |

### Network Topology and Configuration Tasks

**I. Network Topology**
Task 1: Build a Network Topology
You may use Cisco Packet Tracer to build a network topology and label the routers and workstations accordingly as shown in Figure 1.

**II. IP Addressing Configuration**
Task 2: Subnet the Address Space
Use Table 1 to record the subnet information.

Task 3: Configure IP Addressing
Use Table 2 Addressing Table to assign the specified IP addresses to workstations and router interfaces, according to the IP addressing specifications.

Task 4: Test and Troubleshoot
You may use Cisco Packet Tracer to validate your answers as well as to exercise your problem-solving skills. After configuring your addressing assignment with Packet Tracer, you can Ping utility to verify your answer and exercise your troubleshooting skills.

**III. Routing Configuration**
Task 5: Record Static Routing Tables
Use Tables 3-5 to record static routing information for R1, R2 and R3.

Task 6: Configure Static Routing
Implement static routing for each router.

Task 7: Test and Troubleshoot
Once again, after you have configured static routing with Packet Tracer, you can use Ping utility to verify your routing configuration and exercise your troubleshooting skills.
# CAB222 Networks Exam Test

# CS Tutor | 计算机编程辅导 | Code Help | Programming Help

# WeChat: cstutorcs

# Email: tutorcs@163.com

# QQ: 749389476

# 非中介, 直接联系程序员本人
