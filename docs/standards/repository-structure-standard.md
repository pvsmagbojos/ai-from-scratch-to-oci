# Repository Structure Standard

## 1. Purpose

Use this structure throughout `ai-from-scratch-to-oci`. It keeps your work traceable and reproducible while leaving room to grow from learning exercises into production-style Python and OCI projects.

## 2. Top-Level Structure

```text
ai-from-scratch-to-oci/
├── README.md
├── LICENSE
├── .editorconfig
├── .env.example
├── .gitignore
├── requirements.txt
├── course/
├── docs/
│   ├── history/
│   ├── prompts/
│   ├── progress/
│   ├── roadmap/
│   ├── setup/
│   └── standards/
├── shared/
├── scripts/
└── templates/
```

### `course/`
Keep learning artifacts here, grouped by roadmap phase. Every phase has a stable folder; create a topic folder only when you actually begin that topic.

### `docs/`
Keep course documentation, standards, prompt templates, roadmap state, shared repository history, and your progress records here. Do not duplicate these documents inside individual phases.

`docs/history/` belongs to the shared course repository and is maintained through `main`:

- `repository-change-log.md` — append-only course/repository maintenance history;
- `repository-issues-and-resolutions.md` — append-only course/repository troubleshooting history.

Keep `docs/progress/` on your progress branch:

- `current-learning-status.md` — your current position and next step;
- `learning-log.md` — append-only chronological record of material learning actions;
- `issues-and-resolutions.md` — your append-only troubleshooting history.

Keeping `history/` separate from `progress/` prevents routine `main` updates from colliding with your append-only personal records.

### `shared/`
Contains only assets that are genuinely reused across multiple phases or projects. Topic-specific code, data, and notebooks stay with the topic or project that owns them.

### `scripts/`
Reserved for repository-level utilities. Do not put lesson code here.

### `templates/`
Contains copyable starting structures for topics, exercises, and projects.

## 3. Phase Structure

Phase folders use this naming format:

```text
phase-NN-short-description/
```

Examples:

```text
phase-00-learning-environment-and-foundations/
phase-04-classical-machine-learning/
phase-19-oci-generative-ai/
```

Every phase folder contains a `README.md` that records phase status and points back to the master roadmap. Topic folders are created as they are started, using:

```text
NN-MM-topic-name/
```

Example:

```text
course/
└── phase-01-python-for-data-science-and-ai/
    └── 01-03-numpy/
        ├── README.md
        ├── notes.md
        ├── references.md
        ├── exercises/
        ├── notebooks/
        └── projects/
```

Do not create a folder for every checkbox in the roadmap. A topic folder represents a roadmap subsection; individual checklist items are tracked in that topic's `README.md` and in the master roadmap.

## 4. Topic Structure

A topic starts from `templates/topic/`.

Required files:

- `README.md` — scope, checklist, prerequisites, completion evidence, and status.
- `notes.md` — durable conceptual notes written for later review.
- `references.md` — authoritative references used during learning.

Optional folders are created only when needed:

- `exercises/` — focused practice tasks and solutions after an attempt.
- `notebooks/` — interactive exploration where notebook execution adds value.
- `projects/` — topic-level projects that are larger than a single exercise.
- `data/` — topic-owned data when a project or exercise requires it.
- `src/` — reusable Python code when the topic has moved beyond isolated scripts/notebooks.
- `tests/` — tests for reusable code.

## 5. Exercise Structure

Each non-trivial exercise gets its own folder:

```text
exercises/
└── exercise-01-short-name/
    ├── README.md
    ├── solution.py
    └── test_solution.py
```

For notebook exercises, use `solution.ipynb` instead of `solution.py` when interactivity is part of the learning objective.

Do not generate a completed solution before you have attempted the exercise unless you explicitly ask for a worked solution.

## 6. Project Structure

Projects start from `templates/project/` and should be self-contained:

```text
project-name/
├── README.md
├── references.md
├── requirements.txt
├── data/
│   ├── raw/
│   ├── processed/
│   └── sample/
├── notebooks/
├── src/
├── tests/
├── models/
└── outputs/
```

Rules:

- Small, legal-to-redistribute sample data may be committed under `data/sample/`.
- Raw or large datasets are not committed by default.
- Generated model files are not committed by default.
- Generated outputs are not committed by default unless they are small, intentional evidence required by the lesson/project.
- A project becomes an installable Python package only when the course reaches packaging/application architecture or when package structure is itself relevant to the learning objective.
- When packaging is appropriate, prefer a modern `pyproject.toml`-based package structure and a `src/` layout for distributable code.

## 7. Notebook Standards

Notebook names use a numeric execution/reading prefix:

```text
01-introduction.ipynb
02-experiment.ipynb
03-evaluation.ipynb
```

A notebook is considered reproducible only when:

1. Its kernel can be restarted.
2. The notebook can be run from the first cell to the last cell in order.
3. Required data/dependencies are documented.
4. The result does not depend on hidden state from earlier interactive work.

Use notebooks for exploration, visualization, mathematical walkthroughs, and interactive experiments. Move reusable application logic into `.py` modules once the logic has stabilized.

## 8. Python Naming Standards

- Directories and non-Python files: lowercase kebab-case.
- Python modules: lowercase snake_case.
- Python packages: lowercase snake_case, preferably short and descriptive.
- Test modules: `test_<subject>.py`.
- Notebook files: numeric prefix plus lowercase kebab-case.
- Constants, classes, functions, and variables follow normal Python/PEP 8 conventions when those conventions are introduced in the course.
- `README.md` and `LICENSE` are intentional naming exceptions.

