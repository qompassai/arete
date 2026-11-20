# Arete (fix library for Salesforce and Salesforce Field Service) — TRIS form-input worksheet

The requestor's working worksheet for this product's TRIS form (Technology Request Information Sheet): every requestor-facing field, pre-filled from the submission evidence wherever the evidence supports a value. Anything only the requestor can supply is marked **[INPUT NEEDED: …]** — nothing here is invented. Numbers in parentheses are the TRIS template's row numbers, so each line can be checked against the form.

This worksheet covers Arete on its own. Arete is a fix library for Salesforce and Salesforce Field Service — not a standalone application — prepared for submission through the same TRIS process as the combined six-product submission worksheet prepared 2026-11-11 (ONTrack, LightShow, Fathom, Versemend, the Salesforce MCP integration, and Niflheim); its shared submitter fields match that package. IT reviewer fields (template rows 66–91) need no requestor input and are not listed here.

## Shared submitter fields (rows 3–6, repeated on all forms)

- Requestor (3): Matt A. Porter — Field Service Technician (FST), matthew.porter@tdstelecom.com
- Requestor's Manager (4): Josh Barter
- PAT Manager (5):
- CoE Director (6): [INPUT NEEDED: CoE Director for the accountable Agile team — if left blank, the TRIS Administrator determines the accountable team, AM, and AD per the process document]

## Product answers

