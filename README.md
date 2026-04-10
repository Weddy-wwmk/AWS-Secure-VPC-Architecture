# ☁️ Secure 2-Tier AWS VPC Architecture
**Project by Weddy Karanja | AWS Cloud Club Captain, KCA University**

## 📌 Project Overview
This project demonstrates the design of a secure, production-ready network on AWS. By implementing a two-tier architecture, I isolated a backend database from the public internet while maintaining controlled access for authorized traffic.

---

## 🏗️ Implementation Steps
1. **Network Segmentation**: Created a custom VPC with a Public Subnet (Web) and a Private Subnet (DB).
2. **Secure Connectivity**: Deployed a **NAT Gateway** to allow the private DB to download updates without inbound internet exposure.
3. **Layered Security**: Configured **Security Groups** to ensure the DB only accepts traffic from the Web Server on Port 3306.

---

## 🚦 Verification & Proof of Work

### 1. Logical Topology
The final layout of the subnets and routing logic as mapped by AWS.
![VPC Map](./images/The-Visual-Map.png)

### 2. Security Group Audit
Confirmation that the Database traffic is restricted to the web tier source.
![Security Rules](./images/security-group-rule.png)

### 3. Network Isolation Test
Proved the database is reachable from within the VPC (Left) but blocked from the public internet (Right).
![Security Comparison](./images/vpc-security-comparison.png)

---
**Status:** ✅ Resources Terminated 
