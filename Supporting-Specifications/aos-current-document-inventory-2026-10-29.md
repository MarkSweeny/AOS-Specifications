# AOS current document inventory — 29 October 2026

Document: aos-current-document-inventory-2026-10-29 · Source revision or record: 29 October 2026 editorial control record

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

Status: editorial navigation/control record under Mark's approved D-01–09 corrections. It records current document identities and retained functional baselines, not approved executable schemas or readiness. This inventory supersedes older “current revision set” summaries as navigation; it does not supersede source decisions or definitions. The working files retain their internal functional version and add the dated editorial edition where changed. Exact before/after hashes are retained in the local correction evidence.

## Component catalogues

Counts are retained normative table identities and planned case identities, deduplicated by local ID; deferred identities are retained catalogue entries and not active-core evidence. A listed case is planned, never an execution result. Counts do not measure semantic uniqueness or implementation coverage. The kernel requirement rows total 366, not 366 independent safety guarantees.

| Component | Retained functional baseline | Retained requirement IDs | Planned case IDs |
| --- | --- | --- | --- |
| [AOS-01](../Foundation/aos-01-authority-constitutional-controls-and-change.md) | 0.12 | 70 | 46 |
| [AOS-02](../Foundation/aos-02-unified-data-layer-and-shared-records.md) | 0.11 | 73 | 49 |
| [AOS-03](../Foundation/aos-03-identity-access-consent-and-data-use.md) | 0.12 | 69 | 52 |
| [AOS-04](../Foundation/aos-04-common-agent-architecture-and-lifecycle.md) | 0.10 | 77 | 57 |
| [AOS-05](../Foundation/aos-05-platform-operation-security-and-resilience.md) | 0.11 | 77 | 65 |
| [AOS-10](../Sensing-Domains/aos-10-asset-intelligence.md) | 0.5 | 49 | 34 |
| [AOS-11](../Sensing-Domains/aos-11-resident-intelligence.md) | 0.3 | 55 | 33 |
| [AOS-12](../Sensing-Domains/aos-12-people-intelligence.md) | 0.3 | 53 | 35 |
| [AOS-13](../Sensing-Domains/aos-13-process-intelligence-and-operational-coordination.md) | 0.2 | 57 | 40 |
| [AOS-14](../Sensing-Domains/aos-14-boundary-intelligence-and-external-exchange.md) | 0.9 | 55 | 34 |
| [AOS-20](../Governance-Intelligence/aos-20-governance-intelligence-architecture-and-charter.md) | 0.8 | 57 | 38 |
| [AOS-21](../Governance-Intelligence/aos-21-corpus-organisation-knowledge-and-precedent.md) | 0.7 | 48 | 30 |
| [AOS-22](../Governance-Intelligence/aos-22-synthesis-interpretation-and-option-preparation.md) | 0.6 | 52 | 32 |
| [AOS-23](../Governance-Intelligence/aos-23-governance-artefact-assessment-and-monitoring.md) | 0.6 | 52 | 32 |
| [AOS-24](../Governance-Intelligence/aos-24-petra-presentation-and-explanation.md) | 0.5 | 40 | 26 |
| [AOS-25](../Governance-Intelligence/aos-25-governance-oversight-drift-and-learning.md) | 0.5 | 48 | 30 |
| [AOS-30](../Governance-Intelligence/aos-30-governance-hub-and-accountable-decision-workflows.md) | 0.8 | 48 | 31 |
| [AOS-40](aos-40-acceptance-integration-assurance-and-commissioning.md) | 0.13 | 41 | 39 |

The AOS-40 annex v0.7 contains 110 planned variants across 39 parent cases; its original 660-entry non-AOS-40 inventory plus four subsequent-decision entries describes 664 retained local cases, including seven deferred Phase 2-only cases. Parent cases, variants and local rows are different units and must not be added into an executed-coverage total. Exact run scope/bindings, justified exclusions and observed evidence remain separate prerequisites.

