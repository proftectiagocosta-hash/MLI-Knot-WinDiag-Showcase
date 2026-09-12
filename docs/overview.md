# Overview

MLI-Knot-WinDiag is a Windows diagnosis, maintenance and recovery platform built around conservative operational boundaries.

## Public-safe architecture summary

The current private baseline represents:

- local diagnostic orchestration;
- a local API and browser dashboard;
- a CLI;
- Windows-specific collectors;
- safe cleanup workflows;
- reversible Registry remediation;
- driver and firmware inventory;
- Windows update discovery;
- JSON and HTML reporting;
- asynchronous diagnostic jobs;
- WinPE-oriented recovery tooling;
- a remote-ready architecture that remains disabled by default.

The product separates discovery and diagnosis from write operations. Potentially destructive behavior requires stronger gates than observation.

This showcase documents the product without mirroring its private implementation.
