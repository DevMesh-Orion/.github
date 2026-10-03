# Security Policy

Security is an important part of DevMesh-Orion.

This document describes how security vulnerabilities should be reported and the general security principles used across the organization.

## Reporting a Vulnerability

Do not report security vulnerabilities through public GitHub Issues.

If you discover a potential security vulnerability, use GitHub's private vulnerability reporting or security advisory functionality when available.

If private reporting is not available for the affected repository, contact the repository owner privately.

## Please Do Not Publicly Disclose

Do not publicly disclose:

- passwords
- API keys
- authentication tokens
- session tokens
- private certificates
- database credentials
- personally identifiable information
- exploitable vulnerability details

until the issue has been investigated and an appropriate disclosure decision has been made.

## Examples of Security Issues

Examples include:

- authentication bypass
- authorization bypass
- SQL injection
- cross-site scripting
- cross-site request forgery
- insecure direct object references
- sensitive information exposure
- credential leakage
- insecure file handling
- dependency vulnerabilities
- server-side request forgery
- privilege escalation

## Security Principles

Projects in this organization should follow security principles including:

- least privilege
- defense in depth
- secure defaults
- input validation
- output encoding
- secure authentication
- secure authorization
- protection of secrets
- data minimization
- appropriate logging
- dependency management
- regular security testing

## Secrets

Secrets must never be committed to source control.

Use appropriate secret-management mechanisms for:

- local development
- CI/CD
- staging
- production

Examples include environment variables, development secret stores, GitHub Actions secrets, and deployment-platform secret stores.

## Authentication

Authentication systems should:

- store password hashes rather than plaintext passwords
- use secure password policies
- protect authentication endpoints from abuse
- use secure session and token handling
- implement appropriate account verification
- provide account recovery mechanisms where applicable

## Logging

Logs must not contain sensitive information such as:

- passwords
- access tokens
- session cookies
- authentication codes
- unnecessary personal information

## Dependencies

Dependencies should be monitored for known vulnerabilities.

Security updates should be applied according to their severity and impact.

## Responsible Disclosure

Security reports will be evaluated and handled in good faith.

Where appropriate, fixes and security advisories may be published after remediation.