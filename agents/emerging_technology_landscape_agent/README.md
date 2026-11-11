# Emerging Technology Landscape Agent

Specialist for current, dated technology-landscape assessment and management monitoring.

## Files

- `specialist_instructions.md` - decision rules and boundaries.
- `cases/primary.json` - 1,000-employee SaaS company case.
- `cases/contrast_1.json` - 4-person software startup contrast.
- `records/dated_evidence_source_register.md` - source portfolio and limitations.
- `records/monitoring_trigger_structure.md` - default monitoring design.
- `records/agent_record.md` - assignment record and known limitations.

## Next required workflow

Build the two prompt packets with `tools/build_prompt.py`, run them in the established ChatGPT workflow, save only actual JSON responses, then validate them with `tools/validate_response.py`. No response files are included yet.
