# Security Policy — iv-assets

## Reporting a vulnerability
Email **security@ivuniverse.com**, or raise a HITL issue on the iVPL OS Decide
surface. Do **not** open a public issue for a suspected vulnerability. We
acknowledge within **2 business days** and aim to mitigate within 30 days.

## Secrets
No secret is ever committed or logged. Credentials live in the estate credential
store — macOS Keychain locally, systemd `LoadCredential` (tmpfs, root-only) on
the VPS — never in a plaintext `.env`. Secret scanning (gitleaks) runs in CI and
pre-push; a match blocks the merge.

## Data protection
This project complies with the **India DPDP Act 2023**. Any personal data is
encrypted at rest (AES-256-GCM) and subject to defined retention and erasure
controls.

## Supported versions & patching
The latest released version receives security fixes. Dependency and
static-analysis scans run per release via `security-scan.yml`.