- Technology Name (8): Arete — a fix library for Salesforce and Salesforce Field Service (public repository, qompassai/arete on GitHub).
- Technology Version (9): [INPUT NEEDED: version to cite — the library was created 2026-11-12 and is unversioned as a whole; each fix is a self-contained folder carrying its own problem statement, change, and verification evidence]
- Vendor Name (10): Salesforce (the platforms the fixes target). The library itself is the requestor's own work (Qompass AI).
- Website (11): https://github.com/qompassai/arete (the library itself). The target platforms are Salesforce's (salesforce.com).
- Description (14): A public library of fixes for Salesforce and Salesforce Field Service, in two tracks: salesforce/ (Apex, Lightning Web Components, flows, AgentScript agents, and related configuration/metadata) and field-service/ (Field Service mobile app configuration, scheduling, work orders and service appointments). One folder per fix, containing the problem statement, the complete change, and test/verification evidence. Fixes are authored and verified in scratch or developer orgs — never in a TDS org — and submitted through TRIS for review; a fix is applied to a TDS org only after approval, through the normal change process. Nothing in the library connects to or runs against any TDS system.
- How used at TDS (15): As the submission package for proposed Salesforce and Field Service changes: reviewers read the problem statement, the change, and the verification evidence in the repository, and any approved change is applied through the org's normal change process.
- Who will use it (16): The requestor (authoring and submitting fixes); TDS Salesforce administrators and developers reviewing submitted fixes.
- Technology replaced/removed (17): Nothing. No TDS technology is removed.
- Direct customer impact (18): No direct customer-facing impact — the library itself is a submission artifact; any org change resulting from it passes TRIS review and normal change control first.
- Supported internally or by vendor (19): The library is supported by the requestor. The target platforms are Salesforce's services, supported by Salesforce under the org's existing agreements.
- Production or test/development (20): Test/development at this time. Status, honestly: the library was created 2026-11-12 and currently contains no fixes — the two tracks, the per-fix convention, and this worksheet are in place. Each future fix is verified in a scratch/developer org before submission and reaches a TDS org only if approved through this review.
- Impact if discontinued (21): None — no system depends on the library; un-submitted fixes simply remain unused.
- Backout plan/cost (22): Delete the repository, or the individual fix folder. A fix already applied to an org is backed out per that fix's own documented reversal under the org's normal change process. Cost: minutes for the library itself.
- Similar technologies at TDS (23): [INPUT NEEDED: TDS-approved Salesforce tooling/processes to name as related — in the requestor's own use, the sf CLI and Salesforce Setup are the incumbent routes for org changes]
- Alternatives considered (24): Making changes directly in the org without a reviewed, evidence-carrying submission (no review trail); keeping fixes in private notes (not reviewable, not reusable). The library is requested because it makes each fix reviewable as a self-contained unit before submission.
- AI component (26): The library contains no AI model and runs no AI component. Individual fixes may concern AI features of the platform (for example AgentScript agent definitions); AI Policy 710 should be treated as applicable to such submissions.
- Internet access (28): No — the library is a static repository of documents and source; it makes no network calls. (It is hosted publicly on GitHub.)
- Hosted internal/external (29): External hosting of the repository (GitHub, public). Contents are generic and publishable by design — no TDS data, org identifiers, internal hostnames, ticket numbers, or credentials are stored in it.
- Uploads data outside the Enterprise network (30): No — no TDS or org data is uploaded. The repository contains only the requestor's own authored material, written for publication — the fix library, plus a draft public comment on NIST SP 2400-102 stored under nist/ (added 2026-11-14); verification evidence is produced in scratch/developer orgs.
- Inbound access to the Enterprise network (31): No — the library initiates no connections of any kind.
- Data collected (32): None. The library collects no data and processes no TDS data. Credentials: none are held — the repository is public and credential-free by rule.
- Java required (33): No.
- Microsoft 365 integration (34): No.
- Security risk assessment required (35): [INPUT NEEDED: whether a security risk assessment is required for a content-only fix library — the library holds no credentials and no TDS data and executes nothing; one is requested if the reviewer judges it necessary]
- Cardholder/banking data (36): No cardholder or banking data is processed or stored by the library.
- How licensed (38): The library is the requestor's own work, licensed under the Apache License 2.0. The target platforms are Salesforce commercial services under the org's existing agreements; no platform licensing changes.
- License model (39): Apache License 2.0 (permissive, no fees) for the library. Platform licensing is unchanged (Salesforce's existing agreements).
- License fees and quantity (40): None for the library. No new purchase is requested; platform use runs on the org's existing Salesforce entitlements.
- Support/maintenance fees (41): None for the library.
- How long around (43): Library created 2026-11-12. The target platforms (Salesforce and Salesforce Field Service) are long-standing Salesforce offerings already in use at TDS.
- Governing License (45): Apache License 2.0 governs the library. Salesforce service terms govern the target platforms.
- License previously reviewed by legal (46): [INPUT NEEDED: whether the Apache License 2.0 has prior TDS legal review in this context — an Apache-2.0 license statement was drafted for the six-product package prepared 2026-11-11]
- Distributed / external use (47): Yes — the repository is public on GitHub by design (generic, publishable material only; no TDS data). No TDS use depends on the public copy.
- Modified by TDS (48): No — the library is requestor-authored; TDS modification is not applicable. (Reviewers may adapt a submitted fix under the org's change process.)
- Directly impacts a product or service provided to customers (49): No — the library is a submission artifact for internal platform changes; anything applied passes TRIS and change control first.
- Mobile — developer (51): Not applicable to the library itself — it is not a mobile app. Field-service-track fixes concern the Salesforce Field Service mobile app (developer: Salesforce); the fix content is authored by the requestor.
- Mobile — store certification (52): Not applicable — no application is distributed.
- Mobile — platforms (53): Not applicable to the library. Field-service fixes may target the Salesforce Field Service mobile app (iOS/Android) as configuration/content, not as a distributed application.
- Mobile — TDS fee / required for a TDS service (54): No fee charged by TDS; not required to use any TDS service.
- Mobile — confidential information (55): No — the library holds no confidential information by design.
- Mobile — third-party code (56): Fixes are the requestor's own code and configuration. Platform code is Salesforce's own.
- Mobile — user data collection language (57): Not applicable — the library collects no user data and contains no telemetry.
- Mobile — development tools/SDKs (58): Salesforce DX / sf CLI toolchain for authoring and verification in scratch orgs. No Apple/Google SDK code is distributed by the library.
- Mobile — in-app purchase (59) / Apple push (60) / Game Center (61) / iCloud (62) / Passes (63) / Apple Maps (64): No / not applicable.

---
*Worksheet prepared 2026-11-12 from the TRIS template and process documents, mirroring the format of the six-product submission worksheets prepared 2026-11-11. DRAFT — not yet submitted. See the repository [README.md](../README.md) for the library overview.*
