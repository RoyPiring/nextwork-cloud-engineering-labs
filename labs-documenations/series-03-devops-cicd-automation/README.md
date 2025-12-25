# DevOps & CI/CD Automation Series

**Rank:** 3 (High Feature Project Priority)

This series builds automated software delivery pipelines using AWS DevOps services, from infrastructure as code to continuous deployment. Demonstrates production-ready delivery automation and DevOps maturity.

## Principal Engineering Story

This series tells the story of building automated, repeatable software delivery following principal engineering methodology. We progress from manual processes to fully automated CI/CD pipelines, documenting each automation decision and its impact on reliability, security, and velocity.

### The Journey

**Foundation (Labs 1-2):** We establish the development environment and understand CI/CD principles. These labs set the foundation for automation.

**Infrastructure as Code (Labs 3-4):** We implement infrastructure automation using Terraform and CloudFormation, demonstrating repeatable infrastructure provisioning.

**Source Control & Packages (Labs 5-6):** We integrate source control and package management, establishing the foundation for automated builds.

**Build & Deploy (Labs 7-8):** We automate the build and deployment processes, reducing manual intervention and errors.

**Complete Pipeline (Lab 9):** We orchestrate all components into a complete CI/CD pipeline, demonstrating end-to-end automation.

## Learning Path

### 1. CI/CD Introduction
**File:** `01-cicd-introduction.md`

**Principal Engineering Focus:** Understanding DevOps principles and CI/CD value proposition

- DevOps principles and practices
- CI/CD concepts and benefits
- Pipeline architecture overview
- 7-day challenge framework
- **Decision Point:** Manual deployment vs. automated CI/CD

**Prerequisites:** standalone-labs/prerequisite-fundamentals

### 2. Development Environment: VS Code
**File:** `02-development-environment-vscode.md`

**Principal Engineering Focus:** Setting up productive development workflows

- VS Code setup and configuration
- AWS CLI configuration
- Local testing workflows
- Development best practices
- **Decision Point:** IDE selection and development tooling

**Prerequisites:** Lab 1 (CI/CD concepts)

### 3. Infrastructure as Code: Terraform
**File:** `03-infrastructure-as-code-terraform.md`

**Principal Engineering Focus:** Declarative infrastructure provisioning

- Terraform basics and resource provisioning
- State management and collaboration
- Module development and reuse
- **Decision Point:** Terraform vs. CloudFormation vs. CDK

**Prerequisites:** Lab 2 (development environment)

### 4. Infrastructure as Code: CloudFormation
**File:** `04-infrastructure-as-code-cloudformation.md`

**Principal Engineering Focus:** Native AWS infrastructure automation

- CloudFormation templates and stacks
- Parameters, outputs, and nested stacks
- Stack management and updates
- **Decision Point:** CloudFormation vs. Terraform for AWS-native resources

**Prerequisites:** Lab 3 (IaC concepts)

### 5. Source Control: GitHub Integration
**File:** `05-source-control-github-integration.md`

**Principal Engineering Focus:** Integrating source control with AWS services

- GitHub Actions integration
- Repository webhooks
- Branch protection and workflows
- **Decision Point:** GitHub vs. CodeCommit vs. GitLab

**Prerequisites:** Lab 2 (development environment)

### 6. Package Management: CodeArtifact
**File:** `06-package-management-codeartifact.md`

**Principal Engineering Focus:** Managing dependencies and artifacts

- Package repository setup
- Dependency management and versioning
- Integration with build pipelines
- **Decision Point:** CodeArtifact vs. other package repositories

**Prerequisites:** Lab 5 (source control)

### 7. Build Automation: CodeBuild
**File:** `07-build-automation-codebuild.md`

**Principal Engineering Focus:** Automated build and test execution

- Build environment configuration
- Build specifications and artifacts
- Build optimization and caching
- **Decision Point:** CodeBuild vs. self-hosted build servers

**Prerequisites:** Labs 5-6 (source control and packages)

### 8. Deployment Automation: CodeDeploy
**File:** `08-deployment-automation-codedeploy.md`

**Principal Engineering Focus:** Controlled, repeatable deployments

- Deployment strategies (blue/green, rolling)
- Application deployment configuration
- Rollback procedures
- **Decision Point:** CodeDeploy vs. other deployment tools

**Prerequisites:** Lab 7 (build automation)

### 9. Complete CI/CD Pipeline
**File:** `09-complete-cicd-pipeline.md`

**Principal Engineering Focus:** End-to-end delivery automation

- Pipeline orchestration with CodePipeline
- Stage configuration and approval gates
- Pipeline monitoring and troubleshooting
- **Decision Point:** CodePipeline vs. other orchestration tools
- **Showcase Project:** Complete automated delivery pipeline

**Prerequisites:** Labs 1-8 (all previous labs)

## Series Goals

By completing this series, you will:
- Implement infrastructure as code practices
- Build automated CI/CD pipelines
- Integrate source control with AWS services
- Automate testing and deployment
- Implement deployment strategies and rollback procedures
- Apply principal engineering methodology to delivery automation

## Principal Engineering Decisions

Throughout this series, we document key automation decisions:

1. **IaC Tool Selection:** Terraform vs. CloudFormation tradeoffs
2. **Build Strategy:** Managed vs. self-hosted build infrastructure
3. **Deployment Model:** Blue/green vs. rolling vs. canary deployments
4. **Pipeline Orchestration:** CodePipeline vs. alternatives
5. **Cost vs. Velocity:** Balancing automation investment with delivery speed

## Prerequisites

- standalone-labs/prerequisite-fundamentals
- Basic understanding of software development lifecycle
- series-02-vpc-networking-architecture (recommended)
- series-01-three-tier-application-architecture (recommended)

## Next Steps

After completing this series, proceed to:
- **series-05-cloud-security-identity** for DevSecOps practices
- Apply CI/CD to projects from other series
- **series-06-conversational-ai-lex** for ML model deployment pipelines

## Feature Project Showcase

**Lab 9 (Complete CI/CD Pipeline)** is the primary feature project that demonstrates:
- End-to-end automation
- Production-ready delivery workflows
- Integration of multiple AWS services
- Principal engineering decision-making in automation
