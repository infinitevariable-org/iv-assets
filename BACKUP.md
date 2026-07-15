# Backup Policy — iv-assets
Infinite Variable Pvt Ltd (CIN U74140PN2020PTC192821).

- **Scope:** Binary assets + git history are the durable record; mirrored on GitHub and in off-box backups.
- **Off-box:** backups are stored off the primary host, encrypted at rest.
- **Cadence:** daily, encrypted, off-site.
- **Retention:** TODO: confirm.
- **Verification:** periodic test-restore (ISO 27001 A.12.3) — restore-and-verify is a standing practice, not an assumption.

See DISASTER_RECOVERY.md for RTO/RPO and failover.
