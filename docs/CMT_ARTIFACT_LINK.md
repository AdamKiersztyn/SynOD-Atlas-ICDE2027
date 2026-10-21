# Frozen artifact — final CMT supplementary-material link

**Status: Published and validated, 21 October 2026.**

- Tagged release: [icde2027-v1.4a](https://github.com/AdamKiersztyn/SynOD-Atlas-ICDE2027/releases/tag/icde2027-v1.4a)
- Direct binary asset: [SynOD-Atlas-ICDE2027_VERIFIED_ARTIFACT_v1.4a.zip](https://github.com/AdamKiersztyn/SynOD-Atlas-ICDE2027/releases/download/icde2027-v1.4a/SynOD-Atlas-ICDE2027_VERIFIED_ARTIFACT_v1.4a.zip)
- Archive size: 3,501,637 bytes
- SHA-256: `76f072db5effd157121f031d88a9de640b11d245de9cd5a1dae1b952607502ee`
- Frozen commit/tag target: `aca4c342f1141519d595f504a993e604afb400d1`
- Release publication workflow: [completed successfully](https://github.com/AdamKiersztyn/SynOD-Atlas-ICDE2027/actions/runs/39670175761)
- Analytical reproduction workflow: [completed successfully](https://github.com/AdamKiersztyn/SynOD-Atlas-ICDE2027/actions/runs/39609831518)

**What was tested:** integrity of 2,100 synthetic tasks and 27,300 frozen run records (13 detectors), 65 deterministic smoke cases, the relational Failure Cube, internal SHA-256 files, and matching 32 reproduced derived tables. The release job also independently downloaded the release asset and checked its full-file checksum.

**Boundaries of these checks:** this validation is based on frozen source/results and a sample of re-executions; all 27,300 historical model evaluations were not independently rerun from zero in a separate environment. Some external source-data and preprocessing lineage is incomplete for the 31 × 24 panel. Synthetic-to-real exact geometric transfer was not supported by the reported statistical tests. These limitations must remain explicit in the manuscript.

## Suggested CMT supplementary-material text

Public artifact (versioned GitHub release): https://github.com/AdamKiersztyn/SynOD-Atlas-ICDE2027/releases/tag/icde2027-v1.4a

The frozen release contains versioned generator/detector code, result tables, supplementary audits, a queryable Failure Cube and reproduction scripts. GitHub Actions verified archive checksums, integrity, 65 smoke cases and 32 derived tables (separate workflow). Reproduction of analyses from frozen results is supported; not all original detector executions were rerun afresh. Real-data source provenance limitations are documented.
