# Promethean Technology Classification Agent

This Lab 4 specialist classifies an emerging technology as Incremental, Breakthrough, Potentially Promethean, or Insufficient Evidence using the Chapter 11 categorical-barrier and cross-tier framework. It preserves the frozen intake/output contracts.

## Package

- `specialist_instructions.md` — governing 10-section specialist logic.
- `cases/primary.json` and `cases/contrast_1.json` — same implantable BCI technology and application; organization changes.
- `responses/primary_v0_1_schema_failure.json` — preserved genuine early schema failure.
- `responses/*_response.json` — revised, schema-valid local response records for review.
- `records/` — Agent Record draft, independent professional judgment draft, and team handoff.

## Reproduce

Run the frozen tools from the scaffold root:

```powershell
python tools/build_prompt.py --agent agents/promethean_classification_agent --case agents/promethean_classification_agent/cases/primary.json --out agents/promethean_classification_agent/prompt_packets/primary_prompt.txt
python tools/build_prompt.py --agent agents/promethean_classification_agent --case agents/promethean_classification_agent/cases/contrast_1.json --out agents/promethean_classification_agent/prompt_packets/contrast_1_prompt.txt
python tools/validate_response.py agents/promethean_classification_agent/responses/primary_response.json
python tools/validate_response.py agents/promethean_classification_agent/responses/contrast_1_response.json
python tools/check_frozen_core.py
```

The prompt packets are ready for an interactive ChatGPT run. The saved revised response records are structured evidence drafts authored in this workspace and schema-validated locally; they are not represented as an independently completed interactive model run.
