# Wikimedia policy-index working notes

This project will hold public-safe methods and dated discrepancy reports that help maintain the live Meta-Wiki policy index. The reports are working notes, not official policy determinations or a replacement for the index. The project does not edit Wikimedia sites.

## Working boundaries

- Track public-safe code, configuration, tests, prompts (if used), comparison baselines, and dated notes in this repository. Write reports, including work in progress, directly in `reports/` in the active worktree; use Git for their history, without a separate drafts directory.
- Keep raw API responses, request logs, and checkpoints in ignored `cache/` or `runs/` directories in the active worktree. A sibling `policy-index-local/` is not required. Reports must not be ignored.
- Before committing, review staged content. Before pushing any branch to the public GitHub remote, a human checks its diff and history for private or unreviewed material. A pushed branch and its PR are public before merge; `.gitignore` cannot remove an earlier committed file from Git history.
- A complete, reviewed, public-safe baseline will be tracked here when its schema is agreed. Incomplete searches do not advance that baseline. Reports must state scope, coverage, failures, and the distinction between policy changes and catalogue gaps.
- Do not edit any of the following files:
  - README.md
  - CONTRIBUTING.md

## Python environment (Hermes and Codex)

- The committed `.python-version` selects the project Python version. From this worktree, create the ignored local environment with `pyenv exec python -m venv .venv` if it does not exist. If `.python-version` changes, recreate the venv before using it.
- Run project Python commands through `.venv/bin/python` (for example, `.venv/bin/python -m unittest` or `.venv/bin/python script.py`), not bare `python` or `python3`. Hermes and Codex must use the same worktree's `.venv/bin/python`; each separate worktree needs its own venv.
- Check `.venv/bin/python -c 'import sys; print(sys.executable, sys.version)'` when verifying interpreter selection. Install project dependencies into this venv when a dependency manifest exists; do not assume either agent's own runtime packages are project dependencies. Hermes itself and the Codex CLI remain in their existing installations.
