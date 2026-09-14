# Public boundary

## Safe to publish

- product purpose and problem domain;
- high-level architecture;
- capability summaries;
- safety principles and deliberate exclusions;
- roadmap milestone state;
- sanitized validation facts;
- operating-system and toolchain versions when they describe a deliberately public experimental validation environment without identifying a machine or user;
- fictional examples;
- public-safe diagrams;
- deliberately prepared screenshots;
- explicit limitations and not-yet-proven claims.

## Keep private

- private source code;
- real machine reports;
- usernames, hostnames and environment identities;
- IP addresses, gateways and real network topology;
- hardware serials and device identifiers;
- credentials, API keys, tokens and local runtime secrets;
- exact local secret/runtime locations;
- operational logs containing machine-specific evidence;
- quarantine, backup and restoration artifacts;
- private deployment configuration;
- internal continuity checkpoints, pointers and reports;
- local filesystem paths not required to explain the public product;
- procedures or implementation detail that would weaken safety gates.

## Evidence classes

Public wording should keep four classes separate:

```text
PROVEN / RECORDED
implemented behavior or validation supported by current source evidence

HISTORICAL / SUPERSEDED
older source documentation retained as provenance but not current operational truth

PLANNED
roadmap capability not yet established as current behavior

NOT PROVEN
claim that available evidence does not establish
```

A project name, roadmap item or historical document must not silently promote a planned or superseded state into current fact.

## Stale documentation rule

The private source contains historical documents from earlier synchronization and bootstrap phases.

Public material follows the current documented product state and live repository baseline. Historical synchronization descriptions are provenance, not authority for present operational claims.

## Validation rule

A successful recorded build or smoke-test run may be published as bounded evidence.

It must not be expanded into claims of:

- universal Windows compatibility;
- production certification;
- complete hardware/OEM coverage;
- production remote readiness;
- broad WinPE hardware validation.

## Privacy principle

When evidence comes from a real diagnostic run, recreate public examples with fictional values rather than masking and reusing operational data.
