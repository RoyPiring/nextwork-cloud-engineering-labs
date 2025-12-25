# Three-Tier Application Architecture Series

**Rank:** 1 (Highest Feature Project Priority)

This series demonstrates complete full-stack cloud-native application architecture, from serverless functions to containerized workloads. The three-tier web application showcases principal engineering decision-making in service selection, integration patterns, and scalability design.

## Learning Path

### 1. AWS Lambda
**File:** `aws-compute-lambda.md`

- Serverless function development
- Lambda execution roles and permissions
- DynamoDB integration
- Function testing and debugging

### 2. API Gateway Integration
**File:** `aws-compute-api.md`

- RESTful API creation
- Lambda integration
- Request/response handling
- API versioning

### 3. Three-Tier Web Application
**File:** `aws-compute-threetier.md`

- Complete three-tier architecture
- Presentation tier (S3 + CloudFront)
- Logic tier (API Gateway + Lambda)
- Data tier (DynamoDB)
- CORS configuration
- End-to-end integration

### 4. Elastic Beanstalk
**File:** `aws-compute-eb.md`

- Platform-as-a-Service deployment
- Application environment management
- Auto-scaling configuration
- Environment health monitoring

### 5. Elastic Container Registry (ECR)
**File:** `aws-compute-ecr.md`

- Container image storage
- Image versioning and tagging
- Registry security and access control
- Integration with ECS/EKS

### 6. Elastic Kubernetes Service (EKS) - Part 1
**File:** `aws-compute-eks1.md`

- EKS cluster creation
- Cluster networking
- Node group configuration

### 7. Elastic Kubernetes Service (EKS) - Part 2
**File:** `aws-compute-eks2.md`

- Application deployment
- Service and ingress configuration
- Pod networking

### 8. Elastic Kubernetes Service (EKS) - Part 3
**File:** `aws-compute-eks3.md`

- Auto-scaling (HPA/VPA)
- Cluster monitoring
- Log aggregation

### 9. Elastic Kubernetes Service (EKS) - Part 4
**File:** `aws-compute-eks4.md`

- Advanced networking (CNI)
- Security policies
- Multi-region considerations

## Series Goals

By completing this series, you will:
- Deploy serverless applications with Lambda
- Build and deploy containerized applications
- Manage Kubernetes clusters on AWS
- Understand compute service selection criteria
- Implement auto-scaling and monitoring

## Prerequisites

- AWS Account Setup (standalone-labs/prerequisite-fundamentals)
- series-02-vpc-networking-architecture recommended
- Basic understanding of containers and Kubernetes (for EKS labs)

## Next Steps

After completing this series, proceed to:
- **series-04-managed-database-services** for data persistence
- **series-03-devops-cicd-automation** for automated deployment
- **series-05-cloud-security-identity** for compute security hardening
- **standalone-labs/storage** for integrating storage with applications


