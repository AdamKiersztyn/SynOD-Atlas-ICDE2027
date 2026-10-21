# SynOD-Atlas — ICDE 2027 reproducibility artifact

**Artifact status: IN PREPARATION — not yet a reproducible public release.**

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

The frozen release ZIP has been assembled from the final v1.4a package and passed local integrity, 65 smoke checks, and comparison of 32 reproduced result tables. **The ZIP still needs to be uploaded to a GitHub Release by the repository owner; this GitHub connector cannot attach a binary release asset.**

- [Local verification report](docs/LOCAL_AUDIT_2026-10-21.md)
- [How to publish the prepared ZIP](docs/UPLOAD_RELEASE_ASSET.md)
- [Release verification workflow](.github/workflows/verify-release.yml)

## Contents planned for the audited release

The following materials **have not yet been verified as present in this repository**:

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

**Not available yet.** Reproduction commands and claimed pass/fail results will be provided only after the frozen code, exact inputs, and run instructions are uploaded and verified.

## Scope and provenance

The real-data evaluation does **not** demonstrate exact synthetic-to-real geometric transfer. Its source-level preprocessing lineage is not fully recoverable for every dataset. The release must accurately preserve this limitation.

## Citation and manuscript

Manuscript title: *From Aggregate Scores to Competence Geometry in Unsupervised Outlier Detection*. The category prefix required by the venue is handled separately in submission metadata.

**Do not cite this repository as a completed reproduction artifact until a frozen, independently checked release exists.**

## Contact

Adam Kiersztyn — Lublin University of Technology.
