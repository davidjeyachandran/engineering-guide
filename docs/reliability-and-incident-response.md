# Reliability and Incident Response

## Service criticality tiers

Define service tiers so teams can align engineering effort with business impact.

- Tier 0: critical infrastructure and shared control planes
- Tier 1: customer-critical product capabilities
- Tier 2: important but non-critical capabilities
- Tier 3: internal, experimental, or low-criticality services

Tier can influence reliability targets, test depth, release safeguards, and response urgency.

## SLOs and error budgets

Each service should define measurable reliability objectives and alerts tied to user-impacting capabilities.

- Define SLO indicators and targets
- Establish alerting thresholds and response expectations
- Review error budget burn regularly
- Adjust release velocity when reliability is trending out of bounds

## On-call and escalation expectations

- Maintain clear ownership for production services
- Define primary and secondary responders where needed
- Document escalation paths and incident roles
- Keep runbooks current for common failure modes

## Incident management

### Severity model

Use a small shared set of severity levels with clear impact criteria.

### Response workflow

1. Detect and triage quickly
1. Assign an incident lead
1. Stabilize and restore service
1. Communicate status and impact clearly
1. Capture timeline and evidence for follow-up

## Post-incident review

Use blameless post-incident reviews focused on systems and process improvements.

- Document root and contributing causes
- Identify durable prevention actions
- Assign owners and due dates
- Track completion of remediation work

You can adapt [Post-Incident Review Template](templates/pir-template.md).

## Operational review cadence

- Weekly team-level review of incidents, alerts, and reliability trends
- Monthly cross-team review for recurring reliability themes
- Quarterly leadership review to rebalance product and operational investment
