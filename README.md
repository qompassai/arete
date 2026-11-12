# Arete

**Arete** (Greek ἀρετή — excellence: quality you can see in the work) is a library of fixes for **Salesforce** and **Salesforce Field Service**, prepared for submission to TDS through the **TRIS** (Technology Request Information Sheet) process.

Each fix is authored and verified outside TDS systems, packaged here as a self-contained, evidence-carrying unit, and submitted through TRIS for review. A fix is applied to a TDS org only after approval, through the normal change process. Nothing in this repository connects to, runs against, or contains data from any TDS system.

## Tracks

- [`salesforce/`](salesforce/) — Salesforce platform fixes: Apex, Lightning Web Components, flows, AgentScript agents, and related configuration/metadata.
- [`field-service/`](field-service/) — Salesforce Field Service fixes: the Field Service mobile app, scheduling, work orders and service appointments, and related configuration.

## Per-fix convention

One folder per fix, inside its track, named for the problem it solves. Every fix folder contains:

1. **Problem statement** — what is wrong, where it shows up, and how it was observed.
2. **The change** — the complete fix: source, metadata, or configuration, ready to review as-is.
3. **Test / verification evidence** — how the fix was verified (tests run, scratch-org results, before/after evidence), sufficient for a reviewer to reproduce the result.

A fix that cannot carry all three does not belong here yet.

## Content rules

This repository is public by design. Contents are generic and publishable only:

- No TDS data, org identifiers, internal hostnames, ticket numbers, or customer information.
- No credentials, tokens, or secrets of any kind.
- Verification evidence is produced in scratch or developer orgs, never in a TDS org.

## TRIS submission

The TRIS worksheet for this library lives in [`tris/WORKSHEET.md`](tris/WORKSHEET.md), in the same format as the worksheets of the other Qompass AI products submitted through TRIS.

## License

Licensed under the Apache License 2.0 — see [LICENSE](LICENSE).
