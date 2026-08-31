# Repository Issues and Resolutions

Use this append-only log for problems encountered while maintaining the reusable course repository on `main`.

Keep personal course errors in `docs/progress/issues-and-resolutions.md` on your `progress/<learner>` branch.

## Status Values

- `Open` — investigation or resolution is still required.
- `Resolved` — a resolution was implemented and verified.
- `Deferred` — intentionally postponed; record why and what would allow work to resume.

## Repository Issue Entry Template

### REPO-ISSUE-0000 — Short descriptive title

- Date:
- Status: Open | Resolved | Deferred
- Repository area:
- Affected files/commands:

#### Symptom / Error

Record the observable behavior or useful error text. Redact secrets and sensitive values.

#### Context / Reproduction

Record what was being attempted and the smallest reliable reproduction steps when applicable.

#### Investigation / Attempts

Record only meaningful attempts that narrowed the problem or produced a reusable lesson.

#### Root Cause

Record the evidence-supported root cause. Use `Unknown` if it has not been established. Distinguish a workaround from a root-cause fix.

#### Resolution

Record the exact corrective steps or workaround.

#### Verification

Record how the fix was tested and the result.

#### Maintenance Takeaway

Record the reusable repository-maintenance lesson.

#### References

Record sources used specifically for diagnosis/resolution when applicable.

---

## Recorded Issues

### REPO-ISSUE-0001 — Repository tree generator command unavailable

- Date: 2026-08-31
- Status: Resolved
- Repository area: Initial course scaffold and standards
- Affected files/commands: `docs/standards/repository-tree.md`; attempted `tree` shell command

#### Symptom / Error

The repository-tree regeneration step could not use the intended shell utility because the `tree` command was unavailable in the generation environment. The process reported `tree command unavailable`.

#### Context / Reproduction

While updating repository standards, the repository tree snapshot needed to be regenerated. The generation command first checked for the `tree` executable and found that it was not installed/available.

#### Investigation / Attempts

The shell step explicitly checked `command -v tree`. The check failed, confirming that relying on the external CLI would make the documentation-generation step environment-dependent.

#### Root Cause

The `tree` command-line utility was not available in the execution environment. The repository itself does not require `tree`; it was only a documentation-generation convenience.

#### Resolution

Replaced the external `tree` dependency with a small Python filesystem traversal that recursively enumerates the repository and writes the snapshot to `docs/standards/repository-tree.md`.

#### Verification

Verified that the regenerated tree exists and includes the expected repository structure.

#### Maintenance Takeaway

Do not introduce an undocumented external CLI dependency for repository maintenance when the same task can be performed with tooling already guaranteed by the environment. If a convenience command is unavailable, document the failure and use a reproducible fallback.

#### References

None required.

### REPO-ISSUE-0002 — Duplicate setup-guide section number during documentation update

- Date: 2026-08-31
- Status: Resolved
- Repository area: AI tutor onboarding documentation
- Affected files/commands: `docs/setup/initial-repository-setup.md`; automated Markdown section insertion/renumbering

#### Symptom / Error

Validation showed two `## 5.` headings in `initial-repository-setup.md`: the newly added AI tutor repository-context section and the existing course-update section.

#### Context / Reproduction

The direct-repository-reading instructions were inserted before the existing section 4, after which an automated renumbering pass shifted the existing headings. The same replacement also shifted the newly inserted section number.

#### Investigation / Attempts

A heading-only validation using `grep -n '^## '` made the duplicate numbering visible immediately after the edit.

#### Root Cause

The section-number replacement was applied to the whole file after inserting the new section, so the new `## 4.` heading was unintentionally included in the `4 -> 5` renumbering operation.

#### Resolution

Corrected the AI tutor repository-context heading to `## 4.` and retained the existing course-update section as `## 5.`.

#### Verification

Re-ran the heading listing and confirmed a single sequential section series from 1 through 10, followed by References.

#### Maintenance Takeaway

When programmatically inserting numbered Markdown sections, validate heading order after transformation and avoid global renumbering that can mutate newly inserted headings.

#### References

None required.


### REPO-ISSUE-0003 — Terminology validation covered only a partial update tree

- Date: 2026-08-31
- Status: Resolved
- Repository area: Documentation terminology and validation
- Affected files/commands: Full Markdown documentation tree; previous terminology-update validation

