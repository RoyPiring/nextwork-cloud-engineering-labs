# VPC Networking Engineering

**Domain:** Network Infrastructure & Connectivity

This engineering domain covers comprehensive cloud networking architecture through hands-on VPC design, security configuration, and connectivity patterns. Demonstrates foundational infrastructure design critical for all cloud deployments.

## Domain Overview

This domain tells the story of designing secure, scalable network infrastructure following principal engineering methodology. We progress from foundational concepts to advanced networking patterns, documenting each decision and its tradeoffs.

## Navigation

- **[Business Context](./business-context.md)** - Problem statement, requirements, and constraints
- **[Architecture](./architecture.md)** - System design, components, and integration patterns
- **[Implementation](./implementation.md)** - Step-by-step implementation guide
- **[Validation](./validation.md)** - Testing, verification, and success criteria
- **[Executions](./executions/)** - Detailed execution guides for specific networking patterns

## Executions

The `executions/` directory contains detailed guides for specific networking implementations:

1. **[Subnet Segmentation](./executions/subnet-segmentation.md)** - Network isolation and address planning
2. **[Routing Boundaries](./executions/routing-boundaries.md)** - Route table configuration and traffic control
3. **[Flow Logs Validation](./executions/flow-logs-validation.md)** - Network monitoring and observability
4. **[Isolated Network Test](./executions/isolated-network-test.md)** - Security boundary validation

## Learning Path

### Foundation
- Networking concepts and architecture
- VPC design principles
- Address planning and CIDR block sizing

### Security & Isolation
- Network security boundaries
- Defense-in-depth networking strategies
- Private subnet configuration

### Integration & Connectivity
- Service connectivity patterns
- Multi-VPC connectivity
- CDN and edge integration

### Advanced Patterns
- Network monitoring and troubleshooting
- Advanced peering patterns
- Cost optimization strategies

## Principal Engineering Decisions

Throughout this domain, we document key networking decisions:

1. **Address Planning:** CIDR block sizing and subnet allocation
2. **Security Model:** Security groups, NACLs, and defense-in-depth
3. **Connectivity Patterns:** Internet gateway, NAT, VPC endpoints
4. **Multi-VPC Strategy:** Peering vs. Transit Gateway
5. **Cost Optimization:** Right-sizing network resources

## Prerequisites

- AWS account setup and fundamentals
- Basic understanding of IP addressing and routing
- Understanding of network security concepts

## Related Domains

- **Application Architecture Engineering** - Deploy workloads in your VPC
- **Security and Compliance Engineering** - Advanced security controls
- **CI/CD Automation Engineering** - Network-aware deployment automation