Avoid spaces, platform-specific characters, and decorative Unicode punctuation in file and folder names.

## 9. Environment and Dependency Standards

- Use one repository-local `.venv` for shared course tooling while learning ordinary Python/pip workflows.
- Never commit `.venv/`.
- Use project-specific environments when a project needs dependencies that should not affect the shared learning environment.
- Use Conda when the roadmap is explicitly teaching Conda or when an OCI/scientific/GPU environment genuinely requires it; do not introduce Conda merely as a second way to do the same beginner task.
- Root `requirements.txt` is reserved for shared course tooling only.
- A standalone project owns its own dependency declaration.
- Introduce `pyproject.toml` when packaging or a production-style application makes it appropriate rather than forcing package metadata onto simple lesson folders.

## 10. Secrets and Public-Repository Safety

- Never commit passwords, tokens, OCI credentials, API keys, private keys, connection strings, or sensitive personal data.
- Store local secrets in environment variables or `.env` files that are ignored by Git.
- Commit `.env.example` with variable names and safe placeholder values only.
- If a secret is accidentally committed, treat it as compromised and rotate/revoke it rather than merely deleting the file from the latest commit.
- Do not commit large generated artifacts merely because the repository is public and convenient to access.
- Before adding third-party material, follow the licensing/provenance rules in `docs/standards/documentation-standard.md`.

## 11. Git and Branch Standards

### 11.1 Shared `main` Branch

`main` represents the latest reusable version of the course, not any individual's learning progress.

Allowed on `main`:

- roadmap and course-scope updates;
- repository standards and templates;
- AI tutor prompts;
- setup instructions;
- corrections to shared course material;
- repository history and repository issue documentation.

Do not put personal exercise answers, notebooks, project implementations, completed checklist state, learning logs, or personal troubleshooting history on `main`.

### 11.2 Initial Baseline Tag

Tag the first published public baseline as:

```text
v0.1.0
```

That tag is immutable and represents the exact starting point used before personal learning begins. Future shared course releases may use later semantic-version tags.

### 11.3 Your Progress Branch

Use a long-lived branch for your own progress:

```text
progress/<learner>
```

Examples:

```text
progress/paul
progress/alice
```

Commit your personal learning evidence there. Never merge that personal progress back into `main`.

When `main` receives a shared course update, merge `main` into your progress branch so you get the update without rewriting your learning history.

### 11.4 Course Maintenance Branches

Shared course changes should normally be made on a temporary branch created from `main`:

```text
course/<short-description>
```

After review, merge the change into `main`, update the repository history, and then bring the updated `main` into any progress branches that need the change.

If you discover a shared-course defect while working on `progress/<learner>`, record how it affected your work there. Make the reusable correction from `main` through a `course/<short-description>` branch instead of merging personal progress into `main`.

### 11.5 Temporary Work Branches

For isolated implementation or experimentation, you can branch from `progress/<learner>` using:

```text
feature/<short-description>
experiment/<short-description>
```

Merge successful work back into your progress branch, not into `main`.

### 11.6 Commit Standards

Commit logical units rather than every keystroke. A useful commit should represent one of the following:

- a completed exercise;
- a completed roadmap item;
- a corrected/refactored implementation;
- a documentation update;
- a phase/project milestone;
- a shared course-maintenance change.

Suggested commit style:

```text
learn: complete numpy broadcasting exercises
docs: record phase 1 progress
fix: correct gradient descent implementation
project: add phase 4 baseline model
course: clarify virtual environment setup
```

Do not commit generated caches, local environments, secrets, large raw datasets, or model binaries unless there is a documented reason.

Repository publication, cloning, or branch creation performed mechanically before the corresponding Git lesson does not constitute evidence that a Git learning objective has been completed. Competency requires later explanation and demonstrated use.

## 12. Process and Issue Traceability

Record each material action in the history that matches the work:

- shared course/repository maintenance on `main` → `docs/history/repository-change-log.md`;
- shared repository maintenance issues on `main` → `docs/history/repository-issues-and-resolutions.md`;
- your learning activity on `progress/<learner>` → `docs/progress/learning-log.md`;
- your learning issues on `progress/<learner>` → `docs/progress/issues-and-resolutions.md`.

Topic/project documents reference issue IDs rather than duplicating full troubleshooting histories. Resolved issues remain in the appropriate log as evidence.

## 13. Licensing

The repository's original content is licensed under the root `LICENSE` file.

Third-party datasets, models, code, images, papers, documentation, or other materials retain their original licenses and terms. Do not assume the repository's MIT License grants permission to redistribute third-party material.

Before committing third-party material, verify that redistribution is allowed and document its provenance/license as required by `docs/standards/documentation-standard.md`. If redistribution rights are unclear or prohibited, commit instructions or retrieval metadata instead of the material itself.

## 14. References

- Python Packaging User Guide — virtual environments: https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/
- Python Packaging User Guide — packaging projects: https://packaging.python.org/en/latest/tutorials/packaging-projects/
- Python Packaging User Guide — `pyproject.toml`: https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
- Jupyter architecture and kernels: https://docs.jupyter.org/en/latest/projects/architecture/content-architecture.html
- GitHub repository best practices: https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories
- GitHub licensing a repository: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository
- GitHub secret-storage guidance: https://docs.github.com/en/get-started/learning-to-code/storing-your-secrets-safely
