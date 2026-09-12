# Screenshot publication policy

WinDiag screenshots can expose unusually sensitive machine information and therefore require deliberate sanitization.

## Preferred source

Use a demonstration machine or recreated interface populated with fictional/non-sensitive values.

## Reject a screenshot if it contains

- real usernames or machine names;
- real IP addresses, gateways or DNS configuration;
- hardware serial numbers or unique device identifiers;
- storage identifiers or volume details tied to a real machine;
- credentials, API keys or tokens;
- real event-log contents;
- operational filesystem paths;
- installed-software or service details that should remain private;
- real quarantine, backup or repair receipts;
- private logs or internal checkpoints;
- unrelated windows, notifications or browser tabs.

## Rule

Do not treat blur as the preferred sanitization method. Recreate the demonstration with fictional values whenever possible.

A screenshot is not automatically public-safe merely because it shows read-only diagnostics.
