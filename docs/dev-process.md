# Development Process

## Operating model

Teams should plan and execute work with two complementary commitments:

- Outcome commitments (objectives and key results)
- Reliability commitments (service level objectives and support obligations)

Balancing both prevents short-term feature pressure from eroding long-term product health.

## Decision framework

Use explicit decision paths based on scope and risk:

- Small, reversible decisions can be made directly by the owning team
- Cross-team or high-impact changes should be documented in an RFC
- Complex, multi-stakeholder decisions should identify one accountable decision owner

For non-trivial decisions, record context, options considered, trade-offs, and final rationale.

You can adapt [RFC Template](templates/rfc-template.md).

## Lifecycle

1. Define problem and success criteria
2. Align on approach and risks
3. Implement in small, reviewable increments
4. Validate with tests and verification checks
5. Roll out and monitor outcomes
6. Document lessons learned

## Pull request standards

- Keep changes focused and scoped to one concern
- Explain user impact and technical impact
- Include test evidence for changed behavior
- Link related issues or decision notes
- Include at least one reviewer who is not the author
- Aim for passing build and test checks before merge

## Release readiness

Use a lightweight operational readiness checklist before non-trivial launches.

You can adapt [Operational Readiness Checklist Template](templates/operational-readiness-checklist.md).

## Operational readiness checklist

- Capacity and performance expectations are defined
- Logging, metrics, and alerts are in place
- Rollback and mitigation paths are tested
- Ownership and support paths are clear
- Security and compliance requirements are addressed where applicable

## Stakeholder awareness

Before progressive rollout of customer-facing changes:

- Notify product, support, and documentation stakeholders
- Define customer-visible impact and communication needs
- Attach key metrics to monitor release impact

## Incident follow-up

- Capture timeline and impact
- Identify contributing factors
- Define concrete prevention actions
- Keep incident analysis blameless and system-focused
- Set owners and due dates for follow-up actions

You can adapt [Post-Incident Review Template](templates/pir-template.md).
