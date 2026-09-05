# Deployment

## Release trigger
Create and push a semantic version tag:
```bash
git tag vX.Y.Z
git push origin vX.Y.Z
```

## Artifacts
Release workflow publishes:
- `sparxstar-data-gap.zip`
- `sparxstar-data-gap.zip.sha256`

## WordPress install
Upload `sparxstar-data-gap.zip` via the WordPress plugin installer and activate.
