# Agentic Systems for Root Cause Analysis: A Survey - Replication Package

This repository is the replication package for the survey paper **"Agentic
Systems for Root Cause Analysis: A Survey"** (Pulagam, Aston, Baysal, and
Shafiq; Carleton University; under submission). It holds the search protocol,
the reviewed corpus, the rating rubric, and the per-system ratings behind the
figures and tables in the paper.

## Summary

Root cause analysis (RCA) in complex software and infrastructure systems has
drawn renewed attention since large language models (LLMs) began to be applied
to the diagnostic task. This survey reviews **30 papers** published between
**January 2023 and April 2026**: 11 multi-agent RCA architectures, 4 generic
multi-agent frameworks retained for context, and 15 single-LLM RCA designs. It
contributes a **10-dimension comparison framework (D1–D10)**, each dimension
rated 0/1/2 and read as a per-system capability *profile* rather than summed
into a score, a taxonomy of four architectural patterns
(function-partitioned, modality-partitioned, hierarchical, decentralized), and
a capability-profile table with deployment maturity (L1–L4) reported on a
separate axis.

## Repository map

| Path | Contents |
|---|---|
| `search/search-query.txt` | The exact Boolean query run against each database. |
| `search/databases.md` | The four databases searched, with URLs and access date. |
| `search/inclusion-exclusion.md` | Inclusion and exclusion criteria. |
| `corpus/corpus.csv` | The 30 reviewed papers: key, system, group, year, pattern, evaluation setting, deployment maturity, DOI, and resolvable URL. |
| `extraction/dimensions-rubric.md` | The D1–D10 rubric with the 0/1/2 thresholds and the L1–L4 maturity levels. |
| `extraction/ratings.csv` | Per-system D1–D10 ratings and deployment maturity for the 13 rated systems. |
| `figures/` | Figures used in the paper. |

## How to reproduce

1. **Search.** Run the query in `search/search-query.txt` against each
   database in `search/databases.md`, restricted to January 2023 – April 2026.
2. **Screen.** Apply the criteria in `search/inclusion-exclusion.md`.
3. **Extract.** For each included paper, record its metadata in
   `corpus/corpus.csv`.
4. **Rate.** Apply the thresholds in `extraction/dimensions-rubric.md` to score
   each rated system on D1–D10. The ratings are in `extraction/ratings.csv`.

The ratings are a **descriptive profile**: they are not summed, averaged, or
ranked. A rating of 0 records that a paper does not report the capability.

> **Note on the single-LLM results.** Where the corpus lists a reported result
> for a single-LLM system, each figure is in that system's own metric, dataset,
> and scale. These values are **not comparable across rows**.


## License

Text and data in this repository are released under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). See `LICENSE`.
