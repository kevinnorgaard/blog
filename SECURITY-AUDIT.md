# Security Audit Report

Generated: 2026-08-08

## HIGH vulnerabilities requiring manual semver-major upgrades

All fixes require `npm audit fix --force` (breaking changes).

| Package | Severity | Advisory |
|---------|----------|---------|
| `image-size` | HIGH | https://github.com/advisories/GHSA-w3rx-r6r6-pgpr |
| `image-size` | HIGH | https://github.com/advisories/GHSA-5p2g-fcmc-qvqq |
| `less` | HIGH | (depends on image-size) |
| `undici` | HIGH | https://github.com/advisories/GHSA-8xcm-r25x-g524 |
| `undici` | HIGH | https://github.com/advisories/GHSA-4cwx-7wf7-3272 |
| `undici` | HIGH | https://github.com/advisories/GHSA-m8rv-5g2x-5cg5 |
| `undici` | HIGH | https://github.com/advisories/GHSA-jr45-8vmc-qm54 |
| `undici` | HIGH | https://github.com/advisories/GHSA-v3r7-h72x-cjcm |
| `@angular-devkit/build-angular` | HIGH | (depends on above) |

## Remediation

Run `npm audit fix --force` to apply breaking-change upgrades:
- `@angular-devkit/build-angular` → `22.1.3`

Verify the app builds and works correctly after upgrading.
