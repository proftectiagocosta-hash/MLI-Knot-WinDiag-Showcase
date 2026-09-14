# Public roadmap

## 0.1 — Foundation

**Status: implemented.**

The private source contains the local diagnostic engine, API/dashboard, CLI, Windows collectors, safe-cleanup mechanisms, reversible Registry remediation, driver/firmware inventory, Windows Update discovery, JSON/HTML reporting, asynchronous jobs and WinPE-oriented recovery assets.

A recorded Windows checkpoint also reports a successful Release build and passing smoke tests for the baseline.

## 0.2 — Stabilization

**Status: next.**

The source roadmap includes broader Windows validation/correction, additional Registry coverage, correlation/history, stronger protection of local credentials, signed action receipts and dashboard improvements.

## 0.3 — Controlled repair

**Status: planned.**

Planned analysis and controlled-repair workflows include Windows integrity, update-cache handling, services/tasks, network reset and offline recovery.

## 0.4 — OEM adapters

**Status: planned.**

Planned work includes vendor-specific discovery, exact model/revision matching, official package validation, driver backup and recoverable vendor workflows.

Generic firmware flashing is not part of the current baseline automation model.

## 0.5 — Remote management

**Status: planned.**

The architecture anticipates service hosting, mutual authentication, role-based authorization, support sessions, central history and remote writes only after sufficient audit maturity.

The current source remains local-only by default. Remote production readiness is not claimed.

## 1.0 — Stable product

**Status: gated future release.**

The source reserves 1.0 for completion of multi-machine validation, recovery drills, threat-model review, signed packages, documented rollback and reproducible WinPE generation.

## Progress convention

This roadmap reports milestone **state**, not an equal-weight completion percentage.

The former `1/6 = 16.7%` representation was only a mathematical count of named milestones. Because those milestones have different scope and complexity, it is not used here as an engineering-progress, security-maturity or production-readiness metric.
