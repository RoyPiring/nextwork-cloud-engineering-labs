# Architecture: VPC Networking Engineering

## System Design

The VPC networking architecture provides logically isolated virtual networks with controlled connectivity, security boundaries, and observability.

## Core Components

### 1. Virtual Private Cloud (VPC)
- Logically isolated virtual network
- Custom IP address range (CIDR block)
- Regional resource (spans multiple Availability Zones)

### 2. Subnets
- **Public Subnets:** Direct internet access via Internet Gateway
- **Private Subnets:** No direct internet access, use NAT Gateway for outbound
- **Isolated Subnets:** No internet access (neither inbound nor outbound)

### 3. Internet Gateway
- Provides internet connectivity for public subnets
- Enables bidirectional internet access
- One per VPC

### 4. NAT Gateway
- Provides outbound internet access for private subnets
- Managed service with high availability
- Regional resource (one per Availability Zone for redundancy)

### 5. Route Tables
- Control traffic routing within VPC
- Define paths to internet, VPC endpoints, and peered VPCs
- Associated with subnets

### 6. Security Groups
- Stateful firewall at instance level
- Inbound and outbound rules
- Default deny, explicit allow

### 7. Network ACLs (NACLs)
- Stateless firewall at subnet level
- Additional layer of security
- Default allow, explicit deny

### 8. VPC Endpoints
- **Gateway Endpoints:** S3, DynamoDB (free)
- **Interface Endpoints:** PrivateLink for other AWS services
- Private connectivity without internet

### 9. VPC Peering
- Connect two VPCs
- Route table configuration required
- Non-transitive (A→B and B→C does not imply A→C)

### 10. Transit Gateway
- Centralized hub for multi-VPC connectivity
- Transitive routing
- Supports VPN and Direct Connect

## Architecture Patterns

### Pattern 1: Basic VPC with Public/Private Subnets
```
VPC (10.0.0.0/16)
├── Public Subnet (10.0.1.0/24) → Internet Gateway
└── Private Subnet (10.0.2.0/24) → NAT Gateway
```

### Pattern 2: Multi-AZ High Availability
```
VPC (10.0.0.0/16)
├── AZ-1
│   ├── Public Subnet (10.0.1.0/24)
│   └── Private Subnet (10.0.2.0/24)
└── AZ-2
    ├── Public Subnet (10.0.3.0/24)
    └── Private Subnet (10.0.4.0/24)
```

### Pattern 3: VPC Endpoints for Private Service Access
```
Private Subnet → VPC Endpoint → AWS Service (S3, DynamoDB, etc.)
(No internet required)
```

### Pattern 4: Multi-VPC Hub-and-Spoke
```
Transit Gateway
├── VPC-1 (Production)
├── VPC-2 (Development)
└── VPC-3 (Shared Services)
```

## Integration Points

- **Compute Services:** EC2, ECS, EKS, Lambda (VPC configuration)
- **Storage Services:** S3 (VPC endpoints), EBS (within VPC)
- **Database Services:** RDS, Aurora, DynamoDB (VPC endpoints)
- **CDN:** CloudFront (origin in VPC)
- **Monitoring:** VPC Flow Logs, CloudWatch

## Security Architecture

### Defense-in-Depth Layers

1. **Network Level:** Subnet isolation, route tables
2. **Firewall Level:** Security groups, NACLs
3. **Service Level:** VPC endpoints, service control policies
4. **Application Level:** Application-level security controls

### Security Boundaries

- **Public Boundary:** Internet Gateway, public subnets
- **Private Boundary:** NAT Gateway, private subnets
- **Isolated Boundary:** No internet, VPC endpoints only
- **Cross-VPC Boundary:** Peering, Transit Gateway with route controls

## Scalability Considerations

- **Address Space:** Plan CIDR blocks for growth
- **Subnet Sizing:** Allocate sufficient IP addresses per subnet
- **Route Table Limits:** Consider route table size limits
- **Peering Limits:** Plan for multi-VPC connectivity patterns

## Cost Optimization

- **NAT Gateway:** Use per-AZ for HA, consider NAT Instance for cost savings
- **VPC Endpoints:** Gateway endpoints (free) vs. Interface endpoints (cost)
- **Data Transfer:** Minimize cross-AZ and internet data transfer
- **Flow Logs:** Enable selectively to manage costs

