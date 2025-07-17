# 🧪 Phase 3: Network Security – Hands-on Log

## ✅ VPC Creation
- [x] Created custom VPC: `secure-lab-vpc`
- [x] CIDR: 10.0.0.0/16

## ✅ Subnet Setup
- [x] Public Subnet: `10.0.1.0/24`
- [x] Private Subnet: `10.0.2.0/24`

## ✅ Routing
- [x] Created and attached Internet Gateway
- [x] Public Subnet route table: `0.0.0.0/0` → IGW
- [x] Private Subnet route table: `0.0.0.0/0` → NAT Gateway

## ✅ EC2 and Security Group
- [x] Launched EC2 in Public Subnet
- [x] Security Group: Allow SSH (port 22) only from `my IP`
- [x] Verified instance is reachable via SSH from my IP only

## ✅ Bonus: NACL
- [ ] Created NACL to block all inbound port 22 (test denied access)
