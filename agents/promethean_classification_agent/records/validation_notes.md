# Validation Notes

- `tools/validate_response.py` passed the revised primary and contrast records.
- `tools/check_frozen_core.py` reported `FROZEN CORE INTACT`.
- The frozen output schema sets `additionalProperties` to `false`. Directly comparing response keys with `core/output_schema.json` showed that the preserved v0.1 record has the unsupported `promethean_criteria` field, while both v0.2 records have no unsupported top-level fields.
- The bundled Python environment does not include `jsonschema`; no package was installed and no frozen file was altered. The direct check complements, rather than replaces, the provided validator.
