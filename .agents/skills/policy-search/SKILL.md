---
name: policy-search
description: Research and compare Wikimedia policy rules across wikis.
version: 0.1.0
author: Claudine Chionh and Hermes Agent
license: CC-BY-SA-4.0 OR GFDL-1.3-no-invariants-or-later
---

# Cross-wiki policy search

Use this skill for read-only discovery, verification and comparison of policy or guideline provisions across Wikimedia projects. For AI/LLM rules, apply the [AI topic recipe](references/ai-policy-search.md). The [general method](references/policy-search.md) and [evidence/change-reporting contract](references/evidence-and-change-reporting.md) specify the detailed procedure and record fields. These are project-local instructions usable with a person or any harness; do not assume Hermes profiles or private integrations.

## Procedure

1. Define the question, included/excluded families and page classes, time window, catalogue, coverage standard and reviewer **before** collecting. Record whether the run is a baseline, broad search or limited recheck. No recurrence, publication, wiki edit or message is implied by permission to research.
2. Enumerate the approved live sites from SiteMatrix, including special projects as appropriate; record exclusions. Resolve each site's local search namespaces. Search multilingual terms, local rule indexes and secondary discovery routes, preserving the routes actually used and all incomplete sites.
3. Verify each lead directly on its own wiki: canonical page and section, revision, status evidence and original-language operative wording. A snippet, copied passage or Meta catalogue listing cannot establish adoption. Keep uncertain translations and proposals outside the adopted-rule list.
4. Compare verified site/page/section identities with the previous accepted baseline **separately** from matching the current catalogue. Distinguish new adoption, substantive amendment, repeal and status change from moves, older discoveries, catalogue gaps and cosmetic edits. Do not infer a repeal from a retrieval failure.
5. Write a dated, coverage-labelled, evidence-linked working note directly in `reports/` in the active worktree, including work in progress. A partial run cannot advance a complete baseline or support an unqualified “no changes” claim. Human review precedes public sharing, wiki edits or notifications.

## Boundaries

Follow the repository `AGENTS.md` for report and raw-output storage; do not edit `README.md` or `CONTRIBUTING.md`. Do not use browser credentials or authenticated wiki sessions. A public branch or PR is already public before merge. No collector or validator is included in this skill yet; do not claim automated coverage or a complete baseline.
