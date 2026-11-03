# Search scope comparison — 3 November 2026

Working notes for scope selection. This compares the November pilot’s searched sites with size rankings; it is not a new policy search or an accepted policy baseline.

## Answer

After excluding Incubator and Wikifunctions from the 20 live pilot sites, 18 sites remain. Abstract Wikipedia was not searched in that pilot and is also excluded going forward. Closed English Wikinews remains outside the live-site scope.

Only nine of the 18 retained pilot sites are in the top 100. A strict size cutoff must extend to **rank 697** to include all 18: Beta Wikiversity is the limiting site. A rounded top-700 cutoff would therefore suffice for this snapshot. Without Beta Wikiversity, the cutoff would be rank 355 (French Wikiquote).

## Pilot sites outside the top 100

| Site | Live Wikistats rank | Meta-copy rank |
| --- | ---: | ---: |
| [Meta-Wiki](https://meta.wikimedia.org) | 113 | 113 |
| [English Wikibooks](https://en.wikibooks.org) | 142 | 142 |
| [English Wikiquote](https://en.wikiquote.org) | 165 | 165 |
| [Multilingual Wikisource](https://wikisource.org) | 174 | 174 |
| [English Wikiversity](https://en.wikiversity.org) | 216 | 216 |
| [English Wikivoyage](https://en.wikivoyage.org) | 221 | 221 |
| [German Wikivoyage](https://de.wikivoyage.org) | 276 | 276 |
| [French Wikiquote](https://fr.wikiquote.org) | 355 | 355 |
| [Beta Wikiversity](https://beta.wikiversity.org) | 697 | 697 |

The nine already inside the top 100 are Commons (1), Wikidata (2), English Wiktionary (3), Polish Wikipedia (19), Chinese Wikipedia (22), Portuguese Wikipedia (32), English Wikisource (33), Wikispecies (38) and French Wikisource (48).

## Metric and sources

The supplied ranking orders sites by the **Good content-page count**, descending. This is not a ranking by storage bytes, active editors or relevance to AI-policy work. The displayed counts are family-specific content counts, so they include items such as Wikidata entities and Commons media.

- [Live top 100](https://wikistats.wmcloud.org/wikimedias_html.php?s=good_desc&th=0&lines=100).
- [Live top 1000, used to locate the pilot sites below the cutoff](https://wikistats.wmcloud.org/wikimedias_html.php?s=good_desc&th=0&lines=1000).
- [Meta’s list of Wikimedia projects by size](https://meta.wikimedia.org/wiki/List_of_Wikimedia_projects_by_size). The directly retrieved copy had mostly 1–2 November data; the live ranking mostly 2–3 November data. The ranks of all 18 retained pilot sites agree between these snapshots.
- [Named special-project table](https://wikistats.wmcloud.org/display.php?t=wx), used to resolve the aggregate table’s malformed Wikidata label by matching its Good/total/edit counts exactly.
- [Wikisource-family table](https://wikistats.wmcloud.org/display.php?t=ws) identifies the multilingual portal as `mul.wikisource.org`. Its redirect to `wikisource.org` was checked, so it was matched to the pilot’s `sourceswiki` site rather than treated as a different wiki.

The comparison uses the saved per-site coverage ledger from the 1 November pilot, not every historical September search. The first 100 rows were checked against the first 100 of the extended table; names/aliases were resolved before matching, and rank/coverage arithmetic was checked. Raw snapshots, the comparison script and machine-readable result are retained in ignored `runs/2026-11-03-scope-comparison/`.

## Current scope — agreed 3 November 2026

**Top 100 plus the nine named exceptions above** is the agreed scope for now. It retains all 18 pilot sites with 109 candidate sites in this snapshot. Deduplicate sites and exclude closed/private sites, Incubator, Wikifunctions and Abstract Wikipedia. Record the ranking date and selected sites for each run. Meta-Wiki is needed as the index reference regardless of whether its own local pages are discovery targets.

The recipe now records the explicit exclusions of Incubator, Wikifunctions and Abstract Wikipedia. It also records the goal of identifying appropriate Wikidata items and proposed additions for human review. Historical pilot findings and coverage have not been rewritten to apply the new scope retroactively. No Wikimedia edits, schedule, commits or pushes were performed.
