# AOS-20–25 and AOS-30 — consistency review

Document: aos-20-25-and-30-gi-consistency-review-v0-1 · Source revision or record: v0.2

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

Version: 0.2  
Date: 7 October 2026  
Status: author review and authorised functional corrections complete; GI-CR-01–04 closed. Planned acceptance cases remain unexecuted.

## 1. Conclusion

The seven specifications form a coherent functional architecture. Corpus stewardship, synthesis, artefact assessment, presentation, oversight and human decision support have distinct responsibilities. The kernel retains authority, data custody, permitted use and enforced execution. No fundamental responsibility conflict or new general architecture decision was identified.

Four targeted changes were identified and have now been applied to close the GI drafting/consistency item: reciprocal independence of the two review accounts; complete reciprocal decision-record consumer declarations; unqualified wording of the human Mode 2 boundary; and current completion/traceability statements. The first two were functional specification gaps; the others were wording and documentary maintenance. They have been resolved within existing principles and approved directions. The finding descriptions below retain the reviewed issues; §7 records their applied closure evidence.

This review assesses functional consistency and planned evidence. Exact schemas, APIs, deployment counts, numerical thresholds, appointments and operational profiles can remain later owned dependencies. Their absence is not a reason to enlarge these specifications now.

## 2. Reviewed baseline before amendments and authority

| Document | Current version | Review role |
| --- | --- | --- |
| AOS-20 | 0.4 | GI charter and responsibility boundaries |
| AOS-21 | 0.5 | Corpus, organisation context and precedent |
| AOS-22 | 0.3 | Synthesis, interpretation and options |
| AOS-23 | 0.4 | Artefact assessment and monitoring |
| AOS-24 | 0.2 | Petra presentation and explanation |
| AOS-25 | 0.1 | Oversight, drift and learning |
| AOS-30 | 0.4 | Human records, approval and accountability |
| AOS-00 / Specification Map | 0.31 / 0.31 | Allocation and DEC-001–091 |
| AOS-01–05 / AOS-14 | 0.8 / 0.4 | Kernel and Boundary constraints |
| Shared / Core / Exchange Register | 0.14 / 0.6 / 0.13 | Common semantic definitions and reciprocal adoption |
| Source Traceability Matrix | 0.14 | Source allocation; original source manifest preserved |
| Control Coordination / Protected Reporting and Recovery | 0.2 / 0.1 | Current checks, corrections, reporting and recovery |
| Component template / quality standard | 0.4 / 0.1 | Specification level, traceability and honest assurance |

Governing sources: Foundational Principles v4; Reasoning Principles v6; Governance Intelligence Tests. Supporting sources: GI Internal Architecture working paper, Petra, Trade-Off Divergence Tool and GIL v2. The GIL comparison v0.2 records 38 dispositions and the approved subsidiary/corroboration directions DEC-090/091. Older dated baseline entries are historical; they do not themselves contradict a clearly stated current baseline.

## 3. Findings and proportionate remedies

### GI-CR-01 — Make report preparation independent in both directions

**Priority: medium. Owner: AOS-25, with AOS-20/21/30 and the organisation’s independent review authority. Status: closed at the functional-document level; see §7.**

RP v6, precedent integrity, requires the system self-assessment and independent curation report to be prepared without reference to each other. AOS-20 §3, AOS-21 VER-017, AOS-25 REQ-021/§7/§10/VER-015 and AOS-30 VER-023 explicitly protect the human account from prior GI framing. They do not expressly prohibit the GI account from being prepared using the independent human account. “Separate reports” alone does not establish that reciprocal preparation boundary.

**Remedy:** state that each account is prepared independently of the other account before their formal comparison. Both may use the same permitted underlying evidence, with differing evidence and revisions disclosed. Preserve the original accounts and any subsequent responses or revisions. This does not create a second evidence store or prevent later dialogue.

**Closure evidence:** aligned requirements/workflows in 20/21/25/30; a planned case where GI has access to the human report before its own preparation, alongside the existing reverse-direction case. The claimed independence must fail in either direction. Operating independence remains an appointed human institution, not a second model.

### GI-CR-02 — Complete reciprocal decision-record and outcome declarations

**Priority: medium. Owner: AOS-30 and AOS-02/common-contract custodians, with AOS-22/23/24/25. Status: closed at the functional-document level; see §7.**

