# Initial Repository Setup

Use this guide to publish the public starter and begin your own progress without mixing personal work into the shared `main` branch.

Some Git actions happen here before the course formally teaches Git. That is fine, but treat them as setup only. Check off a Git objective later, after you can explain and demonstrate the operation yourself.

## 1. Public Repository

Use this repository name:

```text
ai-from-scratch-to-oci
```

Use this GitHub description:

```text
A hands-on AI learning journey from Python and data science fundamentals to machine learning, deep learning, LLMs, agentic AI, and production deployment on Oracle Cloud Infrastructure.
```

Put the scaffold contents directly at the repository root. Do not add another `ai-learning/` folder around them.

Your root should contain files and folders such as:

```text
README.md
LICENSE
course/
docs/
shared/
scripts/
templates/
```

## 2. Publish the Initial `main` Baseline

Use the first public `main` state as the reusable starting point for the course. When you create the GitHub repository, do not ask GitHub to generate another README, `.gitignore`, or license—the scaffold already contains them.

After you publish and verify the complete starter, tag that exact commit:

```text
v0.1.0
```

Keep `v0.1.0` unchanged so it always points to the original public starting state. Future fixes to the shared course can continue on `main` and use later version tags.

Record shared repository/course maintenance under `docs/history/`. Keep personal progress off `main`.

## 3. Start Your Progress Branch

Before you record learning work, create or switch to a long-lived progress branch:

```text
progress/<learner>
```

For example:

```text
progress/vincent
```

Creating this branch during setup does not mean you have completed the roadmap's Git branching objective. You will demonstrate that skill later when the course reaches it.

On your progress branch, update `docs/progress/current-learning-status.md` so it shows the branch you actually use.

## 4. Bring In Shared Course Updates Later

If the shared course needs a correction or improvement, create a temporary branch from `main`:

```text
course/<short-description>
```

After you review the change, merge it into `main`, update `docs/history/`, and publish the updated shared course state. Then merge the updated `main` into your progress branch.

Never merge your personal progress branch into `main`.

## 5. Keep a Learning Trail

Once learning begins, keep these documents handy:

- `docs/standards/documentation-standard.md`
- `docs/progress/learning-log.md`
- `docs/progress/issues-and-resolutions.md`

For each session, record the material actions you took, why you took them, important observations, evidence, and verification results. Do not put secrets or sensitive values into repository documentation.

If you hit an error or material issue, add or update an issue entry as part of the learning process. After you fix it, record how you verified the fix instead of documenting only the successful end state.

## 6. Create the Python Environment During Phase 0

Do not create the course `.venv` just to finish repository setup. Create it when Phase 0 reaches the Python environment objective, after you have verified your Python interpreter/version and understand what the environment is for.

Use `.venv/` as the default repository-local environment, and keep it ignored by Git.

## 7. Separate Git Learning From Repository Setup

Because the course itself is distributed through GitHub, you may clone/fork the repository and create a progress branch before the Git lessons explain those commands. Treat those early actions as setup.

When the roadmap later teaches Git:

- `git init` — practice it in a suitable temporary/practice repository instead of running it blindly inside an existing clone;
- `git clone` — explain and demonstrate what cloning created locally;
- `git status`, `git add`, `git commit`, `git pull`, `git push`, branches, and merging — provide your own evidence before checking them off.

## 8. Keep the Public Repository Safe

Before you publish or commit changes:

- inspect the files you staged;
- never commit `.env`, private keys, credentials, access tokens, or OCI secrets;
- keep `.venv/`, caches, generated model binaries, and large raw/processed datasets out of Git unless you have a documented reason to include them;
- check redistribution rights before you commit third-party datasets, models, code, images, papers, or other assets.

If you ever commit a secret, treat it as compromised. Rotate or revoke it; deleting it from the latest commit is not enough.

## 9. Begin Phase 0

Once the public baseline and your progress branch exist, start with the first active item in `docs/progress/current-learning-status.md`.

Before you end each session:

1. verify the work you performed;
2. update `docs/progress/learning-log.md`;
3. finish or explicitly defer any issue entries;
4. update `docs/progress/current-learning-status.md`;
5. update the master roadmap only for objectives you actually completed;
6. identify the exact next roadmap item.

## References

- Python Packaging User Guide — virtual environments: https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/
- GitHub Docs — repository best practices: https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories
- GitHub Docs — licensing a repository: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository
- GitHub Docs — storing secrets safely: https://docs.github.com/en/get-started/learning-to-code/storing-your-secrets-safely
