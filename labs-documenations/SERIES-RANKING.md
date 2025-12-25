# Series Ranking & Naming

## Feature Project Priority Ranking (1 = Highest)

Series are ranked 1-9 based on their value as feature projects for showcasing principal engineering capabilities:

### Rank 1: series-01-three-tier-application-architecture
**Previous Name:** end-to-end-02-compute

**Why Rank 1:**
- Complete full-stack application demonstrating end-to-end cloud architecture
- Shows integration of multiple AWS services (Lambda, API Gateway, DynamoDB, S3, CloudFront)
- Production-ready pattern that showcases principal engineering decision-making
- Demonstrates separation of concerns, scalability, and service integration
- Most comprehensive feature project that tells a complete story

**Content:** Three-tier web application, Lambda functions, API Gateway, EKS, Elastic Beanstalk, ECR

---

### Rank 2: series-02-vpc-networking-architecture
**Previous Name:** end-to-end-01-networking

**Why Rank 2:**
- Foundational infrastructure architecture critical for all cloud deployments
- Demonstrates network design, security boundaries, and connectivity patterns
- Shows principal engineering thinking in infrastructure design
- Essential prerequisite for production workloads
- High visibility in enterprise environments

**Content:** VPC design, subnets, routing, security groups, VPC endpoints, peering, monitoring

---

### Rank 3: series-03-devops-cicd-automation
**Previous Name:** end-to-end-04-devops-cicd

**Why Rank 3:**
- Production-ready delivery automation and infrastructure as code
- Demonstrates modern DevOps practices and automation maturity
- Shows repeatability, testing, and deployment strategies
- High value for organizations adopting cloud-native practices
- Combines multiple tools (Terraform, CloudFormation, CI/CD pipelines)

**Content:** CI/CD pipelines, Terraform, CloudFormation, CodeBuild, CodeDeploy, CodePipeline

---

### Rank 4: series-04-managed-database-services
**Previous Name:** end-to-end-03-databases

**Why Rank 4:**
- Data layer architecture and optimization
- Demonstrates database selection, design, and performance tuning
- Critical component of most applications
- Shows understanding of data modeling and access patterns
- Important but often integrated into application projects

**Content:** DynamoDB, Aurora, query optimization, database web applications

---

### Rank 5: series-05-cloud-security-identity
**Previous Name:** end-to-end-05-security

**Why Rank 5:**
- Security and identity governance
- Demonstrates security-first thinking and compliance considerations
- Critical but often integrated into other projects rather than standalone
- Shows understanding of least privilege, encryption, and threat detection
- Important for enterprise but less visible as standalone feature project

**Content:** IAM, KMS, Secrets Manager, GuardDuty, security monitoring

---

### Rank 6: series-06-conversational-ai-lex
**Previous Name:** end-to-end-06-ai-ml (sub-series: 01-aws-lex-series)

**Why Rank 6:**
- Conversational AI application development
- Demonstrates modern AI capabilities and NLP integration
- Shows understanding of intent recognition, slot filling, and conversation flows
- High value but specialized domain
- Growing importance in customer-facing applications

**Content:** Amazon Lex chatbot implementation, multi-turn conversations, Lambda integration

---

### Rank 7: series-07-rag-applications
**Previous Name:** end-to-end-06-ai-ml (sub-series: 02-ai-rag-series)

**Why Rank 7:**
- Retrieval-Augmented Generation (RAG) application development
- Demonstrates knowledge-grounded AI and document retrieval patterns
- Shows understanding of vector databases, embeddings, and model integration
- Specialized domain with specific use cases
- Important for AI applications requiring accurate, context-aware responses

**Content:** Bedrock knowledge bases, RAG API implementation, CloudShell setup, web applications

---

### Rank 8: series-08-data-engineering-analytics
**Previous Name:** end-to-end-08-mcp-data-engineering

**Why Rank 8:**
- Data engineering and analytics workflows
- Demonstrates data pipeline design and optimization
- Specialized domain with specific use cases
- Shows understanding of data modeling and query optimization
- Important but less commonly showcased as primary feature project

**Content:** PostgreSQL, Docker, MCP integration, query optimization, data engineering

---

### Rank 9: series-09-ai-powered-development
**Previous Name:** end-to-end-07-ai-workspace

**Why Rank 9:**
- AI-powered development tools and productivity
- Demonstrates modern development workflows
- Supporting role rather than primary feature project
- Shows understanding of developer tooling and productivity
- Valuable for personal productivity but less visible as showcase project

**Content:** Cursor IDE, Claude Code, Model Context Protocol (MCP) setup

---

## Naming Rationale

Names were chosen to:
- **Clearly describe the content** - Each name reflects the primary focus
- **Use principal engineering terminology** - Terms like "architecture", "automation", "applications"
- **Be searchable and discoverable** - Descriptive names help find relevant content
- **Show progression** - Numbered ranking indicates feature project priority
- **Maintain consistency** - All follow `series-[rank]-[descriptive-name]` pattern

## Usage

- **For Feature Projects**: Start with Rank 1-3 for highest impact
- **For Learning**: Follow dependencies and prerequisites
- **For Specialization**: Ranks 6-9 focus on specific domains
- **For Integration**: Lower-ranked series often support higher-ranked ones

## Series Breakdown

**Core Infrastructure (Ranks 1-3):**
- Application architecture
- Networking architecture
- DevOps automation

**Supporting Services (Ranks 4-5):**
- Database services
- Security and identity

**Specialized Applications (Ranks 6-9):**
- Conversational AI
- RAG applications
- Data engineering
- Developer tools
