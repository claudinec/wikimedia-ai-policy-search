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
