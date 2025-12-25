# Repository Structure Documentation

This document provides detailed guidance on the repository structure and organization principles.

## Directory Descriptions

### `/labs/`

Individual lab projects. Each lab is self-contained but may reference shared patterns.

**Lab Structure:**
```
labs/[lab-name]/
├── README.md              # Lab overview, problem statement, solution
├── decisions/             # Lab-specific ADRs
│   └── 0001-decision-name.md
├── docs/                  # Lab-specific documentation
│   ├── architecture.md    # Architecture diagrams and explanations
│   ├── security.md        # Threat model and security considerations
│   ├── cost-analysis.md   # Cost breakdown and guardrails
│   └── tradeoffs.md       # Documented tradeoffs
├── infrastructure/        # Infrastructure as Code
│   ├── terraform/         # Terraform modules
│   ├── cloudformation/    # CloudFormation templates (if applicable)
│   └── scripts/           # Deployment scripts
├── src/                   # Application code
│   ├── [language]/        # Language-specific code
│   └── tests/             # Unit and integration tests
├── configs/               # Configuration files
├── scripts/               # Lab-specific scripts
└── validation/            # Validation scripts and test results
    ├── tests/             # End-to-end tests
    └── metrics/           # Performance, cost, reliability metrics
```

### `/shared/`

Reusable components, patterns, and utilities used across multiple labs.

**Subdirectories:**
- `infrastructure/`: Reusable IaC modules (Terraform modules, CloudFormation templates)
- `scripts/`: Utility scripts for common tasks
- `configs/`: Shared configuration templates
- `patterns/`: Code patterns and examples (security, reliability, cost optimization)

### `/docs/`

Repository-wide documentation.

**Subdirectories:**
- `decisions/`: Architecture Decision Records (ADRs) that apply across labs
- `patterns/`: Design patterns and best practices
- `security/`: Security guidelines, threat modeling templates, compliance docs
- `cost-analysis/`: Cost analysis methodologies and templates

### `/tools/`

Development, testing, and analysis tools.

**Subdirectories:**
- `lint/`: Linting configurations (ESLint, Pylint, etc.)
- `test/`: Test utilities and frameworks
- `analysis/`: Tools for cost analysis, security scanning, reliability testing

### `/.github/`

GitHub-specific configurations.

**Contents:**
- `workflows/`: GitHub Actions workflows
- `ISSUE_TEMPLATE/`: Issue templates for bugs, features, labs
- `PULL_REQUEST_TEMPLATE.md`: PR template

## Naming Conventions

- **Labs**: `kebab-case` (e.g., `multi-region-failover`, `cost-optimization-patterns`)
- **Files**: `kebab-case` for docs, `PascalCase` for classes, `camelCase` for functions
- **ADRs**: `NNNN-short-description.md` (e.g., `0001-use-terraform-for-iac.md`)

## Decision Documentation

All significant decisions are documented using Architecture Decision Records (ADRs):

1. **Context**: What is the issue we're addressing?
2. **Decision**: What is the decision we're making?
3. **Status**: Proposed, Accepted, Deprecated, Superseded
4. **Consequences**: What are the tradeoffs? Security, reliability, cost, maintainability impacts

## Lab Lifecycle

1. **Proposal**: Create issue using lab proposal template
2. **Planning**: Document problem, alternatives, decision
3. **Implementation**: Build with tests, documentation, validation
4. **Review**: Security, cost, reliability review
5. **Documentation**: Complete ADRs, tradeoffs, lessons learned
6. **Maintenance**: Keep updated, deprecate if superseded

