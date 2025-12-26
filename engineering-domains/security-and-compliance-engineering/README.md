# Security and Compliance Engineering

**Domain:** Security & Governance

This engineering domain covers security fundamentals and advanced security services on AWS, implementing defense-in-depth strategies. Demonstrates security-first thinking and governance practices.

## Domain Overview

This domain tells the story of implementing comprehensive security controls following principal engineering methodology. We progress from identity and access management to advanced threat detection, documenting security decisions and their tradeoffs.

## Navigation

- **[Business Context](./business-context.md)** - Problem statement, requirements, and constraints
- **[Architecture](./architecture.md)** - System design, components, and integration patterns
- **[Implementation](./implementation.md)** - Step-by-step implementation guide
- **[Validation](./validation.md)** - Testing, verification, and success criteria
- **[Executions](./executions/)** - Detailed execution guides for specific security patterns

## Executions

The `executions/` directory contains detailed guides for specific security implementations:

1. **[IAM Least Privilege](./executions/iam-least-privilege.md)** - Identity and access management with least-privilege principles
2. **[Boundary Enforcement](./executions/boundary-enforcement.md)** - Network and service boundary security
3. **[Evidence Collection](./executions/evidence-collection.md)** - Security monitoring and audit logging
4. **[Compliance Checklist](./executions/compliance-checklist.md)** - Compliance validation and reporting

## Principal Engineering Decisions

1. **Access Model:** IAM roles vs. users vs. federated identity
2. **Encryption Strategy:** Key management and rotation policies
3. **Secrets Storage:** Managed services vs. external vaults
4. **Threat Detection:** Native vs. third-party solutions
5. **Security Monitoring:** Cost vs. coverage tradeoffs

## Prerequisites

- AWS account setup and fundamentals
- IAM basics recommended
- Understanding of security fundamentals

## Related Domains

- **VPC Networking Engineering** - Network security controls
- **CI/CD Automation Engineering** - DevSecOps integration
- **Application Architecture Engineering** - Application security

