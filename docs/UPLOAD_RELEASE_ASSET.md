# Public archive now uploaded — next release steps (optional)

The repository owner uploaded `SynOD-Atlas-ICDE2027_VERIFIED_ARTIFACT_v1.4a.zip` directly to the **main branch**. **Do not re-upload the ZIP to main.**

- [Archive on main](../SynOD-Atlas-ICDE2027_VERIFIED_ARTIFACT_v1.4a.zip)
- [Check GitHub Actions](https://github.com/AdamKiersztyn/SynOD-Atlas-ICDE2027/actions/workflows/verify-release.yml)
- Expected SHA-256: `76f072db5effd157121f031d88a9de640b11d245de9cd5a1dae1b952607502ee`
- Expected size: 3,501,637 bytes

## Verify automation

The GitHub workflow runs on changes to the archive or its own workflow definition on branch `main`. If the latest run is missing, open **Actions → Verify SynOD-Atlas reproducibility artifact → Run workflow**, choose `main`, and click **Run workflow**. The action checks the ZIP and 101 internal hashes, validates 2,100 tasks and 27,300 runs, runs 65 smoke cases, and reproduces 32 derived CSV tables. It does **not** repeat 27,300 detector executions.

## Freeze submission version

Once Actions is green, make an immutable reference without uploading the binary again:

1. [Create a new GitHub release](https://github.com/AdamKiersztyn/SynOD-Atlas-ICDE2027/releases/new).
2. Create tag `icde2027-v1.4a` on the **verified commit on main**.
3. Give it a descriptive title and note that the binary is stored in the repository tree as `SynOD-Atlas-ICDE2027_VERIFIED_ARTIFACT_v1.4a.zip`.
4. Publish the Release **without uploading another copy**. GitHub will show the tagged source archive containing the committed ZIP.
5. Check public access to the file through the tag link and use this frozen URL in CMT. If necessary, include the commit SHA and limitations of the external dataset lineage.

The document `docs/LOCAL_AUDIT_2026-10-21.md` records local test results from the source archive.
