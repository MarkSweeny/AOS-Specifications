# Architectural contract model — working draft

Document: contract-model-working-draft · Source revision or record: Design brief, 29 September 2026

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**Status:** design brief for AOS-02 and its companion specifications, 29 September 2026. Source FAR-001 §§9–10, the incorporation review and AOS-00 DEC-002/005/015/019. It does not assert an approved shared schema.

An architectural contract specifies the meaning and obligations of a relationship between logical components or an external participant. Its minimum fields are: stable identity and version; producer and consumer roles; purpose and capability; data/event semantics; authority and permitted uses; preconditions; outputs and side effects; provenance; uncertainty; retention; failure and escalation; observable evidence; conformance cases; semantic owner and change authority. An interface or API realises only part of that contract.

**Example to develop:** a housing management system supplies a repair's completion date as communicated to the resident, evidence of subsequent change and completion events to the governed data layer. Process and Asset Intelligence consume those events; Boundary Intelligence governs the external exchange where the supplier is external; shared identity, purpose and authority controls apply to every participant. The accountable human remains responsible for the overdue-repair escalation selected in DEC-021–026. Exact fields, timing and certification are open, not vendor promises.

Map suppliers by supported AOS capabilities, functions, authoritative records, contracts, exposed interfaces, assurance signals, dependencies and declared partial conformance. Record the distinction between source system, integration, intelligence and decision authority. Resolve semantic ownership under AOS-00 D02 before claiming a stable contract.

## Development reference — 4 October 2026

[Shared Contracts v0.1 review draft](aos-shared-contracts-v0-1-review-draft.md) develops this brief and AOS-00 v0.6 §5.2 into a joint dossier for item 6. It preserves all seven IF identifiers, proposes common semantics and lifecycle/failure obligations, includes nineteen draft obligations and twelve planned verification cases, and makes twelve decision/parameter gaps explicit. The ownership direction under AOS-00-DEC-002 was approved by Mark on 4 October; role appointments, change procedure and exact contract definitions remain open; no shared schema or component specification is approved by this reference. This document remains an explanatory brief, not a second competing contract definition. Use the dossier for current detailed drafting and the controlled architecture for responsibility/decision status.

