# Rollback

## When to roll back
- release introduces production-blocking regressions
- severe runtime errors appear after upgrade

## Procedure
1. Deactivate current plugin version.
2. Reinstall prior known-good release zip.
3. Reactivate and verify shortcode rendering.
4. Capture logs, issue details, and impacted versions for follow-up remediation.
