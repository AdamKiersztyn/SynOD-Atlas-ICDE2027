# ICDE 2027 — public artifact release checklist

This checklist refers to the final 13-detector audited evaluation (2,100 tasks and 27,300 runs). Earlier experiment snapshots are **not** interchangeable with the final paper.

## Required files and checks

- [ ] Publish complete, reviewed generator v1.4 lineage, extension v2.1, and audited detector wrappers v2.1a.
- [ ] Publish full synthetic task manifest: exactly 2,100 unique tasks.
- [ ] Publish exactly 27,300 frozen core detector executions, 13 per task, with matching identifiers.
- [ ] Publish sample-size audit results (6,552 executions).
- [ ] Publish hyperparameter-sensitivity results (1,008 executions).
- [ ] Include the queryable Failure Cube, schema, SQL integrity constraints, and reproducible canonical queries Q1–Q5.
- [ ] Publish figure- and table-producing scripts, including the complete claim-to-inputs manifest.
- [ ] Include 31 × 24 real-data detector profiles with dataset provenance and clear licensing/redistribution boundaries.
- [ ] Pin Python and third-party dependency versions; specify operating environment and expected runtime/storage.
- [ ] Audit private paths, credentials, temporary logs, license compliance, and dataset redistribution permissions.
- [ ] Generate and verify SHA-256 checksums for released files.
- [ ] Run an end-to-end *clean environment* reproduction, compare all manuscript tables/figures, and retain machine-readable checks and logs.
- [ ] Verify anonymous access to repository and release artifacts.
- [ ] Tag a frozen GitHub release only after a successful integrity and reproduction audit.
- [ ] Put the exact frozen release URL/DOI and commit SHA into submission supplementary-material metadata.
- [ ] Reconcile the manuscript artifact-availability claim with the actual public release.

## Scientific integrity and scope

- The controlled dataset count is 2,100; the primary execution count is 27,300, **not** 16,800 or 29,400.
- The PCA wrapper correction must be present in the released stream.
- The synthetic-to-real exact transfer test was negative; do not assert it succeeded.
- Expose any missing upstream lineage for the 31-dataset external panel.
- Do not claim that a public artifact is fully reproducible merely because the repository URL exists.

## Submission status

**Repository established; artifact release pending.** Do not mark the Experiment, Analysis, and Benchmark artifact requirement as fulfilled until all mandatory components above have been uploaded and independently checked.
