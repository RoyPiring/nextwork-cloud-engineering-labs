# Cloud Engineering Systems

Decision-first cloud engineering systems with validated implementations, documented tradeoffs, and curated feature projects derived from repeated hands-on work.

## Philosophy

This repository follows a **decision-first** approach where every implementation is preceded by:
- **Problem statement** and context
- **Decision records** (ADRs) documenting tradeoffs
- **Validated implementations** with production-ready patterns
- **Cost analysis** and guardrails
- **Security considerations** and threat modeling
- **Reliability patterns** and failure modes

## Repository Structure

```
.
├── README.md                 # This file
├── CONTRIBUTING.md           # Contribution guidelines
├── STRUCTURE.md             # Detailed structure documentation
├── .github/                  # GitHub workflows and templates
│   ├── workflows/
│   │   ├── ci.yml           # Continuous integration
│   │   ├── security-scan.yml # Security scanning
│   │   └── cost-analysis.yml # Cost analysis automation
│   └── ISSUE_TEMPLATE/      # Issue templates
├── labs/                     # Individual lab projects
│   ├── _template/           # Lab template for new projects
│   └── [lab-name]/          # Individual lab directories
├── shared/                   # Shared utilities and patterns
│   ├── infrastructure/      # IaC templates and modules
│   ├── scripts/             # Utility scripts
│   ├── configs/             # Shared configurations
│   └── patterns/            # Reusable code patterns
├── docs/                     # Documentation
│   ├── decisions/           # Architecture Decision Records (ADRs)
│   ├── patterns/            # Design patterns documentation
│   ├── security/            # Security guidelines and threat models
│   └── cost-analysis/       # Cost analysis templates and examples
└── tools/                    # Development and analysis tools
    ├── lint/                # Linting configurations
    ├── test/                # Test utilities
    └── analysis/            # Cost, security, reliability analysis tools
```

## Labs

Each lab follows a consistent structure:

- **Problem & Context**: What problem are we solving?
- **Decision Record**: Why this approach? What alternatives were considered?
- **Implementation**: Production-ready code with tests
- **Tradeoffs**: Security, reliability, cost, maintainability analysis
- **Validation**: How was this validated? What metrics?
- **Lessons Learned**: What would we do differently?

### Available Labs

*Labs will be listed here as they are added*

## Getting Started

1. Review [STRUCTURE.md](./STRUCTURE.md) for detailed organization
2. Read [CONTRIBUTING.md](./CONTRIBUTING.md) for contribution guidelines
3. Explore existing labs in the `labs/` directory
4. Use `labs/_template/` as a starting point for new labs

## Operating Standards

All implementations follow these principles:

- **Security-first**: Least privilege, threat modeling, encryption, auditability, safe defaults
- **Reliability-first**: Failure modes, retries/timeouts, idempotency, rollback paths, SLO-aware choices
- **Cost-aware**: Right-size, avoid unbounded spend, explain cost drivers and guardrails
- **Maintainability**: Clean interfaces, tests, linting, docs, predictable repo structure

## License

[Specify license]
