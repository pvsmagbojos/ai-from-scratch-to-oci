# Documentation Standard

## 1. Canonical-Document Rule

Each subject has one canonical document. Update that document instead of creating files such as `final`, `latest`, `v2`, `revised`, or parallel replacements.

The master roadmap remains a checklist. Do not turn it into lesson notes or a running journal.

## 2. Documentation Domains

The repository has two documentation histories because `main` is the reusable course while `progress/<learner>` contains personal learning state.

### Canonical course/repository history

Stored under `docs/history/` and maintained through `main`:

- `repository-change-log.md` — append-only history of material changes to the reusable course/repository;
- `repository-issues-and-resolutions.md` — append-only troubleshooting history for repository/course maintenance issues.

### Learner history

Stored under `docs/progress/` and changed on `progress/<learner>`:

- `current-learning-status.md` — current learner position and exact next step;
- `learning-log.md` — append-only chronological record of material learning actions;
- `issues-and-resolutions.md` — append-only troubleshooting record for learner errors, failed attempts, misconceptions, diagnoses, fixes, and verification.

Do not record routine personal learning history in the repository-maintenance files. Do not record canonical course-maintenance work only in a learner's progress log.

## 3. Other Documentation Types

### Roadmap
Tracks required learning scope and completion only.

### Topic `README.md`
Tracks the topic's local checklist, prerequisites, status, exercises, completion evidence, and relevant learner issue references.

### `notes.md`
Contains durable explanations and learner-facing notes worth reviewing later. Keep notes organized by concept rather than by chat transcript.

### `references.md`
Records sources actually used. Prefer primary/official documentation. For changing services, include the access date and relevant version/region when known.

### Project `README.md`
Explains the problem, requirements, setup, execution, evaluation, known limitations, third-party dependencies/assets, and relevant learner issue references for a project.

## 4. Material-Step Documentation Rule

Every material learning or repository-changing action must be documented well enough that another person can understand how the relevant branch reached its current state.

Material steps include:

- commands that change or verify the development environment;
- files or folders created, changed, moved, or removed;
- dependencies installed, removed, or intentionally deferred;
- configuration changes;
- exercises or knowledge checks attempted;
- experiments run;
- important outputs or observations;
- architectural/course/repository decisions and their rationale;
- verification steps and their results;
- roadmap/progress changes;
- errors and troubleshooting that affected the work.

Do not log meaningless keystrokes or turn the repository into a raw chat transcript. The goal is reproducibility and learning value, not exhaustive surveillance of every interaction.

For normal learning, group related actions into one dated `docs/progress/learning-log.md` entry in chronological order. For course maintenance, group related actions into one dated `docs/history/repository-change-log.md` entry. Record exact commands when the command itself is part of the lesson or is required to reproduce the result.

## 5. Issue and Resolution Documentation

Errors and failed attempts are evidence. Do not remove their history simply because the final implementation works.

Use the issue log that matches the branch context:

- learner/coursework issue → `docs/progress/issues-and-resolutions.md`;
- reusable repository/course-maintenance issue → `docs/history/repository-issues-and-resolutions.md`.

Record an issue when it:

- blocks or materially delays a learning/setup/maintenance step;
- produces an error message that required diagnosis;
- reveals a misconception or important implementation detail;
- requires changing code, configuration, dependencies, environment, or instructions;
- is likely to recur or teach a reusable debugging/maintenance lesson.

Each issue record must include, when applicable:

- unique issue ID;
- date;
- roadmap phase/topic or repository area;
- status (`Open`, `Resolved`, or `Deferred`);
- observable symptom or error message;
- relevant context and reproduction steps;
- attempted fixes that materially informed the diagnosis;
- root cause, or explicitly `Unknown` if it remains unknown;
- final resolution steps;
- verification performed after the fix;
- learning/maintenance takeaway;
- affected files or commands;
- references used to diagnose the issue.

Preserve the original error text when useful, but redact secrets, tokens, credentials, private keys, and other sensitive values. Machine-specific paths may be shortened when the exact absolute path has no learning value.

Do not claim a root cause was found when only a workaround is known. Label workarounds and unresolved uncertainty explicitly.

## 6. Issue IDs and Cross-References

Learner issues use:

```text
LEARN-ISSUE-0001
LEARN-ISSUE-0002
```

Repository-maintenance issues use:

```text
REPO-ISSUE-0001
REPO-ISSUE-0002
```

The relevant issue log is canonical. Topic/project files and chronological logs should reference the issue ID rather than copying the full troubleshooting history into multiple locations.

## 7. Reference Rules

- Prefer official documentation, standards, papers, and primary sources.
- Use secondary tutorials only when they provide learning value not available from a primary source.
- OCI implementation documentation must reference current Oracle documentation.
- Record enough information to re-find a source: title, organization/author when useful, URL, and access date for mutable web documentation.
- Distinguish source-derived facts from learner conclusions or experiment results.
- When a reference was specifically used to resolve an issue, include it in both the relevant topic/project `references.md` when appropriate and the corresponding issue record.

## 8. Third-Party Licensing and Provenance

The root MIT License applies to original repository content. It does not automatically grant rights to redistribute third-party material.

Before committing a third-party dataset, model, code sample, image, paper, document, or other asset:

1. identify its source and owner/author when known;
2. identify its license or usage terms;
3. verify that repository redistribution is permitted;
4. record the source, license/terms, and any required attribution in the owning `README.md` or `references.md`;
5. preserve required notices when the license requires them.

If the license is unclear, unavailable, or does not permit redistribution, do not commit the material. Document how an authorized learner can obtain it instead.

Do not copy a third party's license text into the root `LICENSE` as though it governed the entire repository. Project- or asset-specific license/notice files may be included beside the material when required.

## 9. Code Documentation

Every code-related explanation or change must identify the exact repository path.

Do not document behavior the code does not implement. If code and documentation disagree, correct the inconsistency before marking the associated learning/project item complete.

When debugging code, preserve enough evidence to explain the observed behavior and verified fix without maintaining obsolete duplicate source files solely as a record of the error. Git history and the relevant issue record provide that history.

## 10. Experiment Documentation

For experiments, record at minimum:

- objective/hypothesis;
- data source;
- environment/dependencies;
- random seed when relevant;
- method;
- evaluation metric;
- result;
- interpretation;
- limitations and next step;
- material errors or failed runs, referenced by learner issue ID when applicable.

## 11. Reproducibility

A learning artifact should contain enough setup information for the learner to reproduce it later from a fresh environment. Do not rely on unstated notebook state, machine-local paths, hidden credentials, or undocumented chat context.

A documented resolution is not complete until its verification step is recorded. “The error disappeared” is insufficient when a stronger functional verification is available.