#### Symptom / Error

After rebuilding the complete repository from the starter plus subsequent update bundles, a full-tree search found remaining uses of terminology that had previously been reported as fully removed.

#### Context / Reproduction

The earlier terminology update was validated against a working directory that contained only the files included in the recent update bundle. It did not contain every Markdown file from the full starter repository. Reconstructing the complete repository and running a repository-wide search exposed the missed occurrences.

#### Investigation / Attempts

The full starter archive was extracted, the direct-repository-access update and terminology update were layered on top in order, and all Markdown files were searched rather than only the recently changed subset.

#### Root Cause

The earlier validation target was incomplete. A partial update tree was mistaken for the full repository, so the zero-match result did not prove that the entire repository had been updated.

#### Resolution

Rebuilt the latest full repository, applied the terminology change across the complete Markdown tree, and changed validation to scan the reconstructed full repository.

#### Verification

Ran a full-tree case-insensitive search across every Markdown file and confirmed that the rejected terminology no longer appears.

#### Maintenance Takeaway

When an update is distributed as a partial patch archive, do not use that patch directory as proof of repository-wide state. Reconstruct or inspect the complete repository before making global validation claims.

#### References

None required.

### REPO-ISSUE-0004 — Documentation patch packaging lost relative paths

- Date: 2026-08-31
- Status: Resolved
- Repository area: Documentation update packaging
- Affected files/commands: Changed-file diff and patch-archive generation script

#### Symptom / Error

The patch packaging step failed with `cp: cannot stat` for a changed documentation file because the generated changed-file list contained only basenames such as `ai-tutor-master-prompt.md` instead of repository-relative paths such as `docs/prompts/ai-tutor-master-prompt.md`.

#### Context / Reproduction

A shell `diff -qr` result was post-processed with `sed` to derive changed paths. The expression captured only the final path component, which was ambiguous for repeated filenames such as `README.md` and incorrect for every nested file.

#### Investigation / Attempts

The failed copy path showed that directory information had been discarded. The changed-file list also contained several identical `README.md` entries, confirming that basenames were insufficient.

#### Root Cause

The shell path-extraction expression reduced full paths to basenames rather than preserving repository-relative paths.

#### Resolution

Replaced the shell path extraction with a Python comparison that walks both repository trees, compares matching files by relative path, and emits the exact repository-relative path for each changed file.

#### Verification

Rebuilt the patch archive from the corrected relative-path list and validated the resulting ZIP archive with `ZipFile.testzip()`.

#### Maintenance Takeaway

When packaging repository patches, preserve full repository-relative paths. Basename-only file lists are unsafe because common names such as `README.md` appear in many directories.

#### References

None required.

### REPO-ISSUE-0005 — Release version changed without updating current-version documentation

- Date: 2026-08-31
- Status: Resolved
- Repository area: Release/version documentation
- Affected files: `README.md`, `docs/progress/current-learning-status.md`, `docs/setup/initial-repository-setup.md`, `docs/standards/repository-structure-standard.md`, `docs/history/repository-change-log.md`

#### Symptom / Error

After `v0.2.0` was selected as the next shared course release, several documents still described `v0.1.0` as the intended or current starting version.

#### Context / Reproduction

The instructional-style documentation bundle was generated before the `v0.2.0` release recommendation was made. The Git instructions were updated in conversation, but the repository files were not revised in the same step.

#### Investigation / Attempts

Searched the complete repository for `v0.1.0` and `v0.2.0`, then reviewed each match to distinguish historical references from references that meant the current/recommended release.

#### Root Cause

The release-version decision happened after the documentation bundle had already been produced, and the follow-up release instructions did not include a documentation synchronization step.

#### Resolution

Kept `v0.1.0` wherever it refers to the historical first public baseline, added `v0.2.0` as the current shared course release, and updated setup/status/branching guidance so new progress branches start from the current release.

#### Verification

Re-scanned all release-version references and confirmed that `v0.1.0` is now used only for the original historical baseline while `v0.2.0` is identified as the current recommended release where appropriate.

#### Maintenance Takeaway

Whenever a new release tag is introduced, update the release references in documentation and the repository change history in the same change before publishing the tag.

#### References

None required.