AOS-23 CON-005 explicitly consumes human validation, decision and action/outcome evidence through 30/01/13. AOS-24 CON-004 uses human records through AOS-30-IF-001/KX-06, and CON-007 includes outcome feedback. However, AOS-30 CON-004 names 20–22/25, omitting 23/24; CON-005’s feedback recipients omit 22/23/24. Shared §4.5 and the Exchange Register’s KX-06/§14 producer declaration also omit 23/24, while the later component adoption entries declare their consumption.

The intended functions are present. The reciprocal catalogues are incomplete, leaving it unclear which consumers must accept the exact approval, correction and outcome semantics.

**Remedy:** align the producer declarations with the consumer views already specified. Identify permitted decision/validation consumers and outcome-feedback consumers by purpose, including 23/24 where their functions require them. Delivery may be through AOS-02 and permitted projections; direct interfaces or universal distribution are not required. Distinguish analytical validation, approved decisions, accepted duties, actual effects and reviewed outcomes throughout.

**Closure evidence:** matching 30/common/Register and 22–25 declarations; an AOS-40 planned walkthrough carrying a validated analysis, Chair-approved draft, board-approved record, changed evidence and actual outcome to the relevant permitted consumers. Omitted or unauthorised recipients remain explicit; receipt is not acceptance or completion.

### GI-CR-03 — Remove the qualification from the Mode 2 prohibition

**Priority: low, normative wording. Owner: AOS-20/22. Status: closed at the functional-document level; see §7.**

AOS-20 REQ-019 and AOS-22 REQ-016 prohibit selecting between incommensurable goods through “unapproved or inferred” moral weights. Read alone, this could imply that approved weights authorise machine selection. The surrounding architecture is stronger: AOS-20 §7 prohibits determining which incommensurable good yields; AOS-22 REQ-015 refers such choices to empowered humans; AOS-24 §7 and AOS-30 §7 retain permanent human judgement.

**Remedy:** make the local requirements say plainly that GI shall not adjudicate between incommensurable goods. Separately retain approved commensurable Mode 1 comparisons. Preserve CAP-01’s stricter no-ranking/no-scoring/no-recommendation rule across synthesis, presentation and longitudinal review.

**Closure evidence:** consistent wording and a planned contrasting case showing that even explicitly approved moral weights cannot transfer a Mode 2 judgement to the system. This clarifies the existing FP2 boundary; it introduces no new approval choice.

### GI-CR-04 — Refresh completion and ownership statements

**Priority: low, documentary maintenance. Owner: project custodian and relevant component/common-document owners. Status: closed at the functional-document level; see §7.**

AOS-20 §21 still describes 52 requirements/32 cases and says remaining AOS-21–25 drafting is next. Its current registers contain 57 requirements/38 cases after the external-research additions. AOS-20 §3.1’s assignment sentence also conflates the accountable GI owner, AOS-25 coordination and specialist reviewers. AOS-24 ISS-005 still refers to counterpart 25 adoption without distinguishing its now-completed functional draft from future operational compatibility. The GIL comparison’s opening status says component requirements remain to draft; that was correct when recorded, but needs a current completion note rather than erasure of its history.

**Remedy:** update present-tense counts and next steps; state that 20 owns its charter-level research remit, 21–25 own their specialist remits and 25 oversees portfolio coverage. Mark functional drafting/allocation complete while keeping exact compatibility, operating setup and assurance open. Link this review and its remaining findings from the current status records.

**Closure evidence:** current counts agree with registers; no active statement presents 21–25 as awaiting drafting; research ownership is readable without changing DEC-086; historical entries and original source manifest remain intact.

## 4. Cross-component behaviour checked — reviewed baseline; corrections in §7