## Common and controlling documents

| Document | Retained internal functional baseline / authority |
| --- | --- |
| [AOS_00_SYSTEM_ARCHITECTURE.md](../Foundation/aos-00.md) | AOS-00 0.55; DEC-001–105, with their recorded individual status |
| [SPECIFICATION_MAP.md](../Foundation/specification-map.md) | Map 0.55 |
| [PROJECT_OBJECTIVE.md](../Foundation/project-objective.md) | Unchanged objective; handover without invented material decisions |
| [SPECIFICATION_QUALITY_STANDARD.md](../Foundation/specification-quality-standard.md) | AOS-QS 0.1; separate quality/design and G1–G4 gates |
| [AOS-Shared-Contracts-v0.1-review-draft.md](../Foundation/aos-shared-contracts-v0-1-review-draft.md) | Shared 0.27 |
| [AOS-Core-Record-Contracts-v0.1-review-draft.md](../Foundation/aos-core-record-contracts-v0-1-review-draft.md) | Core 0.11 |
| [AOS-Kernel-Exchange-Register-v0.1.md](../Foundation/aos-kernel-exchange-register-v0-1.md) | Register 0.26; §4 is the current family/view revision and owner index |
| [AOS-Kernel-Control-Coordination-v0.1.md](../Foundation/aos-kernel-control-coordination-v0-1.md) | Coordination 0.3 |
| [AOS-Kernel-Protected-Reporting-and-Recovery-v0.1.md](../Foundation/aos-kernel-protected-reporting-and-recovery-v0-1.md) | Protected Reporting and Recovery 0.3 |
| [AOS-Operational-Profiles-v0.1-review-draft.md](../Foundation/aos-operational-profiles-v0-1-review-draft.md) | Operational Profiles 0.6 |
| [AOS-Source-Traceability-Matrix-v0.1.md](../Foundation/aos-source-traceability-matrix-v0-1.md) | Source Matrix 0.28; original source statuses retained |
| [AOS-Extension-and-Conformance-Specification-v0.1.md](../Foundation/aos-extension-and-conformance-specification-v0-1.md) | AOS-EC 0.1; proposed claim model |
| [AOS-Change-Constitution-v0.1.md](aos-change-constitution-v0-1.md) | Draft 0.1; adoption not implied |
| [AOS-README.md](../Foundation/aos-readme.md) | Expanded orientation adopted 29 October; updated correction links |
| internal project work record | Live work record; dated earlier priorities are historical where superseded |

Document versions and logical family/view revisions are different. The filename `v0.1` and the folder `V0.1` are historical paths, not current versions. No semantic revision is advanced by this editorial correction; affected source documents explicitly carry the dated editorial edition. Future material or semantic changes require their separate controlled revision/compatibility assessment.

## Scope and dependencies

CAP-01/02 and RI-001 remain deferred under DEC-097/098. General risk, purpose, independent challenge, human judgement, evidence and protected reporting remain current. The overdue-repair context remains the first selected demonstration. Requirements are proposed, cases planned/unexecuted and independent project review deferred; documentary closure is not whole-document approval, G3/G4, legal/institutional assurance or live activation. The substantive questions in the deliverability review remain separately open.

## Subsequent substantive decision — DEC-099, 29 October 2026

Question 1 approved: derived-information restrictions. The current version rows above incorporate this controlled semantic amendment; the preceding editorial-only statements describe the D-01–09 correction event, not this later decision. See [DEC-099 record](aos-dec-099-derived-information-restrictions-2026-10-29.md). Catalogue identities/counts unchanged; S-01 is approved at direction/amended-draft level, with implementation/profile/verification dependencies retained. S-02–09 remain open.

## Subsequent substantive decision — DEC-100, 29 October 2026

Question 2 approved: independent advance minimum control-metadata access. Current version/count rows above include AOS-01/03 REQ-069 and planned VER-045/052; earlier ID/count-preservation statements describe the earlier correction/DEC-099 events only. [DEC-100 record](aos-dec-100-control-metadata-access-2026-10-29.md). S-01/02 directions are approved with implementation/profile/evidence gates retained; S-03–09 remain open. No case executed.

