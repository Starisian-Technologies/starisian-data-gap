# Contributing

## Scope
This repository ships the `sparxstar-data-gap` WordPress plugin and release automation.

## Prerequisites
- PHP 8.2+
- Node.js 20+
- npm 10+

## Setup
```bash
npm ci
```

## Required local checks
Run these before opening a pull request:
```bash
npm test
npm run build
php -l wp-content/plugins/sparxstar-data-gap/sparxstar-data-gap.php
```

## Pull request expectations
- Keep changes minimal and scoped to one concern.
- Include risk assessment and rollback notes.
- Update documentation when behavior, release process, or operations change.
- Do not commit generated build artifacts (`*.min.js`, `*.min.css`) unless release automation requires it.

## Security and secrets
- Do not commit secrets, credentials, or environment-specific endpoints.
- Report vulnerabilities privately per `SECURITY.md`.

## WordPress and PHP standards
- Use strict typing and namespaced PHP (`Starisian\\Sparxstar\\DataGap`).
- Escape output and sanitize input in WordPress-facing code.
- Avoid introducing global state unless unavoidable for WordPress hooks.
