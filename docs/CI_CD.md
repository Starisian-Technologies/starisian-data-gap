# CI/CD

## Build workflow
`.github/workflows/build.yml` validates:
- dependency install (`npm ci`)
- JS/CSS build (`npm run build`)
- PHPUnit tests (`npm test`)
- PHP syntax lint for plugin bootstrap

## Release workflow
`.github/workflows/release.yml` runs on semver tags `vX.Y.Z` and:
- derives version from tag
- updates version strings
- builds production assets
- packages plugin zip
- publishes GitHub release with SHA-256 checksum
