# Wikimedia AI policy index -- working notes

This repository is used by members of various Wikimedia AI Cleanup projects to maintain the [global index of AI policies](https://meta.wikimedia.org/wiki/Artificial_intelligence/Policies_by_project).

## Methods

[TODO]

## Instructions

Automated requests to Wikimedia sites or APIs must have a valid User-Agent string to comply with the Wikimedia Foundation's [User-Agent policy](https://foundation.wikimedia.org/wiki/Policy:Wikimedia_Foundation_User-Agent_Policy). An agent can be instructed to use the environment variable `WIKIMEDIA_OPERATOR_CONTACT` to build a User-Agent string. The convention for Wikimedia sites is to use the format `<project>; User:<name>` (e.g.  `wikipedia:en; User:Example`) for contact information.

## Contributing

[use one of the standard GitHub templates?]

## AI disclosure

AI agents may be used to search Wikimedia projects for policies and discussions that have not been listed in the index [or added to Wikidata]. The September 2026 searches were conducted using the following tools:

- Harness: Hermes Agent
- Model: GPT-5.6 Sol
- Kagi API (search and extraction)
- [Prompts](/prompts/find-index-omissions.md)
