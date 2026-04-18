# Engineering Guide

A reusable, product-agnostic engineering handbook template for teams that want shared standards for code quality, delivery, collaboration, and documentation.

## Who this is for

- Engineering teams building software products or platforms
- Technical leaders defining team-wide practices
- Organizations standardizing onboarding and contribution workflows

## What this template includes

- Core handbook chapters in [docs](docs)
- Contribution policies and governance for maintainers
- GitHub issue and pull request templates
- Markdown linting and formatting setup for consistent docs
- A simple CI workflow for docs quality checks

## Quick start

1. Replace placeholders:

- `<org-name>`
- `<repo-url>`
- `<security-email>`

1. Review and adapt all files in [docs](docs).

1. Install dependencies:

```bash
npm install
```

1. Run checks:

```bash
npm run lint
npm run format:check
```

## Handbook index

- [Engineering Principles](docs/engineering-principles.md)
- [Development Process](docs/dev-process.md)
- [Technical Guidelines](docs/tech-guidelines.md)
- [Codebase Structure and Feature Delivery](docs/codebase-structure-and-feature-delivery.md)
- [Onboarding](docs/onboarding.md)
- [Team Collaboration](docs/team-collaboration.md)
- [Sources](docs/sources.md)

## License

This template is provided under the MIT License. See [LICENSE](LICENSE.md).
