# Application Architecture Engineering

**Domain:** Full-Stack Application Development

This engineering domain demonstrates complete full-stack cloud-native application architecture, from serverless functions to containerized workloads. The three-tier web application showcases principal engineering decision-making in service selection, integration patterns, and scalability design.

## Domain Overview

This domain tells the story of building a production-ready cloud application following principal engineering methodology. We start with foundational serverless patterns, build up to complete application architecture, and then explore advanced container orchestration.

## Navigation

- **[Business Context](./business-context.md)** - Problem statement, requirements, and constraints
- **[Architecture](./architecture.md)** - System design, components, and integration patterns
- **[Implementation](./implementation.md)** - Step-by-step implementation guide
- **[Validation](./validation.md)** - Testing, verification, and success criteria
- **[Executions](./executions/)** - Detailed execution guides for specific application patterns

## Executions

The `executions/` directory contains detailed guides for specific application implementations.

## Principal Engineering Decisions

1. **Serverless vs. Containers:** When to choose Lambda vs. ECS/EKS
2. **API Design:** RESTful patterns and versioning strategies
3. **Data Access:** Direct database access vs. API abstraction
4. **Scaling Strategy:** Auto-scaling configuration and tradeoffs
5. **Cost Optimization:** Right-sizing compute resources

## Prerequisites

- AWS account setup and fundamentals
- VPC Networking Engineering (recommended for EKS labs)
- Database Services Engineering (for data tier)

## Related Domains

- **CI/CD Automation Engineering** - Automated deployment
- **Security and Compliance Engineering** - Security hardening
- **Database Services Engineering** - Advanced data patterns

