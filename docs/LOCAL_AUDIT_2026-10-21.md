# Local artifact audit — 21 October 2026

**Result: PASS for integrity, frozen-data analysis reproduction, and smoke verification. Public release: NOT YET UPLOADED.**

Artifact bundle prepared from the **6 October 2026 v1.4a final audit package**.

## Verified facts

| Criterion | Actual result |
| --- | --- |
| Synthetic benchmark tasks | 2,100 |
| Methods/detectors | 13 |
| Frozen core runs | 27,300 |
| Sample-size audit | 6,552 |
| Hyperparameter audit | 1,008 |
| External derived profiles | 31 × 24 |
| Failure Cube database integrity | PASS |
| Canonical query result row counts (Q1–Q5) | 60, 10, 255, 0, 130 |
| Reproduced CSV tables | **32 matched** |
| Generator/score smoke checks | **65 PASS** |
| Maximum difference for AUC/AP/q | 1.110223 × 10^-16 |
| Package internal SHA-256 manifest | PASS |

## Intended release asset

- Filename: `SynOD-Atlas-ICDE2027_VERIFIED_ARTIFACT_v1.4a.zip`
- Archive size: **3,501,637 bytes**
- Archive SHA-256: `76f072db5effd157121f031d88a9de640b11d245de9cd5a1dae1b952607502ee`
- Package files: 102 including `SHA256SUMS.txt`
- Old `.pyc` and `__pycache__` files were stripped from the release package.

This checked artifact ZIP is provided to the repository owner through ChatGPT. **It is not yet available in this GitHub repository.**

## What this audit does not establish

The **27,300 original detector executions were not all rerun** in the current environment; the reproduction regenerated analyses and outputs from frozen metrics and compared 32 derived tables. A fully independent fresh-machine verification and public-download accessibility check will follow asset upload. External original-data provenance is incomplete for some of the 31 tasks and that limitation must be retained.

## To finalize

1. Upload the exact ZIP as an asset to the GitHub release with tag `icde2027-v1.4a`.
2. Publish the release (the workflow in `.github/workflows/verify-release.yml` will then check the asset).
3. Check the public asset URL logged out and record the release tag, commit SHA, and verification result in CMT supplementary material.

Do not claim completion of the ICDE EAB artifact requirement until the public asset is accessible and checked.