## Subsequent substantive decision — DEC-101, 29 October 2026

Human capacity and meaningful review approved as operational-reliance conditions. Current rows reflect amended proposed AOS-30 v0.6 / AOS-40 v0.9 and Operational Profiles v0.2; acceptance annex v0.3 retains all existing identities/counts. [DEC-101 record](aos-dec-101-human-capacity-and-meaningful-review-2026-10-29.md). S-01–03 directions approved, with implementation/organisation/evidence gates retained; S-04–09 remain open.

## Subsequent substantive decision — DEC-102, 29 October 2026

Classification/configuration adequacy approved. Current rows include AOS-01 REQ-070 / VER-046 and revised AOS-01 REQ-015 and AOS-40 REQ-030; preceding count-preservation statements apply to their dated events. [DEC-102 record](aos-dec-102-classification-and-configuration-adequacy-2026-10-29.md). S-01–04 directions approved, with actual profiles/assessment/implementation evidence still gated; S-05–09 remain open.

## Subsequent substantive decision — DEC-103, 29 October 2026

Question 5 approved in revised form after primary legal-source review. [DEC-103 record](aos-dec-103-decision-validity-evidence-and-minutes-2026-10-29.md) governs partial supersession of DEC-087 and KX-06 v0.3. Current rows above identify amended owner/consumer documents; unchanged IDs/counts supply no implementation coverage. S-01–05 directions approved with evidence/profile/compatibility gates retained; S-06–09 remain open.

## Subsequent substantive decision — DEC-104, 29 October 2026

Question 6 approved and applied: class-specific protected reporting against both technical failure and implicated-person suppression. [DEC-104 record](aos-dec-104-protected-reporting-and-implicated-recipients-2026-10-29.md). Current rows incorporate amended owner/consumer documents and KX-19 protected_finding v0.3; all requirement/case/variant IDs/counts retained. S-01–06 directions approved with actual institution/profile/permission/compatibility evidence still required; S-07–09 remain open.

## Subsequent substantive decision — DEC-105, 29 October 2026

Question 7 approved: declared technical limits and observed failure/recovery evidence before operational reliance. [DEC-105 record](aos-dec-105-technical-control-limits-and-evidence-2026-10-29.md). Current rows include new AOS-05 REQ-077 / VER-065 and AOS-40 REQ-041 / VER-039-V01/V02; earlier preservation/count statements describe their dated events. All other existing IDs retained. S-01–07 directions approved with actual profile/implementation/assessment gates retained; S-08–09 remain open.

## Review disposition — S-08, 29 October 2026

Mark rejected question 8 as an architectural amendment. The AI Governance and Ethics Committee already owns the relevant oversight judgement; bounded-task evaluation and related methods are procedural options within that remit. [S-08 disposition](aos-deliverability-review-s08-disposition-2026-10-29.md). No technical baseline, requirement/case/variant identity, count or committee power changes. S-08 is closed/reclassified, not a pending architectural decision; S-09 remains to be triaged. Prior dated statements treating S-08 as open are history.

## Final disposition of substantive review questions — 29 October 2026

Mark agreed to close S-09 without an architectural amendment. No contradiction was demonstrated between prohibited personal inference and permitted welfare referral; existing purpose/data-use controls govern cross-domain personnel reuse. S-01–07 are adopted directions DEC-099–105; S-08 is rejected/reclassified to existing committee procedure; S-09 is closed with no architectural change. [Final disposition record](aos-deliverability-review-s09-and-final-disposition-2026-10-29.md). No technical version, requirement/case/variant identity or count changes through this disposition. Earlier statements that S-08/09 remain open are historical. Completing question disposition does not establish implementation readiness, executed acceptance, publication approval, independent assurance or legal/institutional conformance.

