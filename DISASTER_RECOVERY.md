# Disaster Recovery — iv-assets
- **RTO:** TODO: confirm  ·  **RPO:** TODO: confirm
- **Source of truth:** git history on GitHub (`infinitevariable-org/iv-assets`); a lost working copy is recovered by re-cloning.
- **Recovery:** Re-clone from GitHub; restore any large binaries from the off-box backup if history is unavailable.
- **Procedure:** restore from the latest verified backup (see BACKUP.md), redeploy from a known-good commit, re-point traffic, verify health.
- **Drills:** restore/failover exercised periodically; results logged.
