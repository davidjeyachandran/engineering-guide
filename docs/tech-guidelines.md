# Technical Guidelines

## Architecture

- Prefer modular boundaries with clear interfaces
- Keep implementation details private to modules
- Design APIs around use cases, not internal data models

## Quality

- Use static analysis and formatting tools in CI
- Write tests at appropriate levels: unit, integration, end-to-end
- Keep tests deterministic and fast where possible

## Documentation

- Treat docs as first-class artifacts
- Capture intent, constraints, and trade-offs
- Update docs with behavior changes

## Reliability and operability

- Emit useful logs and metrics
- Fail loudly and clearly when assumptions break
- Include runbooks for critical operational flows
