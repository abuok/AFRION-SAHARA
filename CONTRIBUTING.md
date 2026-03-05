# Contributing to AFRION Sahara

Thanks for contributing to **AFRION Sahara**.

AFRION Sahara is being built under a **“hype now, ownership later”** strategy:
- The public repo focuses on benchmarks, tooling, docs, and safe demos.
- Sensitive assets (proprietary data, weights, production infra, secrets) stay out of this repo.

## 1) Before you contribute (required)
### Sign the CLA
All contributions require agreeing to the **Contributor License Agreement (CLA)**:
- See [CLA.md](CLA.md)
- The CLA ensures AFRION can legally **commercialize, sublicense, and relicense** contributions later.

### Confirm you have the right to contribute
Do not submit:
- employer-owned code
- proprietary code from other projects
- any material you are not licensed to contribute

## 2) What we want contributions on (high priority)
- **Sahara Bench v0.1**
  - African language eval sets
  - Code-switching eval sets
  - Grounded QA tasks
  - Scoring harness + leaderboard scripts
- **Data tooling**
  - language ID
  - deduplication
  - cleaning pipelines
  - dataset cards
- **Tokenization research**
  - code-switch aware tokenization experiments
- **Docs**
  - model card templates
  - evaluation methodology docs
  - contribution guides
- **Demos**
  - safe, non-sensitive prototypes that showcase progress

## 3) What NOT to contribute here
- Model weights or checkpoints
- Secrets/keys
- Private datasets or non-public scraped content
- Anything that violates privacy, law, or licensing

If you’re unsure, open a discussion issue first.

## 4) Workflow
### Issues first
- For non-trivial work, open an Issue describing:
  - the problem
  - the approach
  - expected outputs
  - how you’ll test it

### Branches & PRs
- Fork the repo (or create a feature branch if you have access).
- Create a PR against `main`.
- PRs must:
  - clearly describe changes
  - include tests or reproducible checks where applicable
  - reference an Issue

### Reviews
- PRs require review before merging.
- Certain paths may require approval by designated maintainers/owners (see GOV).

## 5) Coding standards (baseline)
**TBD:** exact language/tooling choices for the repo.
Recommended options:
1) Python + Ruff + Pytest
2) Python + Black + Flake8 + Pytest
3) Mixed (Python for data/evals, TypeScript for demos)

Until locked:
- Keep changes small and well-documented.
- Include a simple way to run your work locally (README snippet).
- Prefer deterministic scripts over “magic notebooks.”

## 6) Testing & reproducibility
- If you add evaluation code:
  - provide a small sample dataset or stub
  - document how scores are computed
  - ensure results are reproducible

## 7) Documentation
If you add new features:
- update docs in `README.md` or relevant `/docs` files
- include a short “Why” and “How to use”

## 8) Community expectations
By contributing, you agree to follow:
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

## 9) Help wanted
If you want a place to start:
- Look for Issues labeled: `good first issue`, `help wanted`, `bench`, `data`, `docs`.
