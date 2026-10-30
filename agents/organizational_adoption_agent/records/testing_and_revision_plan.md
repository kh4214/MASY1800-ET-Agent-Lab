# Assignment 7 Testing and Revision Evidence Plan

## Execution status

The prepared prompt packets were executed through the available LLM capability. Initial primary and contrast responses are preserved as `primary_response_v0_1.json` and `contrast_1_response_v0_1.json`. The revised agent was rerun; final responses are `primary_response.json` and `contrast_1_response.json`.

## Required test comparison

Hold constant: generative AI for first-line SaaS customer-support automation, with human escalation for consequential inquiries.

Primary context: a small startup with limited runway, a small engineering team, existing support staff, and unknown governance, baseline, ownership, and employee-readiness evidence.

Contrast context: a larger SaaS organization with stronger infrastructure and financial capacity, formal governance, established support/training processes, and dedicated operational ownership; material control details remain unknown.

Observed stable conclusion: both responses keep Chapter 8's general Leading Edge maturity context separate from organizational readiness, and require a human-escalation design and support baseline for consequence-sensitive inquiries.

Observed changed conclusion after revision: the startup receives readiness-building before a pilot because several stage gates are unknown or absent; the established organization receives a conditional low-consequence pilot because governance and ongoing ownership are stated. Neither receives a scale-up recommendation.

## Required missing-information test

For both cases, ask for evidence of the current support-quality baseline and the effectiveness/design of human escalation for consequential inquiries. These facts determine whether the organization can measure quality degradation and safely control higher-consequence responses. The agent must not invent them.

## Observed weakness and revision

The initial outputs gave both organizations the same "conditional pilot" action. Although each mentioned different capabilities, the action did not distinguish the startup's missing baseline, owner, escalation design, and capacity from the larger organization's stated governance and ownership. This weakened context sensitivity.

Revision: Added a stage-gate rule requiring a relevant baseline, accountable owner, low-consequence scope, escalation/control design, and observation capacity before a pilot. The revision requires readiness-building when several gates are unknown/absent, conditional pilot when they are substantially present but unproven, and evidence of a controlled learning stage before staged implementation. It also requires the single stage-gating difference to be named in comparisons.

Retest result: the final responses differ appropriately: readiness-building for the startup and conditional pilot for the established organization.

## Completion log

- [x] Save initial and final primary JSON-only responses.
- [x] Save initial and final contrast JSON-only responses.
- [x] Run the frozen response validator on all four responses.
- [x] Compare stable and changed conclusions.
- [x] Record the observed weakness, revision, and retest result.
- [x] Update the Agent Record with actual response filenames and validation status.
