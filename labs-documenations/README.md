# Lab Documentation Series

This directory contains organized lab documentation grouped into **principal engineering series** that demonstrate production-ready implementations with documented tradeoffs and validated patterns. Series are ranked by feature project priority (1 = highest priority for showcase projects).

## Series Ranking (Feature Project Priority)

Series are ranked 1-9 based on their value as feature projects, with 1 being the highest priority for showcasing principal engineering capabilities:

1. **series-01-three-tier-application-architecture** - Complete full-stack application (highest feature project value)
2. **series-02-vpc-networking-architecture** - Foundational infrastructure architecture
3. **series-03-devops-cicd-automation** - Production-ready delivery automation
4. **series-04-managed-database-services** - Data layer architecture
5. **series-05-cloud-security-identity** - Security and governance
6. **series-06-conversational-ai-lex** - Conversational AI applications
7. **series-07-rag-applications** - Retrieval-Augmented Generation applications
8. **series-08-data-engineering-analytics** - Data engineering workflows
9. **series-09-ai-powered-development** - Developer productivity tools

## Structure Overview

### Standalone Labs
**Path:** `standalone-labs/`

Individual labs that are not part of series, including prerequisites and supporting resources:

- **prerequisite-fundamentals** - Foundation labs required before starting any series (AWS account setup and cloud computing fundamentals)
- **ai-ml-tools** - Standalone AI/ML tools (Transcribe, Agents, Prompt Engineering)
- **storage** - Storage fundamentals (S3 hosting, multi-cloud storage)

**Start here if:** You're new to AWS (begin with `standalone-labs/prerequisite-fundamentals`)

### Principal Engineering Series

These numbered series provide complete, production-ready implementations from design to deployment:

1. **series-01-three-tier-application-architecture** - Complete full-stack serverless application (Lambda, API Gateway, DynamoDB, S3, CloudFront)
2. **series-02-vpc-networking-architecture** - Comprehensive VPC architecture, security, connectivity, and monitoring
3. **series-03-devops-cicd-automation** - Infrastructure as Code and automated CI/CD pipelines
4. **series-04-managed-database-services** - Managed database services (DynamoDB, Aurora) with optimization
5. **series-05-cloud-security-identity** - Security fundamentals and advanced services (IAM, KMS, GuardDuty)
6. **series-06-conversational-ai-lex** - Amazon Lex conversational AI implementation
7. **series-07-rag-applications** - RAG (Retrieval-Augmented Generation) implementations
8. **series-08-data-engineering-analytics** - Data engineering with Model Context Protocol
9. **series-09-ai-powered-development** - AI-powered development environments (Cursor, Claude Code, MCP)

## Principal Engineering Approach

Each series follows a **decision-first methodology**:
- **Problem statement** and context
- **Architecture decisions** with documented tradeoffs
- **Validated implementations** with production patterns
- **Security, reliability, and cost analysis**
- **Lessons learned** and optimization opportunities

## Recommended Learning Paths

### Path 1: Full-Stack Cloud Engineer
```
standalone-labs/prerequisite-fundamentals
  → standalone-labs/storage (optional)
  → series-02-vpc-networking-architecture
  → series-01-three-tier-application-architecture
  → series-04-managed-database-services
  → series-03-devops-cicd-automation
  → series-05-cloud-security-identity (applied throughout)
```

### Path 2: AI/ML Engineer
```
standalone-labs/prerequisite-fundamentals
  → series-09-ai-powered-development
  → series-06-conversational-ai-lex
  → series-07-rag-applications
  → series-08-data-engineering-analytics
```

### Path 3: DevOps Engineer
```
standalone-labs/prerequisite-fundamentals
  → series-02-vpc-networking-architecture
  → series-01-three-tier-application-architecture
  → series-03-devops-cicd-automation
  → series-05-cloud-security-identity
```

### Path 4: Security Specialist
```
standalone-labs/prerequisite-fundamentals
  → series-05-cloud-security-identity
  → series-02-vpc-networking-architecture (security-focused)
  → All other series (security perspective)
```

## Series Dependencies

```
standalone-labs/prerequisite-fundamentals (required for all)
    ├── standalone-labs (other standalone labs, optional)
    ├── series-02-vpc-networking-architecture
    │   ├── series-01-three-tier-application-architecture
    │   │   ├── series-04-managed-database-services
    │   │   └── series-03-devops-cicd-automation
    │   └── series-05-cloud-security-identity (applies to all)
    ├── series-09-ai-powered-development
    │   ├── series-08-data-engineering-analytics
    │   ├── series-06-conversational-ai-lex
    │   └── series-07-rag-applications
    └── series-05-cloud-security-identity (cross-cutting concern)
```

## Feature Project Recommendations

For showcasing principal engineering capabilities, prioritize these series:

**Tier 1 (Highest Impact):**
- **series-01-three-tier-application-architecture** - Demonstrates full-stack cloud-native application design
- **series-02-vpc-networking-architecture** - Shows infrastructure architecture expertise

**Tier 2 (High Impact):**
- **series-03-devops-cicd-automation** - Production-ready delivery capabilities
- **series-04-managed-database-services** - Data architecture and optimization

**Tier 3 (Specialized):**
- **series-05-cloud-security-identity** - Security governance (often integrated into other projects)
- **series-06-conversational-ai-lex** - Conversational AI specialization
- **series-07-rag-applications** - RAG/AI specialization
- **series-08-data-engineering-analytics** - Data engineering specialization
- **series-09-ai-powered-development** - Developer productivity (supporting role)

## How to Use This Repository

1. **Complete Prerequisites First**: Always start with `standalone-labs/prerequisite-fundamentals`
2. **Follow Series Order**: Each series builds on previous concepts
3. **Read Series READMEs**: Each series contains detailed progression guides
4. **Cross-Reference**: Many labs reference concepts from other series
5. **Practice End-to-End**: Combine labs from multiple series for comprehensive projects

## Naming Convention

- **Standalone Labs**: `standalone-labs/[category]` - Prerequisites and supporting labs
- **Principal Series**: `series-[rank]-[descriptive-name]` - Ranked by feature project priority (1-9)

## Contributing

When adding new labs:
1. Determine if it's a standalone lab or part of a series
2. Place in appropriate folder following naming conventions
3. Update the series README with the new lab
4. Document learning objectives, prerequisites, and dependencies

## Questions?

Refer to individual series READMEs for detailed information about each learning path.
