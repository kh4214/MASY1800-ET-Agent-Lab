# Assignment 7 Testing and Revision Evidence Plan

## Current implementation status

The specialist instructions and two complete common-intake cases are prepared. Prompt packets must be submitted through the supported ChatGPT workflow and the returned JSON saved under `responses/` before response validation or result claims can be made.

## Required test comparison

Hold constant: generative AI for first-line SaaS customer-support automation, with human escalation for consequential inquiries.

Primary context: a small startup with limited runway, a small engineering team, existing support staff, and unknown governance, baseline, ownership, and employee-readiness evidence.

Contrast context: a larger SaaS organization with stronger infrastructure and financial capacity, formal governance, established support/training processes, and dedicated operational ownership; material control details remain unknown.

Expected sensitivity to verify, not a result: the technology/application finding may remain similar, while the larger organization may be able to consider a more advanced staged path because it has named readiness strengths. The startup should not receive a scale-up recommendation without filling its more consequential readiness gaps.

## Required missing-information test

For both cases, ask for evidence of the current support-quality baseline and the effectiveness/design of human escalation for consequential inquiries. These facts determine whether the organization can measure quality degradation and safely control higher-consequence responses. The agent must not invent them.

## Weakness to test and possible revision

Test whether the first version merely lists all eight dimensions and gives both organizations the same generic checklist. If so, revise the instructions to require: (a) ranking gaps by consequence and feasibility, (b) a named most-consequential gap, (c) owner assignment only when supported, and (d) a clear distinction between pilot and scale readiness. The present instructions include those constraints, but they still need execution evidence from actual responses.

## Manual completion log

- [ ] Save primary JSON-only response.
- [ ] Validate primary response with `tools/validate_response.py`.
- [ ] Save contrast JSON-only response.
- [ ] Validate contrast response.
- [ ] Compare stable and changed conclusions.
- [ ] Record the observed weakness, revision, and retest result.
- [ ] Add the actual validation output and response filenames to the Agent Record.
