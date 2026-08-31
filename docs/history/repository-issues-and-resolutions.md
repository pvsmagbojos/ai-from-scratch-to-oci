# Repository Issues and Resolutions

This is the canonical append-only troubleshooting history for problems encountered while maintaining the reusable course repository on `main`.

Learner-specific errors belong in `docs/progress/issues-and-resolutions.md` on that learner's `progress/<learner>` branch.

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
