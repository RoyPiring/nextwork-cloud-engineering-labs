# CI/CD Automation Engineering

**Domain:** Software Delivery & DevOps

This engineering domain builds automated software delivery pipelines using AWS DevOps services, from infrastructure as code to continuous deployment. Demonstrates production-ready delivery automation and DevOps maturity.

## Domain Overview

This domain tells the story of building automated, repeatable software delivery following principal engineering methodology. We progress from manual processes to fully automated CI/CD pipelines, documenting each automation decision and its impact on reliability, security, and velocity.

## Navigation

- **[Business Context](./business-context.md)** - Problem statement, requirements, and constraints
- **[Architecture](./architecture.md)** - System design, components, and integration patterns
- **[Implementation](./implementation.md)** - Step-by-step implementation guide
- **[Validation](./validation.md)** - Testing, verification, and success criteria
- **[Executions](./executions/)** - Detailed execution guides for specific automation patterns

## Executions

The `executions/` directory contains detailed guides for specific automation implementations:

1. **[CI/CD Introduction](./executions/cicd-introduction.md)** - DevOps principles and CI/CD concepts
2. **[Environment Bootstrap](./executions/environment-bootstrap.md)** - Development environment setup (VS Code)
3. **[Idempotent Provisioning](./executions/idempotent-provisioning.md)** - Infrastructure as Code with Terraform
4. **[Infrastructure CloudFormation](./executions/infrastructure-cloudformation.md)** - AWS-native infrastructure automation
5. **[Source Control GitHub](./executions/source-control-github.md)** - GitHub integration and workflows
6. **[Package Management CodeArtifact](./executions/package-management-codeartifact.md)** - Dependency and artifact management
7. **[Build Automation CodeBuild](./executions/build-automation-codebuild.md)** - Automated build and test execution
8. **[Rollback Procedure](./executions/rollback-procedure.md)** - Deployment automation with CodeDeploy
9. **[Guardrail Enforcement](./executions/guardrail-enforcement.md)** - Complete CI/CD pipeline orchestration

## Principal Engineering Decisions

1. **IaC Tool Selection:** Terraform vs. CloudFormation tradeoffs
2. **Build Strategy:** Managed vs. self-hosted build infrastructure
3. **Deployment Model:** Blue/green vs. rolling vs. canary deployments
4. **Pipeline Orchestration:** CodePipeline vs. alternatives
5. **Cost vs. Velocity:** Balancing automation investment with delivery speed

## Prerequisites

- AWS account setup and fundamentals
- Basic understanding of software development lifecycle
- VPC Networking Engineering (recommended)
- Application Architecture Engineering (recommended)

## Related Domains

- **Application Architecture Engineering** - Applications to deploy via CI/CD
- **Security and Compliance Engineering** - DevSecOps practices
- **VPC Networking Engineering** - Network-aware deployment automation

