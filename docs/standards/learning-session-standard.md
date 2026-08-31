# Learning Session Standard

## 1. Purpose

This standard defines how each roadmap item is taught, practiced, assessed, documented, and marked complete. It applies to all future AI-learning conversations unless a roadmap item explicitly requires a different workflow.

## 2. Branch Context

Learning sessions operate on a learner's `progress/<learner>` branch. Do not commit personal progress directly to `main`. If the session discovers a defect in the reusable course itself, document the learner impact on the progress branch and route the canonical correction through a `course/<short-description>` branch from `main` as defined in `repository-structure-standard.md`.

## 3. Source of Truth

Use these documents in this order:

1. `docs/roadmap/ai-learning-roadmap-master-checklist.md` for course scope and completion state.
2. `docs/progress/current-learning-status.md` for the active item and immediate next step.
3. The current topic/project files for implementation state and learner evidence.
4. `docs/progress/issues-and-resolutions.md` for relevant unresolved or previously solved problems.
5. `docs/standards/` for repository and documentation rules.
6. Current authoritative external documentation for technologies whose behavior or product surface can change.

Do not silently rewrite the roadmap. If a prerequisite or missing topic is discovered, document the gap and propose the smallest roadmap change required.

## 4. Standard Lesson Sequence

For each checklist item:

1. **Orient** — state what is being learned and why it matters to later AI work.
2. **Prerequisite check** — briefly confirm only the prerequisite knowledge required for the item.
3. **Teach the concept** — start with intuition, then add formal definitions, mathematics, or implementation details as appropriate.
4. **Worked example** — show one grounded example when an example materially helps.
5. **Guided exercise** — give a small exercise that can be completed with the newly taught concept.
6. **Independent exercise** — require the learner to apply the concept with less scaffolding when the item is practical.
7. **Review** — ask for an explanation, prediction, debugging step, derivation, or other evidence of understanding.
8. **Document** — record the material steps performed, update notes/references and code/notebook artifacts, and record any issues/resolutions.
9. **Verify** — verify that the exercise, environment change, fix, or implementation behaves as intended.
10. **Complete** — mark the checklist item complete only after the required evidence and verification exist.

A purely conceptual item may use a knowledge check instead of code. A practical item must include hands-on work.

## 5. Completion Rules

Do not mark a roadmap item complete merely because it has been explained.

Completion requires evidence appropriate to the item, such as:

- a correct explanation in the learner's own words;
- a completed exercise;
- a working script/notebook;
- a correct manual derivation;
- a successful debugging task;
- a project artifact;
- an exit-criteria demonstration.

Phase completion additionally requires its explicit project/exit criteria where the roadmap defines them.

## 6. Exercise Rules

Every roadmap item receives at least one exercise or knowledge check.

Prefer exercises that require active recall, prediction, implementation, debugging, comparison, or explanation rather than passive reading.

When code is relevant:

- identify the exact repository path/filename;
- do not invent missing project types, APIs, files, schemas, or architecture;
- request all materially missing implementation context at once before producing grounded code;
- let the learner attempt the exercise before presenting a full solution unless a worked solution was requested;
- explain corrections rather than only replacing code.

## 7. From-Scratch Before Abstraction

Where the roadmap explicitly requires a from-scratch implementation, do not replace it with a framework call. Libraries may be used afterward for comparison and validation.

Examples include manual gradient descent, NumPy neural networks, attention primitives, retrieval similarity, and agent loops.

## 8. Notebook and Script Choice

Use notebooks when interactivity, visualization, data exploration, or stepwise mathematical reasoning is part of the lesson.

Use Python scripts/modules when teaching software structure, reusable functions/classes, testing, APIs, agents, production services, or code that should run non-interactively.

A completed notebook must restart and run top-to-bottom without hidden state.

## 9. Mathematics Teaching Rule

For mathematical material:

1. explain the intuition;
2. define the notation;
3. work a small numeric example manually;
4. connect the math to AI/ML;
5. implement or verify it in Python/NumPy when the roadmap calls for implementation.

Do not skip mathematical meaning by jumping directly to library APIs.

## 10. OCI and Other Mutable Technologies

For OCI implementation work, Oracle's current official documentation is authoritative. Verify service names, model availability, APIs, SDK behavior, regional availability, IAM requirements, limits, and agent tooling before implementation.

Clearly distinguish stable conceptual teaching from current product-specific behavior.

If a service is renamed, deprecated, or materially changed, update the existing roadmap/documentation rather than creating a competing document.


## 11. Process and Troubleshooting Documentation

Documentation happens throughout the session, not only after success.

For every material step, preserve the information needed to reconstruct what happened: the action/command, purpose, important result, and verification when applicable. Group these steps into the dated entry in `docs/progress/learning-log.md`.

When an error or material issue occurs:

1. record the observable symptom or exact error text when useful;
2. record the context and reproducible steps;
3. investigate without pretending an unverified hypothesis is the root cause;
4. record meaningful failed attempts when they teach something or narrow the diagnosis;
5. identify the root cause when evidence supports it;
6. record the resolution or workaround;
7. verify the fix with a relevant functional check;
8. record the reusable lesson/prevention step;
9. add or update the corresponding entry in `docs/progress/issues-and-resolutions.md`;
10. reference the issue ID from the session's `learning-log.md` entry and relevant topic/project documentation.

Never expose secrets in logs. Redact credentials, tokens, private keys, and sensitive values from commands or error output before committing documentation.

A workaround does not become a confirmed root-cause fix merely because work can continue. Preserve that distinction.

## 12. Session Closeout

At the end of a learning session:

- update `docs/progress/current-learning-status.md`;
- append a chronological entry to `docs/progress/learning-log.md` covering the material steps and verification performed;
- update `docs/progress/issues-and-resolutions.md` for every material error or issue encountered, including its resolution/verification when resolved;
- update the master roadmap only for items actually completed or deliberately changed;
- update topic notes/references when durable learning was added;
- update existing documentation instead of creating duplicate replacement documents;
- record unresolved questions/blockers;
- identify the next exact roadmap item.

If a changed decision affects repository standards or the course, update the relevant standard document in the same session.

## 13. Output Rule for AI-Assisted Sessions

When the tutor produces a complete repository file longer than 20 lines, provide it as an attachment/downloadable file rather than flooding the conversation with a full preview. Short patches or snippets may be shown inline when useful.
