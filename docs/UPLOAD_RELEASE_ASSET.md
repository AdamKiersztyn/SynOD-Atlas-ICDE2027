# Publish the prepared reproducibility archive

**Prepared file**: `SynOD-Atlas-ICDE2027_VERIFIED_ARTIFACT_v1.4a.zip` (3,501,637 bytes).

1. Obtain the prepared ZIP from ChatGPT.
2. Open [New GitHub Release](https://github.com/AdamKiersztyn/SynOD-Atlas-ICDE2027/releases/new).
3. Choose **Create new tag** `icde2027-v1.4a`, targeting branch `main`.
4. Set release title **ICDE 2027 — audited benchmark artifact v1.4a**.
5. Drag the ZIP into **Attach binaries by dropping them here or selecting them**.
6. Paste the notes from [Local audit](LOCAL_AUDIT_2026-10-21.md) or briefly explain the frozen inputs and the reproduction boundary.
7. Click **Publish release** only after the ZIP has finished uploading.
8. Verify [GitHub Actions](https://github.com/AdamKiersztyn/SynOD-Atlas-ICDE2027/actions) completes successfully. The workflow is triggered by publishing a release.
9. Download the ZIP again using a private/incognito browser and check the archive SHA-256: `76f072db5effd157121f031d88a9de640b11d245de9cd5a1dae1b952607502ee`.
10. In CMT, link the exact release page and record the immutable release commit SHA.

**Warning:** the public repository page without the ZIP does not meet full reproducibility requirements. Do not use the old 16,800-run archive.
