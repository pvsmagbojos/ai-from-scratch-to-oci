# Repository Change Log

This is the append-only history of material changes to the canonical course repository on `main`.

It records course scaffolding, standards, prompt changes, repository-governance decisions, public-baseline changes, and other maintenance that affects all learners. Personal learning activity belongs in `docs/progress/learning-log.md` on a learner's `progress/<learner>` branch.

## 2026-08-31 — Repository Standards and Course Scaffold

- Created the canonical AI learning repository structure.
- Added the master AI learning roadmap.
- Defined repository, documentation, exercise, notebook, project, environment, secrets, and Git standards.
- Defined the master AI tutor prompt and specialized session prompts.
- Created phase folders for all roadmap phases.
- Kept Python environment creation and Git-skill demonstrations as Phase 0 learning work rather than automating them as evidence of competency.

## 2026-08-31 — Reproducible Tutor Onboarding and Troubleshooting Documentation

- Expanded `README.md` with a self-contained AI-tutor onboarding workflow so a new learner/conversation can resume from repository state rather than hidden chat context.
- Established that every material learning or repository-changing action must be documented with its purpose, meaningful result, and verification when applicable.
- Added canonical troubleshooting documentation requirements for observable symptoms/errors, context, meaningful attempts, evidence-supported root cause, resolution/workaround, verification, and learning takeaway.
- Encountered and resolved `REPO-ISSUE-0001`: the external `tree` CLI was unavailable while regenerating the repository-tree snapshot, so a Python filesystem traversal was used instead and the result was verified.

## 2026-08-31 — Public Repository Baseline and Branching Model

- Set the canonical public repository name to `ai-from-scratch-to-oci`.
- Defined the repository description as a hands-on path from Python/Data Science fundamentals through ML, deep learning, LLMs, agentic AI, and production deployment on Oracle Cloud Infrastructure.
- Added the MIT License for original repository content.
- Added third-party licensing rules so external datasets, models, code, images, papers, and other materials retain their own licensing requirements.
- Defined `main` as the canonical reusable course starting point rather than an individual learner's progress history.
- Defined long-lived `progress/<learner>` branches for personal learning artifacts and progress.
- Defined temporary `course/<change>` branches from `main` for canonical course corrections and improvements.
- Defined optional `feature/<short-description>` and `experiment/<short-description>` branches from a learner progress branch for isolated project work.
- Established that personal progress is never merged into `main`; course updates flow from `main` into learner progress branches.
- Separated repository-maintenance history/issues under `docs/history/` from learner history/issues under `docs/progress/` to avoid conflicts when synchronizing `main` into progress branches.
- Reset learner progress and issue logs to a clean pre-learning starting state.
- Designated `v0.1.0` as the intended immutable tag for the first published public baseline.
- Clarified that publishing/cloning/branching the baseline before instruction does not by itself prove completion of Git learning objectives; those require later explanation and demonstrated use.
- Performed a pre-publication hygiene check for unexpected `.env` files, private-key files, and common secret-token patterns in non-documentation files; no matches were found.
- Regenerated and verified the repository-tree snapshot with the final public root name and `docs/history/` structure.
- Generated and verified the distributable starter archive, including `README.md`, `LICENSE`, roadmap, standards, history, and clean learner progress files.
