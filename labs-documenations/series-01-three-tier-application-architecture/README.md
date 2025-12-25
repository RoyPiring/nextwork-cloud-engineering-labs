# Three-Tier Application Architecture Series

**Rank:** 1 (Highest Feature Project Priority)

This series demonstrates complete full-stack cloud-native application architecture, from serverless functions to containerized workloads. The three-tier web application showcases principal engineering decision-making in service selection, integration patterns, and scalability design.

## Principal Engineering Story

This series tells the story of building a production-ready cloud application following principal engineering methodology. We start with foundational serverless patterns, build up to complete application architecture, and then explore advanced container orchestration.

### The Journey

**Foundation (Labs 1-2):** We begin with serverless fundamentals - understanding Lambda functions and API integration patterns. These building blocks establish the core execution model for our application.

**Integration (Lab 3):** We combine all components into a complete three-tier architecture, demonstrating how presentation, logic, and data tiers work together in a cloud-native design. This is our showcase feature project.

**Evolution (Labs 4-9):** We explore alternative deployment patterns - containers, orchestration, and Kubernetes - showing how the same application principles apply across different compute models.

## Learning Path

### 1. Serverless Foundation: Lambda
**File:** `01-serverless-foundation-lambda.md`

**Principal Engineering Focus:** Understanding serverless execution model and IAM boundaries

- Lambda function development
- Execution roles and permissions
- DynamoDB integration patterns
- Function testing and debugging
- **Decision Point:** When to use serverless vs. traditional compute

**Prerequisites:** standalone-labs/prerequisite-fundamentals

### 2. API Layer: Gateway + Lambda
**File:** `02-api-layer-gateway-lambda.md`

**Principal Engineering Focus:** Building scalable API interfaces with managed services

- RESTful API creation with API Gateway
- Lambda integration patterns
- Request/response handling
- API versioning and stages
- **Decision Point:** API Gateway vs. Application Load Balancer for serverless

**Prerequisites:** Lab 1 (Lambda foundation)

### 3. Complete Three-Tier Application
**File:** `03-complete-three-tier-application.md`

**Principal Engineering Focus:** End-to-end application architecture with separation of concerns

- **Presentation Tier:** S3 + CloudFront for static content delivery
- **Logic Tier:** API Gateway + Lambda for request handling
- **Data Tier:** DynamoDB for data persistence
- CORS configuration and cross-tier communication
- **Decision Point:** Three-tier vs. microservices architecture tradeoffs
- **Showcase Project:** This is the primary feature project demonstrating full-stack cloud architecture

**Prerequisites:** Labs 1-2, series-04-managed-database-services (DynamoDB)

### 4. Container Deployment: Elastic Beanstalk
**File:** `04-container-deployment-elastic-beanstalk.md`

**Principal Engineering Focus:** Platform-as-a-Service deployment patterns

- Docker containerization
- Elastic Beanstalk platform configuration
- Application environment management
- Auto-scaling configuration
- **Decision Point:** PaaS vs. serverless vs. container orchestration

**Prerequisites:** Lab 3 (understanding application architecture)

### 5. Container Registry: ECR
**File:** `05-container-registry-ecr.md`

**Principal Engineering Focus:** Container image lifecycle management

- ECR repository setup
- Image versioning and tagging
- Cross-account access patterns
- Registry security and access control
- **Decision Point:** ECR vs. other container registries

**Prerequisites:** Lab 4 (container deployment)

### 6-9. Kubernetes Orchestration: EKS (Parts 1-4)
**Files:** 
- `06-kubernetes-cluster-eks-part1.md` - Cluster creation and networking
- `07-kubernetes-deployment-eks-part2.md` - Application deployment
- `08-kubernetes-scaling-eks-part3.md` - Auto-scaling and monitoring
- `09-kubernetes-advanced-eks-part4.md` - Advanced networking and security

**Principal Engineering Focus:** Container orchestration at scale

- EKS cluster architecture
- Pod networking and service discovery
- Horizontal and vertical pod autoscaling
- Cluster monitoring and observability
- Advanced networking (CNI) and security policies
- **Decision Point:** EKS vs. ECS vs. serverless for container workloads

**Prerequisites:** Labs 4-5 (container fundamentals)

## Series Goals

By completing this series, you will:
- Design and implement complete cloud-native applications
- Understand serverless, container, and orchestration patterns
- Make informed decisions about compute service selection
- Implement auto-scaling and monitoring strategies
- Apply principal engineering methodology to application architecture

## Principal Engineering Decisions

Throughout this series, we document key architectural decisions:

1. **Serverless vs. Containers:** When to choose Lambda vs. ECS/EKS
2. **API Design:** RESTful patterns and versioning strategies
3. **Data Access:** Direct database access vs. API abstraction
4. **Scaling Strategy:** Auto-scaling configuration and tradeoffs
5. **Cost Optimization:** Right-sizing compute resources

## Prerequisites

- standalone-labs/prerequisite-fundamentals
- series-02-vpc-networking-architecture (recommended for EKS labs)
- series-04-managed-database-services (for data tier)

## Next Steps

After completing this series, proceed to:
- **series-03-devops-cicd-automation** for automated deployment
- **series-05-cloud-security-identity** for security hardening
- **series-04-managed-database-services** for advanced data patterns

## Feature Project Showcase

**Lab 3 (Complete Three-Tier Application)** is the primary feature project that demonstrates:
- Full-stack cloud architecture
- Service integration patterns
- Production-ready design decisions
- End-to-end user experience

This project showcases principal engineering capabilities in cloud-native application design.
