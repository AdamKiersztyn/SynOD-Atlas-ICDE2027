# SynOD-Atlas — ICDE 2027 reproducibility artifact

**Artifact status: publicly uploaded to the main branch; automated clean-run verification is pending.**

This repository is intended to accompany the manuscript **“From Aggregate Scores to Competence Geometry in Unsupervised Outlier Detection”**, submitted under the **Experiment, Analysis, and Benchmark** category. SynOD-Atlas is the name of the benchmark, not part of the manuscript title.

## Audited experiment identity

The manuscript's October 6, 2026 audit reports:

| Component | Audited quantity |
| --- | ---: |
| Controlled synthetic tasks | 2,100 |
| Detector implementations | 13 |
| Core detector executions | 27,300 |
| Additional sample-size audit executions | 6,552 |
| Additional hyperparameter audit executions | 1,008 |
| External real-data evaluation | 31 datasets × 24 detectors |

The frozen generator lineage combines the verified v1.4 source, the v2.1 lineage-preserving extension, and the v2.1a detector execution wrappers. In particular, the final 13-detector evaluation includes the corrected PCA reconstruction rule. Superseded 8-detector/16,800-run and 14-detector versions must **not** be substituted for this release.

## Prepared and locally validated archive (21 October 2026)

The frozen release ZIP has been assembled from the final v1.4a package and passed local integrity, 65 smoke checks, and comparison of 32 reproduced result tables. **The ZIP is now available on the public `main` branch.** SHA-256: `76f072db5effd157121f031d88a9de640b11d245de9cd5a1dae1b952607502ee`. The GitHub Actions workflow verifies this branch-based archive on push and on manual dispatch. A tagged release remains desirable for an immutable archival reference.

- [Local verification report](docs/LOCAL_AUDIT_2026-10-21.md)
- [Optional immutable tagged release and verification](docs/UPLOAD_RELEASE_ASSET.md)
- [Release verification workflow](.github/workflows/verify-release.yml)

## Contents of the uploaded ZIP

The uploaded ZIP has been inspected locally and contains:

- Source code for generators, detector wrappers, and all evaluation stages, with exact dependency versions.
- Machine-readable task metadata and 27,300 frozen core results.
- Sample-size (6,552 runs) and hyperparameter (1,008 runs) audits.
- A queryable Failure Cube database, schema, and canonical SQL queries.
- Derived analysis scripts and instructions to regenerate every reported table and figure.
- The external 31 × 24 evaluation matrix and a precise statement of source-data provenance and redistribution restrictions.
- Integrity verification scripts, SHA-256 manifest, and clean-room reproduction logs.
- Third-party attribution and an appropriate redistribution license.

See [release checklist](docs/RELEASE_CHECKLIST.md) for acceptance criteria.

## Reproduction

Download [the frozen ZIP](SynOD-Atlas-ICDE2027_VERIFIED_ARTIFACT_v1.4a.zip), extract it and follow `artifact/README.md`. The repository workflow in `.github/workflows/verify-release.yml` tests the full frozen-data analysis path against 32 reference tables. This does not imply that all 27,300 detector executions have been rerun from raw synthetic datasets.

## Scope and provenance

The real-data evaluation does **not** demonstrate exact synthetic-to-real geometric transfer. Its source-level preprocessing lineage is not fully recoverable for every dataset. The release must accurately preserve this limitation.

## Citation and manuscript

Manuscript title: *From Aggregate Scores to Competence Geometry in Unsupervised Outlier Detection*. The category prefix required by the venue is handled separately in submission metadata.

A public code/data URL now exists. Confirm the GitHub Actions validation result and freeze a tag before treating it as the final supplementary submission URL.

## Contact

Adam Kiersztyn — Lublin University of Technology.
