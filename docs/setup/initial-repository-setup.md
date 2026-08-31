# Initial Repository Setup

This guide describes how the public starter is published and how a learner begins from it without mixing personal progress into the canonical course branch.

Repository administration performed before instruction does not by itself satisfy a Git learning objective. Git checklist items are marked complete only after the learner can explain and demonstrate the relevant operation during the course.

## 1. Canonical Public Repository

Repository name:

```text
ai-from-scratch-to-oci
```

GitHub description:

```text
A hands-on AI learning journey from Python and data science fundamentals to machine learning, deep learning, LLMs, agentic AI, and production deployment on Oracle Cloud Infrastructure.
```

The scaffold contents belong directly at the repository root. Do not create an extra nested `ai-learning/` directory inside the GitHub repository.

The root should contain files/folders such as:

```text
README.md
LICENSE
course/
docs/
shared/
scripts/
templates/
```

## 2. Publishing the Initial `main` Baseline

The first public `main` state is the reusable starting point for every learner. When creating the GitHub repository, do not ask GitHub to generate a second README, `.gitignore`, or license because the scaffold already contains them.

After the complete starter is published and verified, tag that exact commit:

```text
v0.1.0
```

`v0.1.0` is the immutable original public starting baseline. Future fixes to the reusable course may continue on `main` and receive later version tags.

Record repository-maintenance changes under `docs/history/`. Do not place personal learner progress on `main`.

## 3. Starting Personal Progress

Before recording learning work, create or use a long-lived learner branch:

```text
progress/<learner>
```

Example:

```text
progress/paul
```

A learner may create this branch mechanically as part of initial repository administration. Doing so does not mean the roadmap's Git branch objective is complete; that objective requires later understanding and demonstrated use.

Update `docs/progress/current-learning-status.md` on the progress branch by replacing the placeholder branch name.

## 4. Course Updates After Learning Has Begun

If the canonical course needs a correction or improvement, create a temporary branch from `main`:

```text
course/<short-description>
```

After review, merge that change into `main`, update `docs/history/`, and publish the new canonical state. Learners then merge `main` into their own `progress/<learner>` branch.

Do not merge a learner's personal progress branch into `main`.

## 5. Learner Documentation Trail

Once learning begins, read:

- `docs/standards/documentation-standard.md`
- `docs/progress/learning-log.md`
- `docs/progress/issues-and-resolutions.md`

For each learning session, record the material commands/actions, why they were performed, important observations, evidence, and verification results. Do not paste secrets or sensitive values into repository documentation.

If an error or material issue occurs, create/update a learner issue entry before moving on; after resolving it, record how the fix was verified.

## 6. Python Environment

Do not create the course `.venv` merely as bootstrap automation. Create it when Phase 0 reaches the corresponding Python environment objective, after the Python interpreter/version has been verified and the learner understands what the environment is for.

The repository-local environment will use `.venv/` by default and must remain ignored by Git.

## 7. Git Learning Versus Repository Administration

Because the course itself is distributed through GitHub, some learners will clone/fork the repository and create a progress branch before the Git lessons explain those operations. Treat those early actions as setup only.

When the roadmap later teaches:

- `git init` — practice it in an appropriate temporary/practice repository rather than running it blindly inside an already cloned repository;
- `git clone` — explain and demonstrate what cloning created locally;
- `git status`, `git add`, `git commit`, `git pull`, `git push`, branches, and merging — require actual learner evidence before checking them off.

## 8. Public Repository Safety

Before publishing or committing changes:

- inspect staged files;
- never commit `.env`, private keys, credentials, access tokens, or OCI secrets;
- keep `.venv/`, caches, generated model binaries, and large raw/processed datasets out of Git unless a documented exception applies;
- verify third-party redistribution rights before committing external datasets, models, code, images, papers, or other assets.

If a secret is ever committed, treat it as compromised and rotate/revoke it rather than relying on deletion from the latest commit.

## 9. Beginning Phase 0

Once the public baseline and learner progress branch exist, course learning begins at the first active item in `docs/progress/current-learning-status.md`.

Before ending each session:

1. verify the work performed;
2. update `docs/progress/learning-log.md`;
3. finish or explicitly defer learner issue entries;
4. update `docs/progress/current-learning-status.md`;
5. update the master roadmap only for objectives with actual completion evidence;
6. identify the exact next roadmap item.

## References

- Python Packaging User Guide — virtual environments: https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/
- GitHub Docs — repository best practices: https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories
- GitHub Docs — licensing a repository: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository
- GitHub Docs — storing secrets safely: https://docs.github.com/en/get-started/learning-to-code/storing-your-secrets-safely
