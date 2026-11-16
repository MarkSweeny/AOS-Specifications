# DEC-105 — technical-control limits and observed evidence

Document: aos-dec-105-technical-control-limits-and-evidence-2026-10-29 · Source revision or record: DEC-105, 29 October 2026

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

29 October 2026 · Mark approved substantive question 7 in this chat (“yes”). Author: Codex. Approved assurance direction; detailed proposed wording retains ordinary separate quality/design/readiness gates.

## Approved rule

Operational reliance on implemented technical controls requires explicit scope, limits and failure/recovery behaviour supported by accepted observed evidence. The evidence must cover all enabled action paths within the declared control/threat scope, independently of the acting agent; permission-change enforcement points and timing uncertainty; shared cumulative bounds under concurrency; conservative treatment of unknown effects/reservations; and recovery that applies current restrictions without reviving withdrawn authority or repeating completed effects.

The approved control profile fixes exact functions/paths/dependencies/versions, threat assumptions, effect boundary, currentness and revocation/fencing mechanism, timing/uncertainty bounds and units, accounting scopes/consistency and admission, uncertain exposure/release evidence, recovery source/currentness/completeness, permitted fallback/continuing duty, observability/oracle, assessors and objective acceptance conditions. Timeout, cancellation, worker retirement or failover alone cannot prove no effect, release possibly used capacity or permit consequential repetition. No instantaneous global revocation or recall of an irreversible disclosure is promised. Limits are assessed under actual constraints and powers, not silently accepted as waivers of non-waivable safeguards. Missing/failed evidence blocks affected operational-reliance claims with an owned remedy; separately authorised service/reporting duties remain owned and do not acquire extra permissions.

G3 remains authorisation of a bounded build with fixed scope, explicit dependencies/profiles and required separate review; G4 requires implemented observations, and actual operational approval is separate. An explicitly authorised bounded prototype can investigate the mechanisms before operational assurance exists; this decision itself authorises neither a prototype nor live effects. A failed prototype requires investigation of the implementation, assumptions and alternatives; it is not alone proof of architectural impossibility. Model refusal, a generated explanation, intended configuration, an old checkpoint or retrospective log alone is not evidence that all effect paths were enforced or recovery was current. Actual acceptance must link observations to the exact requirement/local-case/variant/profile and endpoint scope, with limitations and competent assessor disposition.

## Controlled allocation

DEC-105 → AOS-05 REQ-077 / planned VER-065 and AOS-40 REQ-041 / planned VER-039 with independent variants V01/V02. Operational Profiles, Control Coordination and Protected Reporting/Recovery carry scope/limit/observability and permitted fallback gates; existing conservative reservation, current-control and no-revival/no-replay meanings retained. Current catalogues: AOS-05 77 REQs / 65 cases; AOS-40 41 REQs / 39 parent cases / 110 variants; non-AOS-40 local cases 664 including retained deferred IDs. Original identities preserved; no case executed. This adopts an assurance requirement, not a technology, numerical default, permission to prototype or deployment.

AOS-00/Map v0.55. Current document versions and actual catalogue populations are in the current inventory and acceptance annex addendum. No record/view schema revision is allocated by this assurance requirement; existing technical rules, source statuses and DEC-099–104 retained. The accepted direction does not demonstrate any implementation or choose technology; S-08–09 remain undecided.

## Verification/provenance

Originals/candidates, exact diff, hashes and scoped checks are retained locally in `AOS/deliverability-review-2026-10-29/decision-105`. Checks preserve existing normative rows and identities, verify the two new requirements/cases and two new variants, existing case counterparts and current counts, added relative destinations and saved contents. All AOS cases remain planned/unexecuted; these document checks are not independent operational assurance.

