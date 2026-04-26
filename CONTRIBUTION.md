# Contributing to AI Agent Playbook

Welcome — this repository collects AI agent projects, templates, demos, and integrations across every major framework and industry. Thank you for helping grow a practical, reproducible, and responsible catalog of agent work.

## Quick summary
- Add small, runnable, well-documented agent examples and templates.
- Prefer reproducible demos and small checkpoints or external download scripts.
- Follow the folder schema and metadata so projects are discoverable and automatable.
- Pay attention to license, data provenance, and ethical/safety notes.

---

## What to contribute
- New agent projects (single- or multi-agent; code, notebooks, or demos).
- Templates/boilerplates for agent types (reactive, planning-based, learning agents, RL, LLM-based, etc.).
- Integrations (environments, simulators, observability / logging tools).
- Shared tooling (evaluation harnesses, metrics, benchmark suites, dataset loaders).
- Docs, reproducible experiments, visualization utilities, or lightweight datasets (or links to them).

If your contribution is large (new category, many projects, major refactor) please open an issue first to coordinate placement and naming.

---

## Project folder requirements (must-have)
Each agent project added must include the following at the top level of its folder:

- `README.md` — concise description, intended use-case, quick start with exact commands, expected output, and runtime.
- `LICENSE` or a note referencing repository root LICENSE.
- `requirements.txt`, `pyproject.toml`, or `environment.yml` (pin critical dependency versions).
- One or more runnable examples (script or notebook) that reproduce the core behavior.
- `tests/` or a smoke-test script with instructions to run them.
- `metadata.yaml` (see example below).

### Example metadata schema
```yaml
title: quick-chatbot-agent
author: Your Name <you@example.com>
language: python
tags:
  - llm
  - agent
  - rl
license: MIT
datasets:
  - name: example-dialogs
    url: https://...
entrypoint: run_demo.py
requirements: requirements.txt
```

---

## Naming & layout conventions
- Folder names: lowercase, hyphen-separated (e.g., `multi-agent-pursuit`).
- Place one logical project per folder.
- Keep demos and notebooks near the code.
- Avoid committing large binaries.

---

## Reproducibility & experiments
- Include seed values, environment variables, and exact dependency versions.
- Provide a minimal run command and expected output sample.
- For stochastic experiments, include evaluation scripts and deterministic seeds or checkpoints.

---

## Models, datasets & large files policy
- Don't add large datasets or model checkpoints directly. Instead provide a download script.
- Clearly state dataset licenses, attribution, and any usage restrictions.

---

## Code style & tests
- Python: follow PEP 8.
- Document complex algorithms with short docstrings and references.
- Add unit or integration tests when possible.

---

## PR process and checklist
Before opening a PR:
- [ ] Fork and create a branch: `feat/<short-desc>` or `fix/<short-desc>`
- [ ] Update README and metadata
- [ ] Include tests or a smoke-test demonstration
- [ ] Ensure no secrets or private data are included
- [ ] Confirm license compatibility for added assets

---

## Ethics, fairness & safety
- Include an explicit "Ethical considerations" section in the README if the agent interacts with people or processes personal data.
- State potential biases, failure modes, and appropriate usage guidance.
- Prefer human-in-the-loop defaults for high-risk demos.

---

## Code of Conduct
By contributing, you agree to be respectful, constructive, and collaborative.

---

Thank you for contributing to AI Agent Playbook — maintained by [Mahip Kakan](https://github.com/mahip-kakan).
