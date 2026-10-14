# Rating rubric (D1–D10)

Each system is characterized along ten dimensions. Each dimension is rated
**0** (absent or minimal), **1** (present in basic form), or **2** (advanced
or validated). The ten ratings are read together as a **per-system profile**.
They are not summed, averaged, or ranked. A rating of 0 records that a paper
does not report the capability.

| Dim | Name | 0 (absent/minimal) | 1 (basic) | 2 (advanced/validated) |
|---|---|---|---|---|
| D1 | Agent architecture | Single agent: one LLM, with or without tools | Role split: two or more agent roles serving one pipeline | Backbone-matched: roles with distinct model backbones matched to their subtask |
| D2 | Orchestration | None: no coordination described | Fixed: same order for every incident | Adaptive: plan adapts to the incident's characteristics |
| D3 | Reasoning paradigm | Direct: zero/few-shot, no intermediate reasoning | Ungrounded chain: CoT-style steps without external grounding | Grounded: reasoning grounded in evidence gathered during the episode (ReAct, TAO, MCTS, KG Five-Whys) |
| D4 | Data modality | Single: one modality | Two modalities, or several sources of one structural type | Multi-modal: three or more qualitatively different modalities |
| D5 | Tool integration | None: no external access during diagnosis | Dynamic-read: retrieval or read access | Dynamic-act: acts on external systems with a safety check |
| D6 | Explainability | None: no structured artifact | Produced: reasoning trace or graph delivered | Validated: artifact's faithfulness to the reasoning is checked |
| D7 | Bias and evaluation coverage | Closed: single proprietary dataset, no independent check | Single-domain: public benchmark(s) from one domain, or proprietary data with human-readable evaluation | Cross-domain: two or more qualitatively different domains |
| D8 | Human-in-the-loop | Autonomous: no defined human role | Advisory: review of outputs or authoring of inputs | Approval-gated: human approval before actions take effect |
| D9 | Context sustainability | None: no compression or cross-episode memory | Single mechanism (memory, summarization, or reflection) | Combined: two or more mechanisms together |
| D10 | Decision synthesis | Passthrough: a single agent's conclusion passes through | Arbitrated: master veto or arbitration by a designated agent | Consensus: formally specified negotiation or consensus protocol |

## Deployment maturity (separate axis)

Deployment maturity is recorded separately from the ten dimensions, because
whether a system is deployed reflects organizational factors external to its
technical design.

| Level | Meaning |
|---|---|
| L1 | Prototype |
| L2 | Real-data validation |
| L3 | Production deployed |
| L4 | Cross-organization |
