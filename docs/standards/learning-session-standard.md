# Learning Session Standard

## 1. Purpose

Use this standard to keep each roadmap item consistent: learn it, practice it, prove you understand it, document what happened, and only then mark it complete. Follow this workflow in future AI-learning conversations unless a roadmap item genuinely needs something different.

## 2. Repository and Branch Context

At the start of each learning session, give your tutor the exact repository and learning branch you are using. That can be the original repository, your fork, or another repository intentionally created from this course.

`progress/<learner>` is the recommended branch pattern, but you can intentionally use another name. Keep your personal progress off upstream `main`.

If you use a fork, treat your fork + your learning branch as the source of truth for your progress. Use the upstream repository only when you need to compare, maintain, or synchronize shared course material.

If you discover a defect in the reusable course itself, record how it affected your learning branch. Make the shared correction through a `course/<short-description>` branch created from upstream `main`, as described in `repository-structure-standard.md`.

## 3. Source of Truth

When your repository and branch are accessible, have the tutor read them directly instead of asking you to upload the same documentation again. Start with `README.md` on your branch. If direct access is unavailable, use a connected repository integration or upload only the specific files needed. Do not silently use stale files from an older conversation.

Use these sources in this order:

1. your specified repository + learning branch for personal progress;
2. `README.md` on that branch for setup/session instructions;
3. `docs/roadmap/ai-learning-roadmap-master-checklist.md` for course scope and completion state;
4. `docs/progress/current-learning-status.md` for your active item and immediate next step;
5. your current topic/project files for implementation state and evidence;
6. `docs/progress/issues-and-resolutions.md` for relevant unresolved or previously solved problems;
7. `docs/standards/` for repository and documentation rules;
8. upstream `main` only when you are comparing or synchronizing shared course changes;
9. current authoritative external documentation for technologies that can change over time.

Do not silently rewrite the roadmap. If you discover a missing prerequisite or topic, document the gap and make the smallest roadmap change that solves it.

### What You Should Expect From Your Tutor

Your tutor should challenge weak assumptions, correct mistakes, explain trade-offs, and verify changing information instead of simply agreeing with you. It should teach the underlying concept before hiding it behind a framework, keep code grounded in your live repository, and require evidence before marking roadmap work complete.

You should normally get a chance to attempt meaningful exercises before seeing the full solution. If later work shows that an earlier concept is still unclear, revisit it rather than carrying the gap forward.

For current OCI implementation details, expect the tutor to verify official Oracle documentation before teaching or generating implementation-specific guidance.

The detailed behavior contract is in `docs/prompts/ai-tutor-master-prompt.md`; the README gives the shorter learner-facing summary.

## 4. Standard Lesson Sequence

For each checklist item:

1. **Orient** — understand what you are learning and why it matters later.
2. **Check prerequisites** — confirm only the knowledge you actually need for this item.
3. **Learn the concept** — start with intuition, then add definitions, mathematics, or implementation details when useful.
4. **Work through an example** — use one grounded example when it helps the concept click.
5. **Try a guided exercise** — apply the concept with some scaffolding.
6. **Try an independent exercise** — apply it again with less help when the item is practical.
7. **Review** — explain, predict, debug, derive, or otherwise show that you understand the item.
8. **Document** — record the material steps, notes, references, code/notebook artifacts, and issues/resolutions.
9. **Verify** — check that the exercise, environment change, fix, or implementation really works.
10. **Complete** — mark the checklist item complete only after the evidence and verification are there.

For a conceptual item, a knowledge check may be enough. For a practical item, do hands-on work.

## 5. Completion Rules

An explanation by itself does not complete a roadmap item.

Use evidence that fits the item, such as:

- a correct explanation in your own words;
- a completed exercise;
- a working script or notebook;
- a correct manual derivation;
- a successful debugging task;
- a project artifact;
- an exit-criteria demonstration.

To complete a phase, also finish its project or exit criteria when the roadmap defines them.

## 6. Exercise Rules

Every roadmap item gets at least one exercise or knowledge check.

Prefer active work—recall, prediction, implementation, debugging, comparison, or explanation—over passive reading.

When code is relevant:

- identify the exact repository path and filename;
- do not invent missing project types, APIs, files, schemas, or architecture;
- collect materially missing implementation context before producing grounded code;
- attempt the exercise before asking for a full solution unless you intentionally want a worked solution;
- understand the correction instead of only replacing your code.

## 7. Build From Scratch Before Hiding the Details

When the roadmap asks for a from-scratch implementation, do not replace it with a framework call. You can use a library afterward to compare and validate your result.

Examples include manual gradient descent, NumPy neural networks, attention primitives, retrieval similarity, and agent loops.

## 8. Choose Notebooks or Scripts Deliberately

Use notebooks when interactivity, visualization, data exploration, or step-by-step mathematical reasoning helps the lesson.

Use Python scripts/modules when you are learning software structure, reusable functions/classes, testing, APIs, agents, production services, or code that should run non-interactively.

Before you consider a notebook complete, restart its kernel and run it top-to-bottom without relying on hidden state.

## 9. Learn the Mathematics, Not Just the API

For mathematical material:

1. understand the intuition;
2. define the notation;
3. work through a small numeric example manually;
4. connect the math to AI/ML;
5. implement or verify it in Python/NumPy when the roadmap calls for it.

Do not skip the mathematical meaning by jumping straight to a library API.

## 10. Verify OCI and Other Changing Technologies

For OCI implementation work, use Oracle's current official documentation. Verify service names, model availability, APIs, SDK behavior, regional availability, IAM requirements, limits, and agent tooling before you implement anything.

Keep stable concepts separate from product details that may change.

If a service is renamed, deprecated, or materially changed, update the existing roadmap/documentation instead of creating a competing document.

## 11. Document the Process and the Problems

Document throughout the session, not only after something works.

For every material step, keep enough information to reconstruct what happened: the action or command, why you did it, the important result, and how you verified it when verification makes sense. Group these steps into the dated entry in `docs/progress/learning-log.md`.

When you hit an error or material issue:

1. record the symptom or useful exact error text;
2. record the context and reproduction steps;
3. investigate without pretending an unverified guess is the root cause;
4. keep meaningful failed attempts when they teach something or narrow the diagnosis;
5. record the root cause once the evidence supports it;
6. record the final fix or workaround;
7. verify the result with a relevant functional check;
8. write down the reusable lesson or prevention step;
9. add or update the issue in `docs/progress/issues-and-resolutions.md`;
10. reference the issue ID from your learning log and relevant topic/project documentation.

Never put secrets in logs. Redact credentials, tokens, private keys, and sensitive values before you commit documentation.

If you only found a workaround, call it a workaround. Do not label it a root-cause fix just because you can continue.

## 12. Close the Session Cleanly

At the end of a learning session:

- update `docs/progress/current-learning-status.md`;
- append the material steps and verification to `docs/progress/learning-log.md`;
- update `docs/progress/issues-and-resolutions.md` for every material issue you encountered;
- update the master roadmap only for items you actually completed or intentionally changed;
- update topic notes/references when you added durable learning;
- update existing documentation instead of creating duplicate replacement files;
- record unresolved questions or blockers;
- identify the exact next roadmap item.

If you make a decision that changes repository standards or the course itself, update the relevant standard in the same session.

## 13. AI-Assisted Output Rule

When your tutor produces a complete repository file longer than 20 lines, have it provided as an attachment/downloadable file instead of filling the conversation with a full preview. Short patches or snippets can still be shown inline when they are useful.
