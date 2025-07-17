# 🌐 Phase 3: Network Security – Notes

## ✅ Key Concepts

### 🔷 VPC (Virtual Private Cloud)
- Isolated cloud network environment
- Default VPC exists in each region (can create custom)
- Contains subnets, route tables, gateways, security settings

### 🔶 Subnets
- Public Subnet: Connected to the Internet via Internet Gateway
- Private Subnet: No direct Internet access (can use NAT Gateway)
- Recommended to place databases, internal apps in private subnets

### 🔄 Route Tables
- Define how traffic flows within the VPC
- Public subnet routes to Internet Gateway (`0.0.0.0/0`)
- Private subnet routes to NAT Gateway (for outbound only)

### 🔐 Security Groups (SGs)
- Instance-level virtual firewall
- Stateful: Return traffic is automatically allowed
- Can control inbound/outbound by port, IP, CIDR block

### 🔒 Network ACLs (NACLs)
- Subnet-level firewall
- Stateless: Must explicitly allow return traffic
- Rarely used unless high-level control is needed

## ✅ Best Practices
- Deny by default (allow only what’s necessary)
- Never expose ports like SSH (22) or RDP (3389) to `0.0.0.0/0`
- Use public subnet only for bastion hosts or load balancers
- Segment VPC using private subnets for sensitive services
