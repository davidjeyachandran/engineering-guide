# Technical Guidelines

## Tech stack policy

Adopt a limited set of preferred stacks to improve portability, supportability, and shared tooling leverage.

- Preferred: default choices for most new systems
- Contextual: acceptable alternatives when team constraints justify them
- Legacy: existing stack choices being maintained or migrated over time

## Architecture

- Prefer modular boundaries with clear interfaces
- Keep implementation details private to modules
- Design APIs around use cases, not internal data models
- Reuse established architecture patterns before inventing new ones

## Quality

- Use static analysis and formatting tools in CI
- Write tests at appropriate levels: unit, integration, end-to-end
- Keep tests deterministic and fast where possible
- Include peer review and passing CI before merge whenever possible

## Documentation

- Treat docs as first-class artifacts
- Capture intent, constraints, and trade-offs
- Update docs with behavior changes

### Documentation standard for shared components

If a service, API, or library is intended for reuse, include:

- An overview and intended use cases
- Reference documentation
- Integration guide with examples
- Ownership and support expectations

Use a third-party-first mindset so internal consumers can adopt with minimal synchronous support.

## Security baseline

- Include security considerations in design and code review
- Use automated scanning in CI and triage findings quickly
- Provide secure coding guidance and training pathways
- Use threat modeling for higher-risk projects

## Accessibility baseline

- Include accessibility in definition of done
- Test accessibility for critical user workflows
- Track accessibility gaps and prioritize remediation

## Open-source usage

- Define approved license and dependency policies
- Track dependency provenance and vulnerability exposure
- Clarify contribution and maintenance expectations for upstream projects

## Reliability and operability

- Emit useful logs and metrics
- Fail loudly and clearly when assumptions break
- Include runbooks for critical operational flows