| Relationship / scenario | Assessment |
| --- | --- |
| 21 sources → 22 synthesis / 23 assessment → 24 presentation → 30 human workflow → 25 learning | Coherent ownership. Canonical content and exact evidence/review revisions remain identifiable; 24 cannot silently revise another owner’s analysis. Reciprocal human-record catalogues need GI-CR-02. |
| Evidence and assessment | Source provenance, fact assurance, uncertainty, document quality, claim support and practice evidence remain distinct. DEC-091 permits corroboration without turning documents or interviews into certification. |
| Subsidiaries and group context | DEC-090 is carried through scoped profiles, applicability, powers and permitted joins. Group membership does not confer parent authority or data access. |
| Board approval and precedent | Minute-taker authorship, Company Secretary stewardship, Chair draft approval and board minutes/decision approval remain separate. An extract cannot replace board approval. Admission, conversational confirmation and approved precedent are distinct. |
| CAP-01 through 22/24/25/30 | Shared factual basis, unranked readings, infeasible alternatives and human-confirmed mixed/disputed/unknown decision mapping are coherent. Distributional patterns do not become moral verdicts or automatic calibration. |
| Independent preparation and constitutional review | Executive tuning is barred; common evidence does not require identical conclusions. Annual and material-triggered reviews retain empowered dispositions and corrective owners/dates. GI-CR-01 closes reciprocal preparation wording. |
| Corrections after preparation, decision or effect | 21–25 notify materially affected 30 workflows; GI revises analysis and 30 obtains empowered human review. Approved minutes and completed effects are not silently rewritten or automatically reversed. |
| Protected reporting and failed human handoff | Mandatory classes bypass optional executive review/preparation windows. Implicated-recipient alternatives, permitted minimal disclosure, explicit responsibility acceptance, cover and unresolved duties agree with kernel reporting/recovery. |
| External research | Each component has a DEC-086 remit and shared evidence/coverage/disposition inheritance. Boundary governs access; 25 portfolio oversight does not take over substantive ownership. Findings do not approve amendment or activation. |
| Privacy, audit and recovery | Derived use and disclosure need independent permission; lifecycle includes derivatives and recovery copies. Current checks and effect reconciliation survive approval or restoration. No unlimited-retention, silence-as-success or automatic replay rule is reintroduced. |

## 5. GIL v2 disposition check

All 38 comparison rows have an identifiable functional destination or explicit retirement/deferment. This table completes the author allocation check; it does not claim full original FP/RP source-item closure, executed conformance or adoption of legacy implementation choices. The four findings above are now closed at the functional-document level, with evidence in §7.

| Disposition | Current destination / treatment |
| --- | --- |
| C01 | 20 §§1/3; organisational ownership retained |
| C02 | 20/22/30 §§1/7; 1+5 and human adjudication |
| C03 | 20 §3; 21–25 decomposition |
| C04 | 21 catalogue and 23/25 coverage; no 121-item completeness claim |
| C05 | 23 assurance boundaries; 24/30 delivery without certification |
| C06 | 21/23 inputs and 24/30 protected-meeting boundary |
| C07 | All component research remits; 14 external access, 01 powers |
| C08 | 20 canonical states; 22–25 provisional/validated reliance; 30 approval |
| C09 | 20/23 authority boundaries; kernel instruments/current checks govern |
| C10 | 21 currency, 23 monitoring/cycles, 25/30 review; profile-owned cadence |
| C11 | Legacy vendor/database/endpoints deferred; kernel privacy/security apply |
| C12 | 21 organisation profiles; multiple sourced revisions and confirmation |
| C13 | 21–25 explicit unknown/disputed/withheld states |
| C14 | 21 criteria/corpus; 23 applicability; analytical standards are not powers |
| C15 | 21 stewardship and 01/30 empowered changes |
| C16 | 23 assessment dimensions and permitted practice corroboration |
| C17 | 20/23 uncertainty/assurance; universal scores and thresholds retired |
| C18 | 22/23 findings/questions; 24 explanation; 30 accepted duties |
| C19 | 21/23 coverage states; 25 patterns; 30 ownership |
| C20 | 23/04 governed tasks; mandatory agent counts and fixed timings retired |
| C21 | 21/23 currency; component research coverage records |
| C22 | 20–25 bounded analysis/research; 25 oversight; 30 human adoption |
| C23 | 01/03/04/05 controls inherited; no local approval-flag guarantee |
| C24 | 21–25/30 audit; 02 custody; no separate truth silo |
| C25 | Governed class-based lifecycle; blanket retention/soft-delete-only retired |
| C26 | 21/23/30 semantic operations retained; endpoint design deferred |
| C27 | 21/23 faithful application; 25/30 feedback; autonomous calibration retired |
| C28 | 23 assessment/review/correction workflow |
| C29 | 22/23 canonical content, 24 presentation, 30 approval; GI-CR-02 |
| C30 | 20/23/25/30 protected handoff and kernel fallback; executive gate retired |
| C31 | 21–25/30 material impact and owned review; blanket waiting retired |
| C32 | Each component §8; FP v4/RP v6/GT contributions, no claimed passes |
| C33 | 22 infeasible alternatives; 23 missing-evidence questions remain distinct |
| C34 | 22/25/30 actual outcomes and human review, not database-only telos claims |
| C35 | Kernel use controls; 20–25/30 purpose-bound explanation and descriptors |
| C36 | AOS-40 later scenario work; build sequencing deferred |
| C37 | 21 catalogue/seed coverage; 23 assessment; 24/30 channels deferred |
| C38 | 21/23 scoped subsidiary context and currency under DEC-090 |

