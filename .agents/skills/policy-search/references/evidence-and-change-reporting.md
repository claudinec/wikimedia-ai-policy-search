# Evidence and change-reporting contract

Use with [the general method](policy-search.md) and a topic recipe such as [AI policy search](ai-policy-search.md). This is a field/decision contract for working notes, **not** a claim that a collector or validator already exists. Write dated reports directly in `reports/` in the active worktree, including work in progress; use Git for their history. Keep raw data and request logs in ignored `cache/` or `runs/` directories as specified by `AGENTS.md`. Only public-safe material belongs in Git. A member cloning the project must not need private run data to understand a published note's classifications and coverage.

## Run ledger and candidate evidence

For each run, record a run ID and UTC start/end, question and topic-recipe revision, scope and explicit exclusions, catalogue URL/revision/retrieval time, search routes/terms, tool version if any, and comparison baseline ID/revision. Record per-site family, code, URL, local projectspace namespace, attempted routes, candidate counts, completed/partial/failed state, failure reasons, request/retry counts and verification time. Distinguish an inaccessible site from a searched site with no verified candidates. Never silently omit a site from the denominator.

For each candidate, retain site/family/code, discovered and canonical titles, page ID, namespace, URL and relevant section anchor, redirects/move evidence, discovery route and original query. Verification fields: local status evidence and its revision/link, original-language operative text and precise section, translation aid/uncertainty, current revision ID/timestamp, verification time, page class, inclusion/exclusion reason and reviewer decision. Record exact catalogue page/section match or gap, with catalogue revision; an ambiguous match stays unresolved. An unavailable page or failed request remains unverified. Provide a direct URL and revision/diff for every public headline claim. Link named categories and templates to their local wiki pages, displaying template calls as inline code. Public-safe excerpts must be minimal and checked before committing; keep full raw responses outside Git.

A stable identity is **site plus page ID** when available, with one or more section-level provision keys; also keep discovered title, current canonical title and move history. When page IDs or anchors cannot be resolved, record an unresolved identity rather than assuming a deletion or match from similar titles. The same rule found by two search routes is one inventory item with both routes; distinct operative sections must remain distinguishable.

## Independent comparisons

1. **Local-rule inventory:** compare accepted, directly verified entries against the previous accepted complete baseline. Material policy changes are adoption, substantive amendment of operative wording, repeal, or formal status change—each supported by dated before/after page or revision evidence. Track newly discovered **older** rules, page moves, cosmetic revisions, and unresolved or failed checks separately. Revision churn is not automatically an operative change.
2. **Meta catalogue:** compare the locally verified qualifying page *and relevant section* with the retrieved catalogue revision. Distinguish a new gap, continuing gap, gap now covered, ambiguous match and catalogue removal. A catalogue addition is not local adoption; removal is not repeal. Keep this comparison independent of inventory changes, including when the same rule appears in both.
3. **Other page classes:** compare non-binding guidance and proposals separately from adopted policies/guidelines. A proposal becoming adopted is a status change only after verification on the relevant local page. Do not silently merge a watchlist into the policy-change count.

Only an explicitly accepted, complete run may replace the complete comparison baseline. A partial run may produce a qualified working note but cannot turn absent checks into removals or advance the complete baseline. Keep the accepted baseline reviewed and public-safe in the project repository; if a necessary field cannot safely be committed, decide a reduced schema and backup/recovery plan **before** claiming a portable baseline. Do not infer acceptance merely from a Git commit or PR merge.

## Dated working-note outline

- Date, run and baseline IDs, scope/time boundary, methods/recipe version, catalogue revision, and a prominent *working notes—not an official index* label.
- Per-family/site coverage: enumerated, attempted, completed, partial, failed, with limitations and actual request totals.
- Adopted rules: verified new adoption, substantive amendment, repeal or status change, with original title, URL/anchor, status evidence, short explanation and previous/current revisions.
- Catalogue gaps: new, continuing (compact appendix), now covered, and uncertain matches; do not mix these with policy changes.
- Non-binding guidance and proposals: distinct labelled sections. Other events: newly discovered older rules, moves and cosmetic changes.
- Review queue: uncertain translations/status, unverified candidates, errors and outstanding checks—never presented as verified findings.
- When justified by completed coverage: “No verified material changes found in the stated scope”; mention any separate catalogue/guidance developments. A failed or materially partial run must not be announced as “No changes found.”

Before exposing a branch or PR, a human reviews the sanitized report and the branch's **entire diff and history**; public Git history cannot be made private by adding `.gitignore`. An open PR is already public. Publication of working notes does not edit the Meta-Wiki catalogue. A Discord heartbeat or report link, if later approved, is an independent action with its own review and deduplication gate.
