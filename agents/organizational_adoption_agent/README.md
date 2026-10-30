# Organizational Adoption Agent

This Assignment 7 specialist evaluates readiness to absorb, govern, and sustain an emerging-technology application. It preserves the common intake and output contracts and does not authorize procurement, legal, security, or production deployment.

## Contents

- `specialist_instructions.md` defines the eight-dimension readiness framework.
- `cases/` holds the primary startup and contrasting established-SaaS scenarios.
- `prompt_packets/` contains packets built by the frozen local tool.
- `responses/` is intentionally empty until structured ChatGPT responses are manually saved and validated.
- `records/` contains the Agent Record and the evidence plan.

## Run workflow

From the repository root, run the existing tools:

```text
python tools/build_prompt.py --agent agents/organizational_adoption_agent --case agents/organizational_adoption_agent/cases/primary.json --out agents/organizational_adoption_agent/prompt_packets/primary_prompt.txt
python tools/build_prompt.py --agent agents/organizational_adoption_agent --case agents/organizational_adoption_agent/cases/contrast_1.json --out agents/organizational_adoption_agent/prompt_packets/contrast_1_prompt.txt
python tools/validate_response.py agents/organizational_adoption_agent/responses/primary_response.json
python tools/validate_response.py agents/organizational_adoption_agent/responses/contrast_1_response.json
```

No response files are included because no separate structured ChatGPT run occurred in this environment. Do not represent the planned test observations as validated results.
