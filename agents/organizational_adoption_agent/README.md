# Organizational Adoption Agent

This Assignment 7 specialist evaluates readiness to absorb, govern, and sustain an emerging-technology application. It preserves the common intake and output contracts and does not authorize procurement, legal, security, or production deployment.

## Contents

- `specialist_instructions.md` defines the eight-dimension readiness framework.
- `cases/` holds the primary startup and contrasting established-SaaS scenarios.
- `prompt_packets/` contains packets built by the frozen local tool.
- `responses/` preserves initial and revised primary/contrast structured responses; all four pass the frozen response validator.
- `records/` contains the template-based Agent Record, testing/revision evidence, and the approved Self-Reflection.

## Run workflow

From the repository root, run the existing tools:

```text
python tools/build_prompt.py --agent agents/organizational_adoption_agent --case agents/organizational_adoption_agent/cases/primary.json --out agents/organizational_adoption_agent/prompt_packets/primary_prompt.txt
python tools/build_prompt.py --agent agents/organizational_adoption_agent --case agents/organizational_adoption_agent/cases/contrast_1.json --out agents/organizational_adoption_agent/prompt_packets/contrast_1_prompt.txt
python tools/validate_response.py agents/organizational_adoption_agent/responses/primary_response.json
python tools/validate_response.py agents/organizational_adoption_agent/responses/contrast_1_response.json
```

The saved response files document the initial contrast weakness and the revised rerun. They are local model-execution evidence for this course workflow; case facts remain labeled assumptions and provider-specific claims remain unverified.
