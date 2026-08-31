# AI From Scratch to OCI

A hands-on AI learning journey from Python and data science fundamentals to machine learning, deep learning, LLMs, agentic AI, and production deployment on Oracle Cloud Infrastructure.

This repository provides both the reusable course starting point and the structure for a learner's working record. The master roadmap is authoritative for course scope and completion. Repository standards define where notes, exercises, notebooks, projects, prompts, references, issues, and progress records belong.

## Public Repository Model

The repository is intentionally designed so multiple learners can begin from the same canonical starting point without mixing personal progress into the shared course baseline.

- `main` — canonical reusable course starting point and course-maintenance history. Do not commit personal learning artifacts directly to `main`.
- `v0.1.0` — immutable tag for the initial published public baseline.
- `progress/<learner>` — long-lived branch containing one learner's roadmap state, exercises, notebooks, projects, learning log, and learner issue history.
- `course/<short-description>` — temporary branch created from `main` for corrections or improvements that should become part of the shared course.
- `feature/<short-description>` / `experiment/<short-description>` — optional temporary branches created from a learner's progress branch when isolated implementation or experimentation is useful.

Personal progress is never merged back into `main`. When `main` receives a course correction or update, learners may merge the updated `main` into their own progress branch.

Publishing, cloning, or creating a branch before instruction is repository setup; it does not by itself satisfy Git learning objectives. Git checklist items are completed only after the learner can explain and demonstrate the relevant operation.

## Start Here

1. Fork or clone the repository.
2. Create/use a personal `progress/<learner>` branch before recording learning work.
3. Read `docs/setup/initial-repository-setup.md`.
4. Read `docs/standards/repository-structure-standard.md`.
5. Read `docs/standards/learning-session-standard.md`.
6. Read `docs/standards/documentation-standard.md`.
7. Use `docs/prompts/new-learning-session-prompt.md` to start each new learning conversation.
8. Track the active item in `docs/progress/current-learning-status.md`.
9. Record material learning steps in `docs/progress/learning-log.md`.
10. Record learner errors, failed attempts, diagnoses, and verified resolutions in `docs/progress/issues-and-resolutions.md`.
11. Begin with Phase 0 and do not mark an item complete until its required exercise or knowledge check has been passed.

## How to Use This Course With an AI Tutor

A new AI conversation must be able to continue the course without relying on hidden chat history, account memory, or knowledge of how this repository was created.

### 1. Provide the Core Context

At minimum, make these files available to the AI tutor:

- `docs/prompts/ai-tutor-master-prompt.md`
- `docs/roadmap/ai-learning-roadmap-master-checklist.md`
- `docs/progress/current-learning-status.md`
- `docs/standards/repository-structure-standard.md`
- `docs/standards/learning-session-standard.md`
- `docs/standards/documentation-standard.md`
- files from the active topic/project folder

Also provide `docs/progress/issues-and-resolutions.md` when an unresolved or previously encountered learner issue may affect the current work. Repository maintainers should provide the relevant `docs/history/` records when a course-level maintenance issue is involved.

### 2. Start the Conversation

Use `docs/prompts/new-learning-session-prompt.md` as the session bootstrap prompt. Replace its placeholder with the exact active roadmap item from `docs/progress/current-learning-status.md`.

The master tutor prompt is the standing behavioral contract. The session prompt tells the tutor where to resume.

### 3. Learn in Roadmap Order

The AI tutor should teach the current roadmap item, assign an exercise or knowledge check, review the learner's evidence, and only then mark the item complete. Prerequisites may be taught when genuinely required, but the tutor must not silently skip or reorder roadmap work.

### 4. Keep the Repository as the Source of Truth

Do not depend on a previous conversation to remember course state. Decisions, progress, references, exercises, troubleshooting, and completed evidence must be written into the repository's canonical files.

If a new conversation disagrees with the repository, inspect the repository first. Update a canonical document only when there is an intentional new decision or a verified correction.

### 5. Document the Process, Including Problems

Every material learning step must leave a useful record. This includes commands run, files changed, decisions made, exercises attempted, verification results, and progress changes.

Errors and unsuccessful attempts are part of the learning record. Do not erase them after a fix. Record the observable error or symptom, relevant context, meaningful attempted fixes, the root cause when known, the final resolution or workaround, how the result was verified, and what should be remembered next time.

Course-maintenance activity on `main` follows the same principle but is recorded under `docs/history/` rather than mixed into a learner's progress logs.

### 6. Close the Session Properly

Before ending a learning session, synchronize:

- the master roadmap;
- the active topic/project documentation;
- `docs/progress/current-learning-status.md`;
- `docs/progress/learning-log.md`;
- `docs/progress/issues-and-resolutions.md` when issues occurred;
- references and durable notes produced by the session.

A future learner conversation should be able to inspect those files and understand where the course stopped, what was learned, what failed, how problems were resolved, and exactly what comes next.

## Canonical Documents

- Roadmap: `docs/roadmap/ai-learning-roadmap-master-checklist.md`
- Repository structure and Git/branch rules: `docs/standards/repository-structure-standard.md`
- Learning/session rules: `docs/standards/learning-session-standard.md`
- Documentation rules: `docs/standards/documentation-standard.md`
- Master tutor prompt: `docs/prompts/ai-tutor-master-prompt.md`
- Current learner progress: `docs/progress/current-learning-status.md`
- Learner process history: `docs/progress/learning-log.md`
- Learner issues and resolutions: `docs/progress/issues-and-resolutions.md`
- Repository change history: `docs/history/repository-change-log.md`
- Repository issues and resolutions: `docs/history/repository-issues-and-resolutions.md`

## Repository Principle

Keep learning evidence close to the roadmap item that produced it. Do not create a large shared dumping ground for notebooks, datasets, model files, or outputs. Reusable material belongs in `shared/` only when it is genuinely reused by multiple phases or projects.

The repository, not a chat transcript, is the durable record of the course.

## License

Original content in this repository is available under the MIT License. See `LICENSE`.

Third-party datasets, models, code, images, papers, documentation, and other materials are not automatically relicensed under MIT. Their original licenses and terms still apply. The course documentation standard requires third-party provenance and licensing to be recorded before redistributable material is committed.
