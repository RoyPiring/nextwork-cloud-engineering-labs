# Cloud Security & Identity Series

**Rank:** 5 (Feature Project Priority)

This series covers security fundamentals and advanced security services on AWS, implementing defense-in-depth strategies. Demonstrates security-first thinking and governance practices.

## Principal Engineering Story

This series tells the story of implementing comprehensive security controls following principal engineering methodology. We progress from identity and access management to advanced threat detection, documenting security decisions and their tradeoffs.

### The Journey

**Identity Foundation (Lab 1):** We establish identity and access management, the foundation of all security controls. This is where security begins.

**Encryption (Lab 2):** We implement encryption at rest and in transit, protecting data confidentiality through key management.

**Secrets Management (Lab 3):** We manage application secrets securely, preventing credential exposure and enabling rotation.

**Threat Detection (Lab 4):** We implement automated threat detection, identifying and responding to security events.

**Monitoring (Lab 5):** We establish security monitoring and observability, enabling continuous security assessment.

## Learning Path

### 1. Identity & Access Management (IAM)
**File:** `01-identity-access-management-iam.md`

**Principal Engineering Focus:** Implementing least-privilege access controls

- IAM fundamentals: users, groups, roles, and policies
- Policy creation and management
- Least privilege principles
- Cross-account access patterns
- **Decision Point:** IAM roles vs. users vs. federated access

**Prerequisites:** standalone-labs/prerequisite-fundamentals

### 2. Encryption: Key Management Service (KMS)
**File:** `02-encryption-key-management-kms.md`

**Principal Engineering Focus:** Implementing encryption at rest and in transit

- Customer-managed keys (CMK) vs. AWS-managed keys
- Key rotation policies and lifecycle management
- Encryption integration with services
- Key access control and policies
- **Decision Point:** CMK vs. AWS-managed keys vs. external key management

**Prerequisites:** Lab 1 (IAM foundation)

### 3. Secrets Management
**File:** `03-secrets-management.md`

**Principal Engineering Focus:** Secure credential and secret storage

- Secrets Manager setup and configuration
- Automatic secret rotation
- Integration with applications
- Secret access policies
- **Decision Point:** Secrets Manager vs. Parameter Store vs. external vaults

**Prerequisites:** Lab 1 (IAM foundation)

### 4. Threat Detection: GuardDuty
**File:** `04-threat-detection-guardduty.md`

**Principal Engineering Focus:** Automated security threat detection

- GuardDuty configuration and findings
- Threat detection service integration
- Finding types and severity classification
- Integration with security workflows
- **Decision Point:** GuardDuty vs. other threat detection solutions

**Prerequisites:** Labs 1-3 (IAM, encryption, secrets)

### 5. Security Monitoring
**File:** `05-security-monitoring.md`

**Principal Engineering Focus:** Security observability and incident response

- CloudWatch security metrics
- CloudTrail log analysis
- Security event detection and alerting
- Incident response procedures
- **Decision Point:** Native AWS monitoring vs. third-party SIEM

**Prerequisites:** Labs 1-4 (all security controls)

## Series Goals

By completing this series, you will:
- Implement least privilege access controls
- Encrypt data at rest and in transit
- Manage secrets securely
- Monitor and detect security threats
- Respond to security incidents
- Apply principal engineering methodology to security architecture

## Principal Engineering Decisions

Throughout this series, we document key security decisions:

1. **Access Model:** IAM roles vs. users vs. federated identity
2. **Encryption Strategy:** Key management and rotation policies
3. **Secrets Storage:** Managed services vs. external vaults
4. **Threat Detection:** Native vs. third-party solutions
5. **Security Monitoring:** Cost vs. coverage tradeoffs

## Prerequisites

- standalone-labs/prerequisite-fundamentals
- IAM basics recommended
- Understanding of security fundamentals

## Next Steps

After completing this series, proceed to:
- Apply security practices to all other series
- **series-02-vpc-networking-architecture** for network security
- **series-03-devops-cicd-automation** for DevSecOps integration
- **series-06-conversational-ai-lex** for AI security considerations
