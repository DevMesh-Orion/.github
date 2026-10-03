# Contributing to DevMesh-Orion

Thank you for contributing to DevMesh-Orion.

This document describes the general development workflow and contribution standards used across the organization's repositories.

## Development Workflow

Development work should be associated with a Jira issue whenever practical.

The general workflow is:

Jira issue
→ Git branch
→ Commits
→ Pull Request
→ CI checks
→ Review
→ Merge
→ Deployment

## Branches

The `main` branch represents the stable branch.

Do not push directly to `main` unless explicitly required for repository administration.

Recommended branch naming:

- `feature/PORT-123-short-description`
- `fix/PORT-123-short-description`
- `refactor/PORT-123-short-description`
- `chore/PORT-123-short-description`
- `docs/PORT-123-short-description`
- `security/PORT-123-short-description`

Replace `PORT-123` with the relevant Jira issue key.

## Commits

Write clear and meaningful commit messages.

Prefer:

`Add email verification flow`

over:

`changes`

When practical, include the Jira issue key:

`PORT-123 Add email verification flow`

Never commit:

- passwords
- API keys
- tokens
- private certificates
- database credentials
- personal data
- production secrets

## Pull Requests

Pull Requests should:

- have a clear title
- reference the relevant Jira issue
- explain what changed
- explain why the change was required
- include appropriate tests
- document relevant security considerations
- document breaking changes

Keep Pull Requests focused.

Avoid combining unrelated changes into one Pull Request.

## Testing

Changes should be tested before opening a Pull Request.

Depending on the project, this may include:

- unit tests
- integration tests
- API tests
- frontend tests
- end-to-end tests
- security tests

All required CI checks must pass before merging.

## Code Quality

Code should follow the conventions defined by the individual repository.

For .NET projects this generally includes:

- consistent formatting
- nullable reference types
- appropriate dependency injection
- asynchronous APIs where appropriate
- meaningful naming
- separation of concerns
- automated testing

For Vue and TypeScript projects this generally includes:

- TypeScript
- strict typing
- consistent formatting
- component separation
- reusable composables where appropriate
- automated testing

## Security

Security is considered part of the development process.

Never commit secrets or sensitive information.

Security vulnerabilities should not be reported through normal public issues.

See `SECURITY.md` for the security reporting process.

## Dependencies

Dependencies should be kept reasonably up to date.

Security updates should be prioritized.

Automated dependency update tools may be used where configured.

## Documentation

Changes that affect public behavior, APIs, configuration, architecture, or development workflows should update the relevant documentation.

## Code Review

Reviewers should consider:

- correctness
- maintainability
- security
- performance
- testing
- backwards compatibility
- documentation

Feedback should be constructive and specific.

## Licensing

Individual repositories may contain their own license and licensing requirements.

Follow the license and contribution requirements of the repository you are contributing to.