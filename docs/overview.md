# Overview

MLI-Knot-WinDiag is a Windows diagnosis, controlled-maintenance and recovery platform built around conservative operational boundaries.

## Product shape

The private `0.1.0` baseline contains four main implementation surfaces:

- `Core`: domain models, orchestration and safety rules;
- `Windows`: collectors, cleanup, Registry, update discovery and reports;
- `App`: local API, asynchronous diagnostic jobs and browser dashboard;
- `CLI`: command-line and WinPE-oriented execution.

The repository also contains WinPE builder assets and offline diagnostic tooling.

## Implemented baseline capabilities

The current source represents:

- local diagnostic orchestration;
- system, hardware, storage, network, service, event, policy, Registry, driver and firmware inventory;
- local API and browser dashboard;
- CLI operation;
- JSON and HTML reporting;
- asynchronous jobs with progress polling;
- cleanup preview, dry-run, quarantine, receipts and restoration;
- reversible startup-Registry remediation;
- driver/firmware inventory and Windows Update discovery;
- WinPE-oriented recovery tooling;
- remote-ready architecture that remains local-only and disabled by default in the initial configuration.

## Recorded Windows validation

The source documentation records a Windows validation checkpoint where:

- the solution compiled in Release;
- Core, Windows, CLI, App and SmokeTests compiled;
- smoke tests passed;
- structural auditing passed for the recorded checkpoint;
- the local `.NET` resolver was validated;
- automatic build/test logging was functioning in the recorded checkpoint.

Separately, the current source changelog records the later correction that made the build/test scripts preserve complete native command output in addition to PowerShell messages.

The recorded experimental environment was Windows 10 Pro 22H2 x64 with PowerShell 5.1 and .NET SDK 10.0.302.

This is evidence of baseline operability in that environment, not a claim of production certification or universal platform support.

## Safety architecture

The product separates observation from mutation.

Its documented principles include reading before writing, preview before maintenance, backup/reversibility where supported, quarantine or disable instead of blind deletion, and validation after changes.

Remote operation is an architectural direction rather than a current production-readiness claim. Non-local operation requires additional transport, authentication, authorization, audit and recovery gates.

## Public interpretation

This showcase documents proven implementation and recorded validation without mirroring the private source.

Historical source documents can describe superseded synchronization arrangements. Public claims follow the current documented state and live baseline, not stale operational assumptions.