C01–C38 abbreviate the existing GIL-C01–GIL-C38 identifiers; no source identifiers are replaced. DEC-090 and DEC-091 are applied, not reopened. GI-CR-01 follows the governing RP v6 source rather than a new legacy GIL requirement.

## 6. Author checks and next action

| Component | Proposed requirements | Planned cases |
| --- | --- | --- |
| 20 | 57 | 38 |
| 21 | 48 | 30 |
| 22 | 52 | 32 |
| 23 | 52 | 32 |
| 24 | 40 | 26 |
| 25 | 48 | 30 |
| 30 | 48 | 31 |
| Total | 345 | 219 |

All seven have the template’s 21 numbered sections. Register checks found no missing referenced case or requirement and no mismatched reverse link among the requirement-to-case links declared in these tables. These are document checks, not execution of the 219 cases. They do not establish that every source obligation has an adequate test; the reciprocal independence case above is a semantic coverage gap despite valid links.

GI-CR-01–04 have been applied and checked; item 7 is closed at the author functional-specification level. Next proceed to AOS-40 acceptance scenarios under item 8, including the already agreed overdue-repair demonstration and contrasting governance cases. Independent project review remains deferred. Operating human independence, exact compatible profiles and accepted evidence remain required before their dependent operation.

No DEC, IF, specification requirement status, source manifest, schedule, deployment or readiness approval is changed by these corrections.

## 7. Applied correction and closure evidence — 7 October 2026

Mark instructed: “apply these corrections, close the GI consistency work.” All four findings are closed at the functional-document level.

| Finding | Applied evidence / disposition |
| --- | --- |
| GI-CR-01 | 20 REQ-034/§3, 21 REQ-025/§10.5, 25 REQ-021/§7/§10/§11, 30 REQ-038 explicitly require reciprocal independent preparation. Existing VER-014/017/015/023 respectively now test both contamination directions; common evidence and later responses remain permitted/distinct. Closed. |
| GI-CR-02 | 30 CON-004/005 and §6.4, Shared §4.5 and Exchange Register KX-06/§14 include the already specified 23/24 consumers and relevant 22–25 outcome feedback. 30 VER-021 carries approved/corrected records and outcomes to permitted consumers. No direct channel or expanded permission. Closed. |
| GI-CR-03 | 20 REQ-019 and 22 REQ-016/§7 prohibit GI adjudication even with approved moral weights; existing VER-005/009 contrast commensurable Mode 1 comparison with permanently human Mode 2. CAP-01 remains unranked. Closed. |
| GI-CR-04 | 20 §21 counts corrected to 57/38 and next step to 40; §3.1 research owners separated; 24 ISS-005 distinguishes completed functional adoption from operating compatibility; GIL comparison v0.3 and suite/current status notes record completed drafting. Historical entries and source manifest retained. Closed. |

AOS-00/Map v0.32, DEC-001–091; AOS-20 v0.5/21 v0.6/22 v0.4/23 v0.5/24 v0.3/25 v0.2/30 v0.5; AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.15/Core v0.6/Exchange Register v0.14/source matrix v0.15; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1.

Author checks: all seven 21-section structures retained; requirement and case identifier sets/counts remain 345/219; every declared REQ-to-case link resolves and has its reverse requirement link; Markdown table widths remain consistent. AOS-23’s requirement, case and contract rows are unchanged. Changed case content provides planned evidence only; none was executed. The 38 GIL disposition rows remain intact and allocated. This closure does not substitute for independent project review, operational human review or commissioned conformance.

Item 7 is complete. Tomorrow’s starting point: AOS-40 planned acceptance scenarios, preserving the agreed overdue-repair demonstration and contrasting governance cases.

