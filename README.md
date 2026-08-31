# AI From Scratch to OCI

A hands-on AI learning journey from Python and data science fundamentals to machine learning, deep learning, LLMs, agentic AI, and production deployment on Oracle Cloud Infrastructure.

Use this repository as both your course starting point and your working learning record. The master roadmap defines what you need to learn and what counts as complete. The repository standards tell you where to keep notes, exercises, notebooks, projects, references, issues, and progress records.

## Public Repository Model

The repository is set up so you can start from the same shared course material as everyone else without mixing your personal work into `main`.

- `main` — the reusable course starting point and shared course-maintenance history. Keep personal learning work off this branch.
- `v0.1.0` — the immutable tag for the original published starting point.
- `v0.2.1` — the current shared course release and recommended starting point for new progress branches.
- `v0.2.0` — the previous shared course release, retained as an immutable historical snapshot.
- `progress/<learner>` — your long-lived learning branch. Keep your roadmap state, exercises, notebooks, projects, learning log, and issue history here.
- `course/<short-description>` — a temporary branch from `main` for fixes or improvements that should become part of the shared course.
- `feature/<short-description>` / `experiment/<short-description>` — optional temporary branches from your progress branch when you want isolated implementation or experimentation work.

Never merge personal progress back into `main`. If `main` receives a course correction or improvement, merge the updated `main` into your progress branch instead.

You may need to clone, publish, or create a branch before the Git lessons teach those operations. Treat that as setup only. Check off a Git objective later, after you can explain and demonstrate it yourself.

## Start Here

1. Fork or clone the original course repository, or use a repository intentionally created from it.
2. Create or switch to your `progress/<learner>` branch before you record learning work.
3. Read `docs/setup/initial-repository-setup.md`.
4. Read `docs/standards/repository-structure-standard.md`.
5. Read `docs/standards/learning-session-standard.md`.
6. Read `docs/standards/documentation-standard.md`.
7. If you are learning with an AI tutor, identify your exact repository URL and learning branch, then use `docs/prompts/new-learning-session-prompt.md` to start each new conversation.
8. Keep your active roadmap item in `docs/progress/current-learning-status.md`.
9. Record material learning steps in `docs/progress/learning-log.md`.
10. Record errors, failed attempts, diagnoses, and verified resolutions in `docs/progress/issues-and-resolutions.md`.
11. Begin with Phase 0. Only mark an item complete after you have the required exercise, knowledge check, or other evidence.

## How to Use This Course With an AI Tutor

You should be able to start a fresh AI conversation and continue the course without relying on hidden chat history, account memory, or repeated file uploads. If your repository is publicly readable, have the tutor read your live learning branch first.

### 1. Identify Your Repository and Branch

At the start of a new conversation, provide these two values:

```text
Repository: <repository-url>
Learning branch: <learning-branch>
```

For example:

```text
Repository: https://github.com/pvsmagbojos/ai-from-scratch-to-oci
Learning branch: progress/vincent
```

If you are using a fork, you can also provide the upstream repository:

```text
Repository: https://github.com/alice/ai-from-scratch-to-oci
Learning branch: progress/alice
Upstream repository: https://github.com/pvsmagbojos/ai-from-scratch-to-oci
```

Your repository can be the original public repository, your public fork, or another repository intentionally created from this course.

`progress/<learner>` is the recommended branch pattern, but you can use another branch name intentionally. If you do, give the tutor that exact branch name.

If you are using a fork, your fork + your learning branch is the source of truth for your progress. Use the original `pvsmagbojos/ai-from-scratch-to-oci` repository only as the upstream source for shared course updates. Do not use upstream `main` in place of your branch when reading your exercises, notebooks, logs, or progress.

### 2. Have the Tutor Read the Live Repository First

If your repository and branch are publicly accessible, have the tutor read the live branch instead of asking you to upload the same documentation again.

Start with `README.md` on your learning branch, then use these files as the main course context:

- `docs/prompts/ai-tutor-master-prompt.md`
- `docs/roadmap/ai-learning-roadmap-master-checklist.md`
- `docs/progress/current-learning-status.md`
- `docs/standards/repository-structure-standard.md`
- `docs/standards/learning-session-standard.md`
- `docs/standards/documentation-standard.md`
- the files for your active topic or project

Also read `docs/progress/issues-and-resolutions.md` when an unresolved or previously solved issue could affect the current work. Use `docs/history/` when a shared course or repository-maintenance decision is relevant.

If the repository is private or cannot be read directly, use a connected GitHub integration when one is available. Otherwise, upload only the specific files needed for the current work. Do not let an old copy from a previous conversation silently override the live repository.

### 3. Start the Conversation

Use `docs/prompts/new-learning-session-prompt.md` as your session bootstrap prompt. Fill in your exact repository URL and learning branch.

