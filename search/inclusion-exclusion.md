# Inclusion and exclusion criteria

The search process and criteria follow He et al. (2025), adapted for RCA.

## Inclusion criteria

A paper is included if **all** of the following hold:

- It is written in English.
- It has an accessible full text.
- It describes multi-agent systems, or LLM-based systems for RCA.

## Exclusion criteria

A paper is excluded if **any** of the following hold:

- It has fewer than 5 pages.
- It is a duplicate, or a similar study by the same authors.
- It is a book, keynote record, panel summary, technical report, thesis,
  tool-demo paper, or editorial.
- It is a literature review or survey.
- It was published before January 2023.
- It does not involve AIOps.

## Multi-agent inclusion boundary

A system is classified as **multi-agent** when (i) it instantiates two or more
distinct agent roles with separate prompt contexts, tool access, or model
backbones, and (ii) the agents exchange information during a single RCA
episode. Systems with one LLM and chained prompt templates are placed in the
single-LLM category. Where a system's classification was ambiguous, it was
resolved by consensus between the coders.
