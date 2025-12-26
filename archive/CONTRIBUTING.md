# Contributing Guidelines

## Process

Following our decision-first approach, all contributions should:

1. **Restate the goal** in 1–2 lines and list assumptions
2. **Propose an implementation plan** (steps + files to touch)
3. **Implement** with production patterns (typing, errors, logging, config)
4. **Add or adjust tests** and provide run commands
5. **End with a verification checklist** and risks

## Code Standards

### Security-First
- Least privilege: Minimal IAM permissions, network isolation
- Threat modeling: Document threats and mitigations
- Encryption: Encrypt data at rest and in transit
- Auditability: Comprehensive logging and monitoring
- Safe defaults: Secure by default configurations

### Reliability-First
- Failure modes: Document and handle failure scenarios
- Retries/timeouts: Implement with exponential backoff
- Idempotency: Operations must be safely retryable
- Rollback paths: Document and test rollback procedures
- SLO-aware: Design with service level objectives in mind

### Cost-Aware
- Right-size: Use appropriate resource sizes
- Avoid unbounded spend: Set limits and alerts
- Explain cost drivers: Document cost implications
- Guardrails: Implement cost controls

### Maintainability
- Clean interfaces: Well-defined APIs and contracts
- Tests: Unit, integration, and end-to-end tests
- Linting: Follow language-specific linting rules
- Documentation: Clear, up-to-date documentation
- Predictable structure: Follow repository conventions

## Pull Request Process

1. Create a feature branch from `main`
2. Follow the lab structure template if creating a new lab
3. Document decisions in ADRs
4. Include tests with adequate coverage
5. Update documentation
6. Run linting and tests locally
7. Create PR with:
   - Clear description of changes
   - Link to related issues/ADRs
   - Verification checklist
   - Risk assessment

## Lab Creation Checklist

When creating a new lab:

- [ ] Problem statement documented
- [ ] ADR created with alternatives considered
- [ ] Implementation with production patterns
- [ ] Security threat model documented
- [ ] Cost analysis completed
- [ ] Reliability patterns implemented
- [ ] Tests written and passing
- [ ] Documentation complete
- [ ] Tradeoffs documented
- [ ] Validation results included

## Questions?

Open an issue with the `question` label.

