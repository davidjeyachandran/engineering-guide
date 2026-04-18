# Codebase Structure and Feature Delivery

## Structure goals

A clear structure improves discoverability, onboarding, and ownership.

## Suggested layout

- `apps/` for deployable applications
- `packages/` for shared libraries and tooling
- `docs/` for architecture and process references
- `scripts/` for automation tasks

## Module boundaries

- Keep domain logic separate from framework adapters
- Restrict cross-module imports to public entry points
- Encapsulate implementation details behind small interfaces

## Feature delivery workflow

1. Clarify the behavior change and scope
2. Identify impacted modules and contracts
3. Implement behind clear boundaries
4. Add or update tests closest to affected behavior
5. Validate non-functional requirements (performance, security, accessibility)
6. Ship incrementally when possible

## Controlled deployments

### What it is

Controlled deployment means introducing changes progressively while monitoring key indicators and limiting blast radius.

### Why this exists

Progressive delivery reduces customer impact when problems occur and improves confidence in change safety.

### How it is used

- Prefer canary or progressive rollout for non-trivial changes
- Use preproduction environments that closely resemble production
- Use blue-green deployment when fast rollback is critical
- Monitor service health and customer-impact metrics during rollout

## Data schema change safety

Avoid tightly coupling schema changes and behavior changes in a single irreversible step.

- Deploy code that supports old and new schema states
- Deploy schema change after compatibility code is live
- Enable behavior changes only after schema rollout is complete
- Remove obsolete compatibility code in a follow-up change

## Feature flag governance

Use feature flags for staged delivery and safer rollback.

- Create flags during planning, not at the last minute
- Associate each flag with owner, success metrics, and expiry plan
- Roll out incrementally and monitor impact
- Remove stale flags and dead paths after full rollout

## Scaling guidance

- Start with conventions, then automate enforcement
- Revisit boundaries when ownership or complexity changes
- Decompose large modules before they become bottlenecks
