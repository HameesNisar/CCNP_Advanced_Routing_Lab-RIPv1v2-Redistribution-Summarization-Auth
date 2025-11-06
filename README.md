# 🛰️ CCNP Advanced Routing Lab — RIP v1 & v2 Redistribution, Route Summarization, and Authentication

## 📘 Overview
This lab demonstrates advanced dynamic routing concepts using **RIP version 1 and RIP version 2**, focusing on interoperability, route summarization, authentication, and route injection.  
The network was built and tested using **GNS3**, simulating a multi-router enterprise topology connected to an ISP for external reachability.

---

## 🎯 Objectives
The main objectives of this lab were to:

- Implement **RIP version 1 and RIP version 2** across multiple routers.  
- Configure **route redistribution** between RIP v1 and RIP v2 domains to ensure interoperability.  
- Apply **route summarization** on loopback interfaces to minimize routing table entries and improve efficiency.  
- Use **authentication (MD5)** between RIP neighbors to enhance routing security.  
- Utilize **passive interfaces** to restrict routing updates from non-routing interfaces while maintaining reachability.  
- Perform **route injection** (default route advertisement) from the **Edge Router** towards the internal network.  
- Ensure that **only the Admin routers (R22 and R24)** receive all route updates.  
- Implement **unicast updates** to limit routing update broadcasts.  

---

## 🧩 Network Topology

The topology consists of:

- **ISP Router** connected to the **Edge Router** for internet simulation.  
- Multiple routers (**R1–R30**) divided into several RIP domains.  
- **Admin Routers:** R22 and R24 – configured to receive full routing information.  
- **Switches** interconnecting the routers to simulate LAN segments.  

📷 **Topology Design:**  
<img width="1861" height="895" alt="topology" src="https://github.com/user-attachments/assets/2b0f0c52-7293-487e-b8b6-25daada744b6" />

---

## 🧠 Key Concepts Demonstrated

- **RIP v1 and RIP v2 interoperability and redistribution**  
- **Route summarization** on loopback interfaces  
- **Routing authentication (MD5)** between neighbors  
- **Passive interface default** and selective activation  
- **Default route injection** using `default-information originate`  
- **Unicast routing updates**  
- **Hierarchical route propagation control**  

---

## ⚙️ Tools & Environment

- **GNS3 v2.2.54**  
- **Cisco IOSv Routers**  
- **VPCS** for host simulation  
- **Switches** for LAN interconnectivity  

---

## 🔍 Verification & Testing

- Used `show ip route` to confirm route learning and summarization.  
- Verified redistribution between RIP v1 and v2 using `show ip protocols`.  
- Confirmed authentication using `debug ip rip` and neighbor status checks.  
- Tested passive interfaces to ensure updates were restricted as intended.  
- Verified route reachability and administrative routing control.  

---

## 🧾 Summary
This lab demonstrates an **enterprise-level understanding of RIP routing concepts** — focusing not just on connectivity, but also on **control, optimization, and security** of routing behavior.  
It bridges foundational **CCNA knowledge** with practical, real-world network engineering tasks such as **route control, authentication, and multi-domain interoperability**.

---

## 👤 Author
**Hamees Nisar**  
*Cybersecurity and Networking Student*  

📘 [LinkedIn](https://www.linkedin.com/in/hameesnisar/)  

