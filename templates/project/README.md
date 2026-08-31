# Project Title

## Roadmap Scope

State the phase/project and competencies this project validates.

## Problem

Define the problem before choosing libraries, models, or OCI services.

## Success Criteria

Define measurable success criteria.

## Structure

- `data/raw/` — local/raw data, normally not committed.
- `data/processed/` — generated intermediate data, normally not committed.
- `data/sample/` — small redistributable fixtures/sample data that may be committed.
- `notebooks/` — exploration and experiments.
- `src/` — reusable implementation.
- `tests/` — automated tests.
- `models/` — generated model artifacts, normally not committed.
- `outputs/` — generated reports/plots/results, committed only when intentionally required.

## Setup

Document environment and dependencies.

## Data Provenance

Document where data came from and any usage/licensing constraints.

## Evaluation

Document metrics, baselines, experiment conditions, and results.

## Known Limitations

Record limitations explicitly.

## Issues / Troubleshooting

Reference relevant `LEARN-ISSUE-NNNN` records from `docs/progress/issues-and-resolutions.md`. Keep the full diagnosis/resolution history in the canonical learner issue log unless a project-specific technical document genuinely needs additional detail.

## Verification / Reproducibility

Record the final checks used to confirm the project behaves as documented.

## References

See `references.md`.