When the live branch is readable, the tutor should get your active roadmap item from `docs/progress/current-learning-status.md` instead of asking you to paste it manually.

### 4. Know What to Expect From the Tutor

Your AI tutor should do more than answer questions. It should help you build understanding progressively and challenge weak assumptions instead of simply agreeing with you.

Expect the tutor to:

- start with intuition, then add technical detail, mathematics, and implementation when they are useful;
- verify changing or vendor-specific information instead of relying on stale knowledge, and prefer current official Oracle documentation for OCI implementation details;
- clearly separate facts, assumptions, inferences, recommendations, and documentation-backed claims;
- correct technical mistakes directly and explain why they are wrong;
- explain important trade-offs when several approaches are valid instead of presenting one preference as the only answer;
- avoid introducing frameworks or abstractions before you understand the underlying concept when the abstraction would hide something important;
- ground code in the live repository and ask for all genuinely missing implementation context at once rather than inventing files, APIs, types, or architecture;
- give you meaningful exercises that require you to think, implement, explain, debug, compare, or make a technical decision;
- let you attempt exercises before giving the full solution unless you ask for it or need it to continue;
- require evidence of understanding or implementation before marking a roadmap item complete;
- document material learning steps, decisions, errors, meaningful failed attempts, fixes or workarounds, verification, and lessons learned;
- distinguish a proven root cause from a workaround that merely makes the problem disappear; and
- keep explanations clear, concise, direct, and natural rather than overly formal or filled with unnecessary jargon.

The full tutor behavior rules live in `docs/prompts/ai-tutor-master-prompt.md`. If your AI platform supports project-level or persistent instructions, you can also use those rules there, but the repository copy keeps the course portable across tools and accounts.

### 5. Follow the Roadmap in Order

Work through the current roadmap item, complete its exercise or knowledge check, and review the evidence before marking it complete. If a prerequisite is genuinely missing, learn that prerequisite first and document why it was needed. Do not silently skip or reorder roadmap work.

### 6. Keep Your Learning Branch as the Progress Source of Truth

Do not depend on a previous conversation to remember where you stopped. Keep decisions, progress, references, exercises, troubleshooting, and completion evidence in your specified repository branch.

For your personal learning state, use this order:

1. your specified repository + your specified learning branch;
2. `README.md` and shared course documents on that branch;
3. your active topic/project files on that branch;
4. upstream `main` only when you are comparing or synchronizing shared course updates.

If a new conversation disagrees with the repository, inspect your learning branch first. Update the relevant source-of-truth document only when you intentionally make a new decision or verify a correction.

### 7. Document the Process, Including Problems

Keep a useful record of every material learning step: commands you ran, files you changed, decisions you made, exercises you attempted, important results, verification, and progress changes.

Errors and unsuccessful attempts are part of the learning process, so keep them too. Record the symptom or error, useful context, meaningful failed attempts, the root cause when you can prove it, the final fix or workaround, how you verified the result, and what you should remember next time.

If the issue affects the shared course itself rather than only your personal work, record the shared fix under `docs/history/` on `main` instead of mixing it into your personal issue history.

### 8. Close the Session Properly

Before you end a learning session, update the files affected by the work on your learning branch:

- the master roadmap;
- the active topic/project documentation;
- `docs/progress/current-learning-status.md`;
- `docs/progress/learning-log.md`;
- `docs/progress/issues-and-resolutions.md` when an issue occurred;
- references and durable notes created during the session.

A future conversation should be able to read the same repository and branch and quickly understand where you stopped, what you learned, what failed, how you fixed it, and what comes next.

## Core Documents

- Roadmap: `docs/roadmap/ai-learning-roadmap-master-checklist.md`
- Repository structure and Git/branch rules: `docs/standards/repository-structure-standard.md`
- Learning/session rules: `docs/standards/learning-session-standard.md`
- Documentation rules: `docs/standards/documentation-standard.md`
- Master tutor prompt: `docs/prompts/ai-tutor-master-prompt.md`
- Current progress: `docs/progress/current-learning-status.md`
- Learning history: `docs/progress/learning-log.md`
- Your issues and resolutions: `docs/progress/issues-and-resolutions.md`
- Shared repository change history: `docs/history/repository-change-log.md`
- Shared repository issues and resolutions: `docs/history/repository-issues-and-resolutions.md`

## Repository Principle

Keep learning evidence close to the roadmap item that produced it. Avoid turning `shared/` into a dumping ground for notebooks, datasets, model files, or outputs. Put something in `shared/` only when multiple phases or projects genuinely reuse it.

Treat the repository—not a chat transcript—as the durable record of your course progress.

## License

Original content in this repository is available under the MIT License. See `LICENSE`.

Third-party datasets, models, code, images, papers, documentation, and other materials keep their original licenses and terms. Before you commit third-party material, check that redistribution is allowed and record the source/license as required by `docs/standards/documentation-standard.md`.
