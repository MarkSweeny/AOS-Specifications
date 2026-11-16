# AOS-23 — Governance artefact assessment and monitoring

Document: aos-23-governance-artefact-assessment-and-monitoring · Source revision or record: v0.6

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**DEC-103 adopted — 29 October 2026:** Current revision 0.6. Decision validity/effective time, attributable evidence/authentication, minutes approval and permission to execute are separate. DEC-087 is partly superseded; [decision/amendment and legal-source record](../Supporting-Specifications/aos-dec-103-decision-validity-evidence-and-minutes-2026-10-29.md). No universal later-minutes or second decision-record approval gate. Exact instruments/evidence policy, KX-06 v0.3 compatibility and ordinary separate review/readiness gates remain required; cases unexecuted. Earlier contrary wording is historical only where explicitly identified.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

**AOS-25 oversight counterpart alignment — 7 October 2026:** AOS-25 v0.1 now supplies the drafted oversight/drift/learning and GI research-portfolio counterpart. Reference-only revision; all existing requirement/case/contract rows preserved. AOS-00/Map v0.31, DEC-001–091; AOS-25 v0.1; AOS-20 v0.4/AOS-21 v0.5/AOS-22 v0.3/AOS-23 v0.4/AOS-24 v0.2/AOS-30 v0.4 (counterpart-reference alignment only); AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.14/Core v0.6/Exchange Register v0.13; source matrix v0.14; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. No build/activation/readiness approval. Next: author GI-set consistency/disposition review across AOS-20–25 and AOS-30, then AOS-40 acceptance scenarios under item 8; independent project review remains deferred. Earlier dated consultation/adoption entries remain history.

**AOS-24 presentation counterpart alignment — 7 October 2026:** AOS-24 v0.1 now supplies the drafted faithful-rendering/explanation counterpart. Reference-only revision; requirement, case and contract rows unchanged. AOS-00/Map v0.30, DEC-001–091; AOS-24 v0.1; AOS-21 v0.4/AOS-22 v0.2/AOS-23 v0.3 (reference alignment only); AOS-01–05 v0.8, AOS-14 v0.4, AOS-20 v0.3, AOS-30 v0.3; Shared v0.13/Core v0.6/Exchange Register v0.12; source matrix v0.13; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. No build/activation/readiness approval. Earlier dated consultation/adoption entries remain history.

**AOS-22 synthesis counterpart alignment — 7 October 2026:** AOS-22 v0.1 now supplies the drafted synthesis/interpretation/options counterpart. This revision changes pending-drafting/current-reference statements only; all requirement, case and contract meanings preserved. AOS-00/Map v0.29, DEC-001–091; AOS-22 v0.1; AOS-21 v0.3/AOS-23 v0.2 (counterpart/reference alignment only); AOS-01–05 v0.8, AOS-14 v0.4, AOS-20 v0.3, AOS-30 v0.3; Shared v0.12/Core v0.6/Exchange Register v0.11; source matrix v0.12; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. No build/activation/readiness approval.


| Document control | Value |
| --- | --- |
| Component / version / date | AOS-23 / 0.6 / 29 October 2026 |
| Status | Functional specification review draft; requirement wording proposed |
| Architecture baseline | AOS-00/Map v0.32, DEC-001–091; prior consultation/allocation retained as history |
| Governing sources | Foundational Principles v4; AOS Reasoning Principles v6; Governance Intelligence Tests; preserved source manifest |
| Dependency manifest consulted | AOS-01–05 v0.8; AOS-14 v0.4; AOS-20 v0.3; AOS-21 v0.1; AOS-30 v0.3; Shared v0.10/Core v0.6/Exchange Register v0.9; source matrix v0.10; Control Coordination v0.2; Protected Reporting and Recovery v0.1; research view RSVIEW-0.1; KX-06 v0.3 |
| Adoption supplements | Shared v0.11/Register v0.10/source matrix v0.11 record this draft's functional adoption; common definitions unchanged |
| Quality / template | AOS-QS v0.1; component template v0.4 |
| Project owner / custodian | Mark Sweeny |
| Operational owner | Accountable GI/artefact-assessment owner; empowered assessment reviewers, monitoring/duty owners and cover require organisation appointments |
| Author / reviewer | Codex at Mark's request; author document checks only; Mark wording/whole-document review pending; independent project reviewer unassigned/deferred |
| Approval / readiness | DEC-091 corroboration and other recorded directions approved; no whole-document, build, activation or readiness determination |
| Change history | 0.5 — GI-CR-01–04 author consistency correction/closure under Mark’s instruction; existing identifiers and proposed/planned status preserved. 0.4 — AOS-25 counterpart/reference alignment only; no requirement/case/contract change. 0.3 — AOS-24 counterpart/reference alignment only; no requirement/case/contract change. 0.2 — AOS-22 counterpart/reference alignment only; no requirement/case/contract change.  0.1 initial draft reconciling GIL v2 through comparison content v0.2 and applying DEC-086/090/091; new component records, no new architectural decision or IF |

## 1. Purpose and scope

AOS-23 makes the quality, currency and evidential basis of governance artefacts assessable and contestable. It answers: what does this artefact contain, what claims can its evidence support, what permitted evidence bears on actual practice, what has changed, and who must review or act? Without it, the organisation can mistake a polished document, stale policy, unexplained score or quiet monitoring run for sound governance.

The component owns permitted ingestion and normalisation, artefact classification, entity-specific applicability and assessment configuration, evidence-linked findings and uncertainty, review states, artefact/source currency monitoring, owned alerts and assessment contributions to governance reporting cycles. Under DEC-091, separately permitted records, outcomes and human-supplied interviews/surveys may corroborate documentary claims. Document quality, support for a claim and evidence of practice remain separately reported. A record that supports a claim does not by itself prove institutional effectiveness.

AOS-21 owns corpus, profiles, source admission, approved criteria and precedent stewardship. AOS-22 owns cross-domain synthesis, interpretation and options; AOS-24 faithful presentation; AOS-25 drift, aggregate/system oversight and independent review; AOS-30 human decisions and accepted duties. AOS-13 coordinates operational handoffs, AOS-14 external retrieval/exchange, and AOS-01–05 common controls/records. AOS-23 does not acquire human moral authority, amend criteria or governing instruments by itself, observe protected deliberation, infer personal feelings/preferences, issue automatic legal/governance certificates or replace the board portal.

Boards and committees, stewards, assessment validators, executives, residents, staff, source/operational owners, reviewers and operators have distinct interests and powers. Parent/subsidiary assessments retain separate entity scope, applicable powers and corpus under DEC-090; group membership is not disclosure permission.

## 2. Authority and sources

FP v4/RP v6 govern; architecture decisions constrain the proposed requirements. GIL is the starting material after explicit reconciliation, not a competing authority register or coding instruction. Each requirement below is a functional derivation unless directly applying a cited decision. The source keys provide precise version/locator references throughout.

| Key | Source and locator / standing |
| --- | --- |
| FP | Foundational_Principles_v4.docx, principles 1–10; governing settlement |
| RP1/2/3 | RP v6 Architecture and Completeness: closed feedback and named accountability; Mode 1/Mode 2 Boundary: permanently human judgement and boardroom; 1+5 Architecture: roles and cross-domain handoff |
| RP4 | RP v6 Options and Decisions: actual organisational state, explicit assumptions and decision feedback |
| RP5/7 | RP v6 Blind Spots and Honesty / Radical Transparency: missing evidence, uncertainty, audit and limits |
| RP6 | RP v6 Ethics and Telos: purpose-led design, no-exit condition, developer-framework and precedent drift distinctions |
| RP8/9 | RP v6 Agentic Delegation / Data and Sensing Boundaries: delegated tools/powers, protected reporting and declared purpose |
| GT | Governance_Intelligence_Tests.docx, M1.1–14/M2.1–15; software contributions and human assessment limits in §8 |
| GIL | GIL_Technical_Specification_V2.docx v2.0, §§1.1–1.4, 2.3–2.5 assessment/calibration/blind spots, §3 monitoring, §4 library, §§6.1–6.5 processes, §§7–9 limitations/build questions |
| CMP | GIL Comparison and Reconciliation filename v0.1, content v0.2, GIL-C01–38 and approved Q01/Q02; disposition allocation in §19 |
| D | AOS-00 v0.27 DEC register; particular approved decisions cited per row |
| C | AOS-21 v0.1 §§3–7/9–11/13/19; sourced profiles, catalogue, permitted evidence, change and approval/precedent boundaries |
| GI | AOS-20 v0.3 §§3–7/10–15; charter, canonical analysis, graduated review, protected duty and common research |
| H | AOS-30 v0.3 §§5–7/9–12; human approval, duty acceptance, correction and outcome feedback |
| E/A/U/X/K | Core v0.6 REC-E/Q, REC-A, REC-D, REC-X; Shared v0.10 §4; Register v0.9 KX views; coordination v0.2 and protected reporting/recovery v0.1 |
| R | DEC-086; template v0.4 §4.4; AOS-04 v0.8 §§3.1/5.1/6.6/10.8 CON-009; AOS-02 v0.8 §6.6 CON-007; AOS-01 v0.8 §§6.6/10.8 |

The preserved source manifest remains unchanged. Current regulatory/standards statements require admitted primary evidence, jurisdiction/status/effective-date checks and empowered applicability review. This draft neither verifies current law nor claims ISO clause conformity. GIL's sixth-peer/adjudication, blanket board-record exclusion, review-before-any-UDL-write, numerical confidence/deadline defaults and local authority-register assumptions are replaced by the approved architecture. Vendor/schema/API/build choices remain deferred.

## 3. Responsibilities

| Responsibility | AOS-23 owns | Other owner / reserved boundary |
| --- | --- | --- |
| Ingestion/classification | Permitted extraction, normalisation and exact artefact revision/type/context | 02 custody; 03 use; 21 admitted sources and uncertain entity reconciliation |
| Assessment applicability | Apply approved criteria to exact entity/profile/source scope; expose exclusions and unknowns | 21 criterion stewardship; 01/30 normative approval; application never amends meaning |
| Findings/corroboration | Evidence-linked question responses, document quality, claim support, practice evidence and uncertainty | 22 synthesis/options; human reviewers validate; broader effectiveness remains human/25/30/40 |
| Monitoring | Artefact currency/applicability, approved source changes and owned alerts | 21 updates corpus; 14 external access; 04 shared agents; 25 system/aggregate oversight |
| Reporting cycles | Assessment coverage/status, alerts, evidence conflicts and owner-confirmed action state | 22 cross-domain synthesis; 24 narrative/projection; 30 approval and duties |
| Corrections | Reassess dependent findings and communicate changed analysis/status | 02 impact; 21 corpus; 30 human account/decision review; no silent rewriting of minutes |
| Own external research | Relevance of developments challenging assessment/monitoring adequacy | Common R services/records; 14 retrieval; 01 human amendment and activation |

Operational roles include accountable assessment owner, validator, corpus Steward, monitoring owner, duty tracker, recipient/cover, privacy/control owners and independent assessor. An executive, Company Secretary or ARC Chair may exercise a role only through evidenced applicable powers. No universal approval route or administrator override is created.

## 4. Capabilities and functions

### 4.1 Capabilities

| ID | Outcome |
| --- | --- |
| AOS-23-CAP-001 | Ingest and classify permitted exact artefact/evidence revisions |
| AOS-23-CAP-002 | Apply scoped, current-for-purpose assessment criteria without normative self-amendment |
| AOS-23-CAP-003 | Produce evidence-linked multidimensional findings with explicit uncertainty |
| AOS-23-CAP-004 | Preserve graduated review and canonical output status |
| AOS-23-CAP-005 | Monitor change/currency/coverage and deliver owned alerts |
| AOS-23-CAP-006 | Contribute faithful assessment/status evidence to governance reporting cycles |
| AOS-23-CAP-007 | Reassess material corrections and preserve action/outcome feedback |
| AOS-23-CAP-008 | Research developments affecting AOS-23 and propose governed adaptation |

### 4.2 Functions

| ID | Trigger → evidence → behaviour → output; boundary and failure |
| --- | --- |
| AOS-23-FUN-001 | Submission/request → source revision and current controls → classify/extract with completeness limits → scoped normalised input; ambiguous/prohibited content withheld or referred |
| AOS-23-FUN-002 | Assessment trigger → 21 profile/corpus/criteria and purpose → select applicable questions with rationale → versioned assessment configuration; unresolved material applicability blocks favourable reliance |
| AOS-23-FUN-003 | Permitted assessment → artefact and separately permitted corroboration → question/criteria analysis and evidence comparison → provisional findings in three distinct dimensions; gaps remain explicit |
| AOS-23-FUN-004 | Findings ready → exact analysis and required review profile → submit/validate/return/dispute → canonical status/revision; review cannot grant action authority |
| AOS-23-FUN-005 | Approved change/time/event trigger → artefact/source/currency evidence → detect material change and actual coverage → alert/currentness finding; no-check/no-change distinguishable |
| AOS-23-FUN-006 | Alert/protected concern → exact finding and duty profile → permitted routing/accepted owner/cover → tracked human handoff; no executive suppression of protected classes |
| AOS-23-FUN-007 | Reporting cycle → scope/period plus assessments, coverage, alerts and owner-confirmed actions → consolidate assessment inputs and flag relational conflicts → canonical cycle contribution for 22/24/30 |
| AOS-23-FUN-008 | Material correction/configuration change → affected old/new dependencies → selective reassessment/review → revised findings/status and consumer notifications; history/effects not silently reversed |
| AOS-23-FUN-009 | Action/outcome update → accepted human/operational evidence → link actual result to finding/cycle and unresolved duties → feedback for 25/30; report publication is not resolution |
| AOS-23-FUN-010 | Approved research trigger → external evidence via 14 → specialist relevance/impact evaluation → common research finding/disposition/change proposal; no autonomous adoption |

### 4.3 Proposed requirements

Rows are component requirements except category I (interface). Categories: G governance, D data, Q assessment quality/uncertainty, S use/security, O operation, R research. Every row has proposed status for v0.1 functional scope, origin 7 October 2026. Requirement owner is the accountable AOS-23/GI owner; delegated reviewers/monitoring owners perform relevant duties. Project approver is Mark; actual organisation approvers derive from 01/30 instruments. Dependencies are the cited source/control, function contract in §6 and owned setup gaps in §17. Each row provides its own rationale, precise source/derivation and planned VER acceptance link. These common attributes complete every requirement record without duplicating metadata. No case is executed and no unresolved setting is an operating default.

| ID | Proposed obligation | Category / FUN | Exact source / derivation | Rationale | Planned VER |
| --- | --- | --- | --- | --- | --- |
| AOS-23-REQ-001 | AOS-23 shall bind each assessment input to its exact source and content revision. | D; 001 | GIL §6.2; E/REC-E; C CON-001 | Prevents assessment of unidentified or silently changed material. | 001 |
| AOS-23-REQ-002 | AOS-23 shall retain the distinct entity scope of each artefact and corroborating assertion. | D; 001 | DEC-090; C §§4/6; GIL-C12/38 | A parent profile cannot replace subsidiary powers/context. | 001 |
| AOS-23-REQ-003 | AOS-23 shall expose material extraction/normalisation omissions or failures before dependent assessment claims. | Q; 001 | GIL §6.2 steps 1–3; RP5/7; E | Partial parsing must not look like complete evidence. | 002 |
| AOS-23-REQ-004 | AOS-23 shall obtain current independent authority, data-use and execution permission for each dependent operation. | S; 001 | A/U/X; coordination CHECK; DEC-064/067 | Technical access cannot authorise processing or effects. | 001/031/032 |
| AOS-23-REQ-005 | AOS-23 shall refer uncertain artefact classification for the confirmation required by its approved classification profile. | Q; 001/002 | GIL §6.2 step 1; C/FUN-003; RP5 | A guessed type cannot silently determine governing criteria. | 003 |
| AOS-23-REQ-006 | AOS-23 shall bind each assessment configuration to exact entity/profile/corpus/criterion revisions and purpose. | D; 002 | GIL §6.2 step 3; C CON-002/004; RP4 | Makes configuration and context reconstructable. | 004 |
| AOS-23-REQ-007 | AOS-23 shall record the rationale and authority basis for applicable and excluded criteria. | Q; 002 | GIL §2.3 calibrations; C §4; DEC-080 | Exclusions must be justified rather than convenient. | 004 |
| AOS-23-REQ-008 | AOS-23 shall refer a proposed change of governing criterion meaning through AOS-21 and the empowered change route before adoption. | G; 002 | DEC-080/081; GIL-C15/27/31; C §7 | Applying criteria is distinct from adopting new meaning. | 005 |
| AOS-23-REQ-009 | AOS-23 shall use current-for-purpose organisation context from AOS-21 rather than assuming the last annual report remains sufficient. | D; 002 | GIL §6.1 reconciled by GIL-C12/27; C §10.1 | Later context can materially change applicability. | 004 |
| AOS-23-REQ-010 | AOS-23 shall retain unresolved material applicability or missing required criteria as a limitation on dependent favourable reliance. | Q; 002 | GIL-C04/13/19; RP5/7; C ISS-002/003 | Unknown applicability cannot become a default pass. | 003/004 |
| AOS-23-REQ-011 | AOS-23 shall link each substantive question response or finding to the assessed criterion and supporting exact evidence references. | D; 003 | GIL §2.4/6.2; E/REC-E; RP7 | Allows interrogation of what supports the assessment. | 006 |
| AOS-23-REQ-012 | AOS-23 shall retain supporting source references separately from linked fact-assurance assessments. | D; 003 | DEC-047/062/063; E/REC-Q | Provenance alone is not assurance of a fact. | 006 |
| AOS-23-REQ-013 | AOS-23 shall preserve material conflicting or contesting evidence in the finding and its review request. | Q; 003 | GI REQ-016/017; RP5/7; GIL-C16 | Prevents an apparently coherent answer concealing dispute. | 006 |
| AOS-23-REQ-014 | AOS-23 shall report document quality, support for a claim and evidence of actual practice as distinct assessment dimensions. | Q; 003 | DEC-091; CMP Q02; GIL-C16 | A good document and sound practice are different propositions. | 007 |
| AOS-23-REQ-015 | AOS-23 shall use corroborating records, outcomes and human-supplied interview/survey evidence only within their separately permitted assessment purpose. | S; 003 | DEC-091; U; C REQ-035; RP9 | Corroboration cannot expand sensing or secondary use by default. | 007/008 |
| AOS-23-REQ-016 | AOS-23 shall qualify absence findings by the assessed source, question and coverage rather than treating documentary silence as absence of practice. | Q; 003 | GIL §2.4 ratings; GIL-C16; RP5 | Absence from a document has bounded meaning. | 002/009 |
| AOS-23-REQ-017 | AOS-23 shall not treat low complaint volume, disengagement or missing responses as evidence of satisfaction or consent. | Q; 003 | FP7; RP6 no-exit; GT M2.7 | No-exit and consent cannot be inferred from silence. | 009 |
| AOS-23-REQ-018 | AOS-23 shall expose uncertainty and limitations without substituting model confidence for approved assurance or review. | Q; 003 | DEC-084; GI §4; GIL-C17; RP7 | A numerical score cannot validate a fact or decision. | 010 |
| AOS-23-REQ-019 | AOS-23 shall preserve provisional status when recording or supplying unvalidated assessment material under permitted graduated access. | G; 004 | DEC-084; GIL-C08; GI §§5/6 | Recording is possible without false promotion to formal validity. | 011 |
| AOS-23-REQ-020 | AOS-23 shall withhold formal validated reliance until the human review required for that exact purpose is evidenced. | G; 004 | DEC-084; GI REQ-021–028; GIL §6.2 step 8 | Formal use must match the approved validation policy. | 011 |
| AOS-23-REQ-021 | AOS-23 shall bind human validation to the exact analysis revision, reviewer capacity, scope, outcome and limitations. | D; 004 | GI §6; H §§5/6; K/KX-22/06 | An old or partial review cannot approve a later whole assessment. | 012 |
| AOS-23-REQ-022 | AOS-23 shall preserve analysis/report approval separately from decision validity/evidence, record authentication, minutes approval and actual action authority under DEC-103. | G; 004/007 | DEC-103; H §10.3; K/KX-06 v0.3 | A report reviewer or Chair is not automatically the board. | 012 |
| AOS-23-REQ-023 | AOS-23 shall not represent artefact assessment as automatic legal compliance or institutional governance-effectiveness certification. | G; 003/004 | GIL §1.2; DEC-005/091; GT introduction | Documentary support cannot settle broader human judgement. | 008/013 |
| AOS-23-REQ-024 | AOS-23 shall perform artefact monitoring only within a valid profile specifying scope, triggers, indicators, review and duty conditions. | O; 005 | GIL §3; DEC-054–057/086; R/04 | Agent count/schedule cannot silently supply monitoring authority. | 014 |
| AOS-23-REQ-025 | AOS-23 shall obtain external monitoring evidence through permitted Boundary retrieval and source verification. | O; 005 | AOS-14-IF-001; GIL-C07/21; RP8/9 | No direct bypass or blanket external API prohibition. | 014 |
| AOS-23-REQ-026 | AOS-23 shall record actual complete, partial, failed, cancelled or not-performed monitoring coverage. | Q; 005 | GIL §3 logs; GIL-C21; RP5 | Missed checking must remain visible. | 015 |
| AOS-23-REQ-027 | AOS-23 shall qualify a no-material-change result by its checked scope, method, period and limitations. | Q; 005 | GIL-C21; RP5/7 | Quiet output is not complete currency assurance. | 016 |
| AOS-23-REQ-028 | AOS-23 shall distinguish publication, consultation/adoption, jurisdiction and effective-date status when assessing source currency. | D; 005 | GIL §3; GIL-C14/21; C REQ-010/011 | A new publication may not be currently applicable. | 016 |
| AOS-23-REQ-029 | AOS-23 shall bind each material monitoring alert to evidence, affected artefact/configuration revisions and declared urgency basis. | D; 005/006 | GIL §3/6.4; E; K/KX-07/19 | An alert must expose what changed and why it matters. | 017 |
| AOS-23-REQ-030 | AOS-23 shall retain required handoff responsibility until an accountable permitted owner or cover accepts it. | O; 006 | DEC-066/071/075; K/KX-21/26; H | Delivery alone cannot establish human responsibility. | 018 |
| AOS-23-REQ-031 | AOS-23 shall preserve overdue or failed review/delivery duties under the approved cover/escalation profile. | O; 006 | DEC-071/075; H §§10/11; GIL-C30 | Unresponsive recipients cannot silently close a concern. | 018 |
| AOS-23-REQ-032 | AOS-23 shall route findings in approved mandatory protected classes without discretionary executive suppression or normal report-release delay. | G; 006 | DEC-083/084; protected reporting annex §§3–6; RP8 | Protects safety/welfare, telos, Mode 2 and assurance-failure findings. | 019 |
| AOS-23-REQ-033 | AOS-23 shall bind each reporting-cycle contribution to its exact scope, period and assessment/input revisions. | D; 007 | GIL §6.3; K/KX-22; RP4 | A report needs a reconstructable evidence window. | 020 |
| AOS-23-REQ-034 | AOS-23 shall expose provisional/disputed assessments, coverage gaps and unresolved duties in reporting-cycle contributions. | Q; 007 | DEC-084; GIL §6.3; RP5/7 | Cycle publication cannot hide unfinished review or missing territory. | 020 |
| AOS-23-REQ-035 | AOS-23 shall preserve report release, delivery, action approval, accepted ownership and completed outcome as distinct states. | G; 007/009 | GIL-C29/34; DEC-066/087; H/KX-26 | Approval/publication does not close actions or establish effects. | 022 |
| AOS-23-REQ-036 | AOS-23 shall identify and selectively reassess materially dependent findings when source, profile, criterion or governing control revisions change. | I-D; 008 | DEC-068/069; K/KX-13; C §10.4; GI §6.5 | Avoids stale assessment without a blanket unrelated freeze. | 023 |
| AOS-23-REQ-037 | AOS-23 shall constrain dependent reliance when correction impact or required reassessment remains materially unresolved. | Q; 008 | DEC-063/067/089; coordination; H | A known uncertainty cannot be silently treated as resolved. | 024 |
| AOS-23-REQ-038 | AOS-23 shall refer material inter-artefact relationship conflicts requiring broader synthesis to AOS-22 with supporting evidence and limits. | I-D; 007 | GIL §6.3 step 5; Map AOS-22/23; GI §3 | Artefact checks must not acquire cross-domain moral adjudication. | 021 |
| AOS-23-REQ-039 | AOS-23 shall communicate materially changed analysis/status and actual action/outcome evidence to affected review owners, including AOS-30 when its workflow is affected. | I-D; 008/009 | K/KX-13/21/26; GI §6.5; H §10; RP1 | Closes analytical feedback without rewriting approved accounts/effects. | 023/030 |
| AOS-23-REQ-040 | AOS-23 shall maintain its own external-research remit against exact assessed component/dependency revisions and status. | R; 010 | DEC-086; R; template §4.4 | Adequacy research differs from document currency monitoring. | 025 |
| AOS-23-REQ-041 | AOS-23 shall conduct external research through permitted Boundary retrieval and current common task/use/execution controls. | S; 010 | R; A/U/X; AOS-14-IF-001 | Research does not create extra access or emergency powers. | 025/029 |
| AOS-23-REQ-042 | AOS-23 shall record research through the common profile/run/finding/disposition views. | R; 010 | R; 02 §6.6 RSVIEW-0.1 | Avoids competing local research state definitions. | 025 |
| AOS-23-REQ-043 | AOS-23 shall bind research findings to exact evidence/status/dates, uncertainty and affected specification elements. | R; 010 | R; RP5/7; DEC-086 | Makes specialist challenge grounded and reviewable. | 026 |
| AOS-23-REQ-044 | AOS-23 shall refer proposed specification/criterion changes through empowered human amendment before adoption. | G; 010 | DEC-086/080/018; 01 §§6.6/10.8; C §7 | Run completion or proposal acceptance is not normative approval. | 028/029 |
| AOS-23-REQ-045 | AOS-23 shall report actual research coverage and bounded no-material-finding outcomes with their limitations. | R; 010 | R; RP5; GIL-C21 | No finding cannot imply successful checking of all sources. | 027 |
| AOS-23-REQ-046 | AOS-23 shall route shared research findings to each materially affected component owner under its permitted duty profile. | R; 010 | DEC-086; R; K/KX-26 | Shared infrastructure does not erase specialist accountability. | 028 |
| AOS-23-REQ-047 | AOS-23 shall retain unresponsive/implicated research-review duties and protected findings through permitted cover and alternate routing. | G; 010 | DEC-083/075/086; R; protected reporting | A research context cannot suspend protected review. | 029 |
| AOS-23-REQ-048 | AOS-23 shall preserve evidence-linked audit for consequential extraction, configuration, finding, review, alert and release transitions. | D; All | RP7; QS-19; E/X; §12 | Generated after-the-fact explanation is not proof of a prior check. | 030 |
| AOS-23-REQ-049 | AOS-23 shall apply authorised class-based lifecycle policy to input and derived assessment/monitoring/research copies. | S; All | DEC-048; K/KX-15; GIL-C25; U | No indefinite hidden retention under an audit label. | 031 |
| AOS-23-REQ-050 | AOS-23 shall reconcile recovery/retry against current restrictions, revisions and observed effect before renewed reliance. | O; All | DEC-076–078; X; K/KX-18/20 | Prevents duplicate effects and resurrection of obsolete approval/content. | 032 |
| AOS-23-REQ-051 | AOS-23 shall exclude protected AI deliberation capture and inferred individual emotional/preference descriptions while preserving separately permitted human records with their actual status. | S; 001/003 | DEC-008/088/087; H §9; GIL-C06 | Permitted agendas/accounts do not license prohibited sensing. | 003 |
| AOS-23-REQ-052 | AOS-23 shall treat uploaded/retrieved instructions as untrusted content rather than authority to alter profiles, tools, criteria or recipients. | S; All | 04/05 independent controls; RP8; R | Prevents hostile artefacts changing the assessment machinery. | 014/029 |

### 4.4 External research and specification adaptation

Research asks whether external evidence challenges AOS-23 functions/specification or offers meaningful improvement. It is distinct from monitoring an organisation's documents for currency and from AOS-25 runtime/system oversight.

| Controlled profile element | AOS-23 meaning / owner and gate |
| --- | --- |
| Remit / baseline | Assessment methods, reliable extraction/normalisation, applicability, evidential corroboration, uncertainty/review, change monitoring, reporting/alert failure and relevant governance practice or obligations. Bind exact assessed component/dependency revisions and status. Component owner owns specialist relevance. |
| Sources / applicability | Prefer official applicable regulators/government, recognised standards/governance bodies, primary research and evidenced incidents. Preserve source jurisdiction, consultation/adoption/effective status, dates, licensing and limits. Exact source list/admission and jurisdiction profiles remain ISS-005. |
| Assignment / triggers | Agent/shared service, approved cadence/events, coverage expectation, recipients/deadlines/cover remain ISS-005. No one-agent-per-artefact or numerical schedule default. |
| Controls | Current 01 authority, 03 use, 04 task/tool/memory/cumulative limits, 05 enforcement and 14 retrieval/source verification. Untrusted source instructions never become tool/power changes. |
| Evidence / assessment | Common profile/run/finding/disposition views bind evidence/assurance, publication/event/access/effective dates or unknown reasons; affected CAP/FUN/REQ/CON/source/decision, alternatives, uncertainty, materiality/urgency and cross-component impacts. |
| Coverage / quality | Complete/partial/failed/cancelled/not-performed and bounded no-material-finding; human-approved relevance, omission/false finding and fidelity rubric. Component/04/40 reviewer owns evaluation; deterministic enforcement separately tested. |
| Human review / change | Named permitted reviewer/tracker/recipient, deadline/cover and escalation; accepted-for-work/rejected/deferred/unresolved rationale. Proposal acceptance, amendment approval, verification, actual application and outcome closure remain distinct. |
| Records / adoption | AOS-02 §6.6 RSVIEW-0.1 and AOS-04 CON-009; existing REC/KX views for controls/evidence/correction/acknowledgement/duties. Exact mapping/compatibility is ISS-004; no competing local research dictionary. |

Normal: approved trigger → permitted evidence/coverage → specialist assessment → human disposition → governed change if warranted → verified/applied revision and outcome review. Degraded: denied access, failed source, stale baseline or partial check → explicit limitation → owned coverage exception and permitted retry/fallback. Urgent live implications use separately authorised protected human response while amendment work remains pending. Research cannot expand tools/sensing, change governing criteria or reopen deferred exploratory self-calibration.

## 5. State model

Dimensions are separate: valid ingestion does not imply applicable criteria; reviewed analysis does not imply action approval; an approved action does not imply actual completion.

| Object / states | Entry, transition, authority, evidence and failure |
| --- | --- |
| Input: received → classified/normalised or partial/held/rejected | Exact source and current use/control checks; extraction/type uncertainty visible. Missing material or ambiguous sensing scope is referred, not treated as complete. |
| Configuration: proposed → confirmed/applicable or unresolved → superseded/restricted | Exact entity/corpus/criteria revisions and applicability rationale; empowered approval required where governing meaning changes. No automatic self-calibration. |
| Assessment: provisional → submitted → validated-for-declared-purpose/returned/disputed → superseded/withdrawn | Common canonical review binds exact revision/reviewer/scope and limitations. Provisional content can be recorded and accessed under approved controls; formal validated reliance awaits required review. |
| Monitoring run: assigned → complete/partial/failed/cancelled/not-performed | Record actual coverage/status/evidence. No-material-finding is bounded to checked scope and method, not proof of complete currency. |
| Alert/duty: detected → routed → accepted → response/outcome review → closed/unresolved | Receipt, accepted ownership, actual action and resolution distinct. Approved deadlines/cover apply; expiry triggers review/escalation, never approval by silence. |
| Reporting cycle: scoped → assembling → review → approved-for-defined-release → delivered → follow-through | Status identifies remaining provisional/disputed inputs and open duties. The particular report approver's valid route applies; approval is not board minutes approval or action completion. |
| Correction: identified → affected reliance marked → reassessed/reviewed → notified/applied → consequences reviewed | Preserve old/new exact revisions; pending reliance constrained selectively. Human account/decision correction remains with 30. |
| Research | Inherit common 04 §5.1 and 02 §6.6 research states; a completed run is neither amendment nor deployment approval. |

Each transition retains controlling revision, actor, purpose, evidence and required acknowledgement. Missing/invalid mandatory profile values withhold dependent transition; applicable independent reporting/service duties continue. Terminal rejection of an assessment does not erase a protected finding or required action/outcome review.

## 6. Semantic contracts and interfaces

CON views complement existing IF identifiers without allocating new IFs. AOS-02 owns structures; each existing semantic owner retains meaning. Component assessment output is canonical analysis under AOS-20-IF-001 when it enters that workflow, with exact purpose/review status rather than a competing report truth store.

| ID | Purpose / producer → consumer | Common definition, minimum meaning and failure |
| --- | --- | --- |
| AOS-23-CON-001 | Artefact/corroboration input: source owners/21/02/permitted humans/14 → 23 | AOS-02-IF-001, REC-E/Q; KX-01/08/09/10/15. Exact entity/type/source/version, extraction completeness, separate assurance and use. Unknown/partial/conflicting input cannot claim complete validated support. |
| AOS-23-CON-002 | Applicable profile/corpus/criteria: 21/01/03 → 23; applicability findings → 21/reviewer | 21 CON-001/004, REC-E/Q/A/D, KX-05/09/13. Exact criteria and entity/purpose/effective scope; application is not normative adoption. Material conflict is held/referred. |
| AOS-23-CON-003 | Current controls and execution: 01/03/04/05 → 23; actual results → 02/25/control owners | REC-A/D/X, CHECK/ACT/CHG/ACC/RSV/WHD and KX-02/03/04/18/20. Independent authority/use/runtime checks, cumulative task limits, actual effect and scoped recovery. Missing controls/unknown effects remain blocked/indeterminate. |
| AOS-23-CON-004 | Assessment/cycle canonical content: 23 → 20/22/24/25/30/permitted reviewers | AOS-20-IF-001; KX-22 and REC-E/Q. Question/criterion, three assessment dimensions, evidence, assumptions/limits, requested review, exact revision and status. Renderings/reports do not promote claims or change substance. |
| AOS-23-CON-005 | Human validation/decision/action outcome: authorised humans via 30/01/13 → 23/02/25 | AOS-30-IF-001 and KX-06 v0.3/17/21/26. Reviewer powers and exact validation scope separate from evidenced decision and separately approved minutes, accepted duties and actual outcomes. Unsupported approval/completion remains unresolved. |
| AOS-23-CON-006 | Ordinary/protected alerts: 23 → 13/30/affected domain owners, protected 05 route | AOS-13-IF-001; KX-07/19/26/21 and protected reporting. Exact evidence/class/urgency/permitted audience, owner/cover/deadline, receipt versus acceptance and outcome. No suppression or executive gate for mandatory protected classes. |
| AOS-23-CON-007 | Material correction/currency impact: 21/02/01/03/source owners → 23; 23 → affected 20–25/30 | KX-13/15/21; coordination impact. Old/new dependencies, effective scope, reason, affected findings and remaining duties. Reconcile out-of-order/duplicate messages against current state; no automatic historical reversal. |
| AOS-23-CON-008 | Own external research: approved profile/agent using 14 → 23 reviewer/affected owners; disposition → change tracker | 02 §6.6 RSVIEW-0.1, 04 CON-009 and existing REC/KX. Exact baseline/remit/evidence/coverage/impact/human disposition; no research approval creates powers or application. |
| AOS-23-CON-009 | Disclosure/lifecycle/recovery: 03/02/05/14 ↔ 23/permitted output recipients | KX-14/15/18/20/23, REC-D/X, AOS-14-IF-001. Permitted projection, class-based retention/deletion, location and actual recovery outcomes. Partial/unknown results remain explicit. |

All views inherit exact organisation/entity/actor/revision references, common known/unknown/withheld states, date precision/time basis, source units for quantities, supported definition versions and reviewed compatibility. Assessment categories and currencies need governed vocabularies; no local score/unit conversion is implicit. Numerical scores are optional only under an approved method/profile, never universally required. Physical types/cardinalities, transport/API, performance and timing values remain implementation/profile dependencies in ISS-004/006.

Ordering and duplicate identity are declared by source/entity/assessment/cycle/duty scope. Repeated inputs can share provenance without erasing different evidence or review duties. Receipt, validation, application and responsibility acceptance are purpose-specific stages; retries use current controls and known effect. Correction/revocation propagates materially dependent use and review. No wire compatibility or consumer implementation is inferred from functional adoption.

## 7. Authority and decision boundaries

Approved Mode 1 assessment/monitoring may classify, analyse, compare, flag and recommend human investigation. Configuration applies admitted approved criteria and actual scoped context. New meaning, constitutional interpretation, moral trade-off, criteria adoption, action authority and deployment remain separately governed. Neither a model recommendation nor confident assessment amends a rule or makes a decision.

Graduated review under DEC-084 permits appropriately labelled provisional recording/access. Validated formal reliance requires the exact declared human review. Urgent mandatory findings use protected routing without waiting for normal report sign-off. Protected duties under DEC-083 cannot be suppressed by an executive; alternate empowered recipients and cover apply if implicated or unavailable.

Live protected deliberation stays outside AI sensing. Permitted pre-meeting documents and authorised human post-meeting accounts may be assessed with their real status. Minute-taker drafting, Company Secretary stewardship, Chair draft approval and decision validity/evidence and separate minutes approval remain distinct under DEC-087. Non-board report approvals use their valid route. An assessment reviewer or ARC Chair does not become board decision authority by approving a report.

Meaningful constraint explanations identify the reason, effect and review route by default; recorded security/privacy/feasibility exceptions may limit disclosure without waiving enforcement. Unresolved material authority/evidence withholds dependent automated reliance selectively, retaining separately permitted service/reporting duties. No inferred personal context, autonomous normative calibration or automatic reversal of actual effects is authorised.

## 8. Reasoning principles applied

| Foundation / RP domain | Application and limit |
| --- | --- |
| FP1/2/8; RP2 | Human telos/Mode 2 and valid powers constrain configuration, review and recommendations; source standards and scores do not decide which good yields. REQ-008/019–023/032/044. |
| FP3/9; RP6 | Purpose-led criteria, no-exit and developer-framework evidence remain distinct from compliance claims. REQ-014/015/017/023; 25/30 own broader integrity judgement. |
| FP4; RP7 | Exact citations, limitations, review and action evidence are legible through permitted projections. REQ-001/011/012/021/035/048. |
| FP5/6; RP1/5 | Extraction gaps, conflicting evidence, partial coverage, failure and unknown outcomes remain explicit. REQ-003/010/016–018/026–029/037/050. |
| FP7; RP6 | Low complaints, disengagement or absent evidence cannot be treated as satisfaction/consent. REQ-017; resident experience evidence requires purpose-permitted assessment, not invented inference. |
| FP10; RP3/8 | Owned cross-domain handoff, changes and bounded research support adaptation without guaranteeing predictable emergent behaviour. REQ-030–034/036–047. |
| RP4 | Exact actual entity/context and sourced claims support downstream options; 22 owns cross-domain synthesis and infeasible alternatives. REQ-002/005–009/014/015/038. |
| RP9 | Independent use, privacy and source/derivative lifecycle restrict ingestion, corroboration and output. REQ-004/020/049/051/052. |

All ten FP principles and nine RP domains are applied without treating them as automated certification criteria.

| GI Tests | AOS-23 contribution / reserved judgement |
| --- | --- |
| M1.1/5 | Artefacts and permitted practice evidence contribute to strategy/performance picture; 22/25/30 assess wider coherence |
| M1.2/3/14 | Assess sensing/risk/Golden Thread artefacts and their supporting evidence; domain owners retain actual operational information and safety accountability |
| M1.4 | Assess board skills/composition documentation and permitted corroboration; human assessors judge real capability |
| M1.6/7/10 | Compare applicable declared standards/arrangements with permitted evidence; no automatic compliance certificate or proof that norms are followed |
| M1.8/9 | Assess feedback/value-for-money artefacts and evidence; silent residents/self-reported measures do not establish legitimacy or value |
| M1.11/12/13 | Link findings/actions/outcomes and limitations for learning/oversight; 25 evaluates aggregate and emergent effects |
| M2.1/2/3/4 | Surface commitments, trade-offs, contradictory evidence and requested human challenge; no AI adjudication or inference of unspoken concern |
| M2.5/11 | Supply permitted evidence for independent review and preparation; genuine dissent and collective sense-making require human assessment |
| M2.6/7/8 | Preserve purpose-bound evidence and accessible reasoned findings; records/surveys alone cannot establish legitimacy/no-exit responsiveness |
| M2.9/10/12 | Assess documented purpose/boundaries and signal conflicts; human constitutional/oversight judgements remain reserved |
| M2.13/14/15 | Examine artefact claims and permitted evidence concerning developer frameworks, purpose-led design and telos/function; 25/30/40 assess institutional adequacy |

All 29 tests have explicit contribution/limits; none is awarded a pass. Human Mode 2 assessment may notice what documents cannot show. Permitted corroboration does not license AI in-room observation or substitute documentary scoring for that judgement.

## 9. Data, privacy and disclosure

Process governance artefacts and separately permitted contextual/evidential material for the declared assessment, monitoring, reporting or research purpose. Retain original assertions, extraction/normalisation limits, corroboration source and separate assurance. Human-supplied interviews/surveys require their own valid use scope; presence in a repository is insufficient. Emotional/preference descriptions are human-provided/confirmed and purpose-bound under DEC-088, with no individual inference, sentiment scoring or automatic calibration.

Entity/group boundaries, sensitive findings, private preparation and permitted disclosure use AOS-03 controls. AOS-24 renders canonical content; AOS-14 handles external exchange. Reports may disclose relevant substance and limits without unrestricted personal/boardroom content. Audience filtering cannot turn a provisional/disputed finding into validated analysis or remove a material uncertainty without an authorised, reviewable basis.

02/03/05 class policies govern source copies, extracted text, prompts, answers, embeddings/indexes, assessments, projections, research and backups. No blanket permanent/seven-year/two-year retention default is inherited. Permitted audit evidence of correction/deletion does not justify retaining deleted payload. Conflicting holds/retention/deletion duties need empowered review and explicit restricted/unresolved state.

## 10. Behaviour and workflows

### 10.1 Ingestion and applicability

Approved request → current authority/use/control → exact source/entity/type → extraction with completeness/format limits → classification confirmation if required → scoped 21 corpus/profile/criteria → question applicability and rationale → confirmed or unresolved configuration. A multipart or multi-entity artefact can produce scoped assessments; it must not silently flatten different governing powers. Applicable documents can include permitted drafts or approved accounts, preserving status. Protected capture is rejected/held; an agenda/minutes keyword alone does not prove prohibition.

### 10.2 Assessment and corroboration

Scoped configuration → artefact claims and separately permitted records/outcomes/human evidence → question-specific analysis → citations, conflicts, assumptions and uncertainty → three distinct dimensions → provisional canonical findings/questions/recommendations → declared review → validation-for-purpose or returned/disputed status. “Absent from document”, “asserted”, “not provided” and “not applicable” have explicit scope/reason. None automatically means absent in practice. Interviews or survey suggestions are proposals; new evidence is obtained only under separately valid powers and use.

### 10.3 Human review and reporting cycle

Approved cycle scope/period → exact assessments/status and coverage → alerts and owner-confirmed action evidence → criteria-defined inter-document checks → relationship conflicts/unknowns sent to 22 as needed → reviewed canonical cycle contribution → 24 faithful presentation → empowered release approval via 30 → recorded delivery and ongoing duties → actual outcome feedback. A partial/provisional report can be prepared under permitted graduated access but cannot label unvalidated findings as formally validated. A cycle cut-off does not suppress urgent later evidence; a supplement/change record preserves its relationship to the earlier report.

### 10.4 Monitoring and handoff

Approved periodic/event trigger → specified internal artefact/source currency indicators and permitted external evidence via 14 → actual coverage/currentness/change assessment → no-material-change or alert with limits → relevant ordinary or protected routing → accepted accountable owner/cover → action/investigation/outcome review → closure only for satisfied duties. Different artefact types may share agents/infrastructure; no fixed 168-hour/120-hour or 4/8/24/72-hour rule is adopted. Timings are controlled urgency/capacity profiles. Wrong-jurisdiction, draft or future-effective changes remain distinct.

### 10.5 Corrections and feedback

Material source/corpus/profile/permission/model change → identify exact affected assessments/pending reliance → selective restriction/reassessment → new analysis revision and required review → notify 20/22/24/25 and materially affected 30 preparation/account/outcome workflow → accepted responsibility/application evidence → consequence review. AOS-23 revises its assessment; 21 maintains source/precedent; 30 obtains human account/decision review. No component silently rewrites approved minutes, invents earlier validation or reverses actual effects. Delayed/duplicate changes reconcile current authoritative state.

Accepted action/outcome evidence links back to findings and later cycles. An action's reported completion can itself be unassessed/disputed; owner confirmation alone does not establish every fact. Unresolved effectiveness or unintended consequences remains visible to 25/30 rather than closing on report publication.

## 11. Failure, escalation and recovery

Unextractable/partial content, unknown type/entity, missing criteria, material contradictory applicability or inaccessible required evidence is recorded as limitation and held/referred for dependent claims. A partial assessment can proceed only within separately permitted scope and labelled limits; it cannot fabricate coverage. Unknown controls block dependent operation while valid independent duties remain.

Unresponsive reviewer, failed delivery or missing cover leaves an owned unresolved duty under approved escalation profiles. Protected concern cannot wait for discretionary executive/ARC release. Ordinary alerts do not acquire emergency powers merely by using urgent language. Independent human response routes and actual capacity require commissioning evidence.

Interrupted assessment/publication, unavailable UDL, partial execution and unknown effect use common 02/05 recording/recovery. Preserve actual state, control evidence and pending delivery; do not claim that an unrecorded assessment was delivered or validated. Retry reconciles current revision, restrictions and known effects before reprocessing/release. Recovery cannot revive deleted input, revoked purpose or obsolete approval. Human fallback uses bounded permitted evidence and makes limitations explicit.

## 12. Evidence, provenance and audit

Reconstruct trigger/request → exact artefact and corroboration → extraction/configuration → actor/current controls → method/model and applied criteria → finding and rationale → human review → routing/release → accepted action → observed result/correction/intervention → outcome review. Record evidence versus inference, rejected/conflicting inputs where permitted, time basis, source/fact assurance, material uncertainty and remaining duties.

Reasoning means source-linked answers, applied rules, model outputs and approved human rationale. Private chain-of-thought is not required; a generated retrospective explanation cannot prove an earlier check. 02 owns shared custody and schemas, 20 canonical analysis, 21 corpus and 23 assessment meaning. Evidence copies remain subject to lifecycle/privacy policy.

## 13. Security and operational requirements

Treat uploaded and externally retrieved text as untrusted data. Enforce task/tools/use/authority/runtime bounds independently of model assessment. User-supplied documents cannot alter the agent profile, assessment rules, permitted recipient or governing corpus. Protect reviewed analysis against unauthorised writes; human amendments produce exact revised records with scope/status.

Approved profiles govern workload, timing, review/cover, availability, extraction quality, alert relevance and source coverage. Missing values have owners/gates, not invented defaults. Human-reviewed contrasting fixtures evaluate citation fidelity, material omission, inappropriate applicability, false/missed alerts, assurance confusion, entity leakage and three-dimension separation. Optional scores require validated purpose-specific methods; model confidence alone is not assurance. Model/configuration changes require proportionate affected-function evaluation under 04/05/40. Deterministic control/review-status enforcement is assessed separately from probabilistic analytical quality.

## 14. Invariants

| ID | Binding invariant / requirement links | Planned VER |
| --- | --- | --- |
| AOS-23-INV-001 | Exact scoped artefact/criteria/evidence stay bound; REQ-001/002/005/006/011 | 001–003/006 |
| AOS-23-INV-002 | Document quality, claim support and practice evidence never collapse into certification; REQ-014/015/023 | 007/008/013 |
| AOS-23-INV-003 | Missing evidence/coverage does not become validated absence, satisfaction or currency; REQ-003/010/016/017/026/027 | 002/003/009/010/015/016 |
| AOS-23-INV-004 | Provisional recording is not formal validation or action/board approval; REQ-019–022/035 | 011/012/022 |
| AOS-23-INV-005 | Protected duties remain owned and cannot be executive-suppressed; REQ-030–032/047 | 018/019/029 |
| AOS-23-INV-006 | Material corrections change exact assessment/status through review, not historical decision/effects; REQ-036/037/039 | 023/024/030 |
| AOS-23-INV-007 | Research proposes and all processing/recovery remains permitted; REQ-040–044/049–052 | 025–032 |

## 15. Conformance and acceptance

All cases are planned. Common configuration: exact document-control baseline, approved synthetic fixtures or expressly permitted real evidence, declared entity/profile/criteria/review/control settings except deliberately invalid paths. Procedure triggers the stated function/input, observes analysis/states/controls and tracks required deliveries/reviews/effects. Evidence includes input/output revisions, configuration, controls, citations, human review/rubric, acknowledgements and actual outcomes. Competent component/control assessors review technical evidence; empowered humans assess semantic judgement and review adequacy; independent institutional review remains separate.

| ID | REQs | Case / input and procedure | Expected acceptance and retained evidence |
| --- | --- | --- | --- |
| AOS-23-VER-001 | 001/002/004 | **Exact artefact and group scope:** Parent and subsidiary artefacts/corroboration have different powers; submit valid and denied-purpose variants. | Preserve exact revisions/entity/purpose; no inherited parent powers or unauthorised processing. Common evidence/assessor rules above apply. |
| AOS-23-VER-002 | 003/016 | **Partial extraction:** Corrupt/missing pages or failed table extraction affect a question. | Expose omissions/failure; do not conclude absence from unparsed content or claim complete assessment. Common evidence/assessor rules above apply. |
| AOS-23-VER-003 | 005/010/051 | **Classification and permitted records:** Ambiguous type, unavailable criteria, live board capture, personal sentiment inference and permitted draft/approved account variants. | Refer uncertain classification/applicability; exclude prohibited sensing; permitted human records retain actual approval status. Common evidence/assessor rules above apply. |
| AOS-23-VER-004 | 006/007/009/010 | **Scoped applicability:** Two entities, an updated operational fact and a future-effective criterion alter applicability; one required source is missing. | Exact profile/criterion versions and inclusion/exclusion rationale retained; unknown remains restricted; annual report not sole current context. Common evidence/assessor rules above apply. |
| AOS-23-VER-005 | 008 | **Configuration versus normative amendment:** Assessment service proposes a new criterion/meaning and tries applying it as approved. | Refer 21/empowered change; no self-adoption or autonomous normative calibration. Common evidence/assessor rules above apply. |
| AOS-23-VER-006 | 011/012/013 | **Citations, assurance and conflict:** Question answer cites a document; separate fact validation is partial and corroboration contests the claim. | Preserve exact criterion/citations, separate assurance and material conflict; no source-as-truth promotion. Common evidence/assessor rules above apply. |
| AOS-23-VER-007 | 014/015 | **Three dimensions:** Policy is well written but an asserted claim lacks support and permitted outcomes suggest weak practice. | Report quality, claim support and practice evidence distinctly; source/use restrictions retained. Common evidence/assessor rules above apply. |
| AOS-23-VER-008 | 015/023 | **Permitted corroboration and effectiveness limit:** Human-supplied interview and outcome records support one practice claim but do not cover governance generally. | Use only permitted sourced evidence; report bounded support without automatic effectiveness/legal certification. Common evidence/assessor rules above apply. |
| AOS-23-VER-009 | 016/017 | **Silence and no exit:** Artefact omits a topic; complaint/response volumes are low or absent. | Documentary absence stays scoped; no inference of absent practice, resident satisfaction or consent. Common evidence/assessor rules above apply. |
| AOS-23-VER-010 | 018 | **Confidence versus assurance:** Model offers high score despite missing evidence; optional scoring method has no approved calibration. | Expose uncertainty and method limits; score neither satisfies assurance nor substitutes for human review. Common evidence/assessor rules above apply. |
| AOS-23-VER-011 | 019/020 | **Graduated review:** Provisional finding is recorded/accessed under approved purpose; request formal validated use before review. | Allow permitted labelled recording; withhold unsupported formal validated reliance; no review-before-every-UDL-write rule. Common evidence/assessor rules above apply. |
| AOS-23-VER-012 | 021/022 | **Exact review and approval powers:** Reviewer validates one revision/purpose; a later changed revision, Chair-approved draft and board-approved decision coexist. | Preserve scope/revision and distinct approval powers; old review/report approval cannot validate new analysis or board minutes. Common evidence/assessor rules above apply. |
| AOS-23-VER-013 | 023 | **Certificate attempt:** Output labels documentary assessment a governance or legal compliance certificate. | Reject/return unsupported certification; retain evidence-qualified findings and human institutional judgement. Common evidence/assessor rules above apply. |
| AOS-23-VER-014 | 024/025/052 | **Controlled monitoring and hostile sources:** Approved profile checks an external source via 14; uploaded/source text instructs new tools/recipient or bypass. | Common current controls/Boundary applied; instructions remain content; no profile/power alteration or mandatory per-type agent. Common evidence/assessor rules above apply. |
| AOS-23-VER-015 | 026 | **Actual monitoring coverage:** Complete, partial, failed, cancelled and unperformed run variants. | Distinct statuses and actual checked sources/indicators retained; no implied complete run. Common evidence/assessor rules above apply. |
| AOS-23-VER-016 | 027/028 | **Currency and no change:** Consultation, wrong-jurisdiction/future-effective rule and a no-change result from a limited check. | Status/dates/applicability remain distinct; bounded no-change cannot establish complete currentness. Common evidence/assessor rules above apply. |
| AOS-23-VER-017 | 029 | **Evidence-linked alert:** Material policy/currency change affects selected artefacts and assessment configuration. | Bind evidence/old-new revisions/urgency basis and affected scope; no uncited generic alarm. Common evidence/assessor rules above apply. |
| AOS-23-VER-018 | 030/031 | **Accepted handoff and capacity:** Receiving owner confirms receipt but not duty acceptance; deadline expires and primary delivery fails. | Retain responsibility duty, approved cover/escalation and evidence; no receipt-as-resolution. Common evidence/assessor rules above apply. |
| AOS-23-VER-019 | 032 | **Protected finding and suppression:** Finding meets approved protected class; executive asks delay until report approval or is implicated. | Use protected permitted alternate route; owned response persists without executive veto; no extra external authority. Common evidence/assessor rules above apply. |
| AOS-23-VER-020 | 033/034 | **Cycle scope and unfinished inputs:** Cycle includes reviewed/provisional/disputed findings, missing artefacts and unresolved prior duties; late material evidence arrives. | Bind exact period/revisions, expose all limits/status; late evidence enters governed supplement/review, not silent omission. Common evidence/assessor rules above apply. |
| AOS-23-VER-021 | 038 | **Inter-artefact conflict:** Relationship check finds contradictory delegations and a cross-domain value tension. | Record criterion/evidence conflict; send broader synthesis/human question to 22/30; no autonomous moral winner. Common evidence/assessor rules above apply. |
| AOS-23-VER-022 | 035 | **Report versus outcome:** Report is approved/delivered while an action lacks accepted owner or observed completion. | Distinct release/delivery/action/acceptance/outcome states; cycle publication does not close outstanding duties. Common evidence/assessor rules above apply. |
| AOS-23-VER-023 | 036/039 | **Material correction and human workflow:** 21 source correction affects assessment, prepared pack, pending account and outcome review. | Identify exact affected dependencies, revise/review assessment and notify 30/other owners; no silent minutes rewrite or effect reversal. Common evidence/assessor rules above apply. |
| AOS-23-VER-024 | 037 | **Unresolved impact and selective brake:** Material evidence conflict affects one pending reliance while an unrelated service duty remains authorised. | Constrain dependent use selectively; retain unresolved owner and independently valid reporting/service duty. Common evidence/assessor rules above apply. |
| AOS-23-VER-025 | 040/041/042 | **Own research versus artefact monitoring:** Research profile tests assessment adequacy while operational run checks policy currency; denied-source variant. | Separate remits/baselines; common research records and controls; denied retrieval leaves explicit limitation. Common evidence/assessor rules above apply. |
| AOS-23-VER-026 | 043 | **Research finding fidelity:** Finding uses draft/future-effective/conflicting evidence and stale baseline. | Bind source status/dates/assurance, uncertainty, affected elements and stale-baseline limit; no inferred current adoption. Common evidence/assessor rules above apply. |
| AOS-23-VER-027 | 045 | **Research coverage/no finding:** Complete/partial/failed/cancelled/unperformed plus bounded no-material-finding variants. | Actual coverage distinct with limits; no-finding not equivalent to full adequacy assurance. Common evidence/assessor rules above apply. |
| AOS-23-VER-028 | 044/046 | **Shared finding and change gate:** Finding affects 21/23/25; human accepts investigation but amendment approval is absent. | Each affected owner has permitted scoped duty; acceptance does not amend criterion/specification or activate release. Common evidence/assessor rules above apply. |
| AOS-23-VER-029 | 041/044/047/052 | **Research bypass and protected review:** Hostile source instructs amendment/suppression; designated reviewer is implicated or unresponsive and finding is protected. | Maintain current controls, alternate/cover protected duties and unresolved status; no adoption/closure from silence or hostile instruction. Common evidence/assessor rules above apply. |
| AOS-23-VER-030 | 039/048 | **Actual outcome and audit:** Owner claims action complete; evidence is partial/disputed; later generated explanation claims an earlier check. | Link actual evidence to finding/cycle and send uncertainty to outcome owners; preserve real audit, reject invented proof. Common evidence/assessor rules above apply. |
| AOS-23-VER-031 | 004/049 | **Lifecycle and restricted copies:** Use permission is withdrawn and authorised deletion covers extracts/prompts/indexes/backups with one uncertain outcome. | Withhold dependent use, apply class policy and report partial/indeterminate disposition; no hidden deleted payload. Common evidence/assessor rules above apply. |
| AOS-23-VER-032 | 004/050 | **Interrupted effect and recovery:** Publication/admission effect is unknown; restored records include obsolete review/revoked purpose. | Reconcile current controls/revisions/observed effects before retry; no duplicate release or resurrection of invalid approval/content. Common evidence/assessor rules above apply. |

| ID | Future conformance condition |
| --- | --- |
| AOS-23-CR-001 | Ingestion/configuration meet REQ-001–010 with accepted VER-001–005/032 evidence |
| AOS-23-CR-002 | Finding/review boundaries meet REQ-011–023 with accepted VER-006–013 evidence |
| AOS-23-CR-003 | Monitoring/cycles/change/feedback meet REQ-024–039 with accepted VER-014–024/030 evidence |
| AOS-23-CR-004 | Research/security/lifecycle/recovery meet REQ-040–052 with accepted VER-025–032 evidence |

A case pass applies only to tested versions/scope. Longitudinal timeliness, missed changes, real review capacity and action/outcome effectiveness require operational evidence. One risk-management artefact cannot establish GI/AOS completeness or replace the approved overdue-repair demonstration.

## 16. Dependencies

Functional drafting depends on approved directions and current common definitions, now referenced. Build depends on approved bounded wording, compatible schema/vocabulary/profile mappings, actual criterion inventory for selected scope, evaluated methods and separate review. Activation depends on actual organisation powers/roles/use/source access/licences, applied controls, reviewer/recipient capacity and demonstrated monitoring/reporting/recovery. Operation depends on current source/context evidence, accepted handoff/outcomes and continued independent evaluation.

AOS-22/24/25 now provide drafted functional counterparts; detailed 13/40 drafting remains. All must implement/adopt compatible stated counterpart duties before operational reliance; implementation is not claimed here. AOS-21 is a functional review draft, not an assured live corpus. These dependencies do not require executable schema design before continuing the functional suite.

## 17. Issues and setup gaps

No new general design question is submitted. DEC-091 settles permitted corroboration; DEC-090 scoped entities, DEC-084 graduated review, DEC-083 protected routing and DEC-086 own research remain agreed. The following are owned build/activation/assurance dependencies, not requests to reopen them.

| ID / type / status | Affected scope and gap | Owner / evidence / gate / disposition |
| --- | --- | --- |
| AOS-23-ISS-001 dependency / open | Entity/perimeter, assessment validator, monitoring/duty/recipient/cover appointments and valid powers; CAP-001–007 | Organisation/GI owner with 01/30; approved instruments/appointments; affected build/activation. Apply scoped authority, not role-title defaults. |
| AOS-23-ISS-002 dependency / open | Applicable criteria/catalogue/content, corroboration sources and review/materiality policies; CAP-002–004 | 21/assessment owner/empowered humans; admitted revisions, permitted-use and approved applicability/review policy; affected build/reliance. No universal score or 121-type completeness claim. |
| AOS-23-ISS-003 dependency / open | Monitoring source/indicator/currency and cycle scope/urgency/deadline/cover settings; CAP-005/006 | Monitoring/cycle owners with 21/14/30; approved profiles and coverage/handoff evidence; activation/operation. No inherited timing defaults. |
| AOS-23-ISS-004 dependency / open | Exact shared schemas/vocabularies, counterparts and compatibility; all CONs | 02/semantic owners/consumers; reviewed mappings and integration evidence; implementation/integration. Logical adoption recorded, no physical schema implied. |
| AOS-23-ISS-005 dependency / open | Own research agent/service, sources/jurisdictions/cadence/triggers/reviewer/cover and rubric; CAP-008 | Component/04/14/30/40 owners; approved profile and actual results; research activation. No automation created by this draft. |
| AOS-23-ISS-006 dependency / open | Extraction/assessment/alert quality, optional scoring methodology, service/recovery conditions and executed cases; §§13/15 | Component/04/05/40 and competent human assessors; accepted purpose-specific rubrics and actual evidence; build/activation as applicable. Confidence does not supply assurance. |
| AOS-23-ISS-007 dependency / open | Privacy, disclosure, derived-copy lifecycle/location/holds and recovery; CON-001/003/009 | 03/02/05/organisation; authorised policy and actual flow/control outcomes; activation. No permanent-retention or unrestricted group-sharing default. |
| AOS-23-ISS-008 dependency / open | Full source-row closure, 22/24/25/13/40 counterpart allocation and independent/longitudinal effectiveness assessment; §19 | Project custodian/component/25/40 owners and independent humans; traceability, review and operating evidence; suite/operational assurance. No institutional GT pass inferred. |

## 18. Implementation guidance — non-normative

An extraction/normalisation pipeline, versioned assessment configuration, evidence-linked question responses and an owned alert/cycle view can realise these functions. Existing repositories can provide permitted originals without a new document portal. Shared monitoring/research services may serve separate governed remits. These are patterns, not mandated models, databases, APIs, hosting, formats, agent counts or schedules. A readable report can be useful without imposing GIL's house style or DOCX template on canonical meaning.

## 19. Traceability and change

| Capability / functions | Requirements | Contracts | Principal planned cases |
| --- | --- | --- | --- |
| CAP-001 / FUN-001 | 001–004/051 | 001/003/009 | 001–003/031/032 |
| CAP-002 / FUN-002 | 005–010 | 002/003 | 004/005 |
| CAP-003 / FUN-003 | 011–018/023 | 001/004 | 006–010/013 |
| CAP-004 / FUN-004 | 019–022 | 004/005 | 011/012 |
| CAP-005 / FUN-005/006 | 024–032 | 006/007 | 014–019 |
| CAP-006 / FUN-007 | 033–035/038 | 004/005/006 | 020–022 |
| CAP-007 / FUN-008/009 | 036–039 | 005/007 | 023/024/030 |
| CAP-008 / FUN-010 | 040–047 | 008/003/006 | 025–029 |
| All applicable | 048–052 | 003/009 | 030–032 |

| GIL comparison dispositions | AOS-23 treatment / other owner |
| --- | --- |
| GIL-C03/05/12/13/14/16/17/18/27/28 | Scoped applicability, three dimensions, evidence/uncertainty and human review: REQ-001–023; corpus/criteria adoption stays 21/01 |
| GIL-C06/07/08/23/24/25/26/35 | Permitted input and controls, graduated recording, audit/lifecycle and canonical output: REQ-004/019–022/041/048–052 |
| GIL-C10/19/20/21/22/30 | Governed monitoring, coverage, bounded agents/research and protected duty: REQ-024–032/040–047 |
| GIL-C15/29/31/34 | Human approval, reporting/action distinction, corrections and outcome feedback: REQ-008/022/033–039; 21 stewardship, 30 human accounts, 25 broader oversight |
| GIL-C01/02/09/32/33 | Internal accountable GI/1+5/human boundary and principled assessment reflected §§1/7/8; 22 owns cross-domain options/infeasible alternatives |
| GIL-C04/11/36/37/38 | Sourced scoped catalogue/content from 21; numerical count/technology/API/build defaults deferred. DEC-090/091 scope applied; ISS-002/004/006 remain operating dependencies |

All 38 disposition IDs are accounted for across the two allocation tables and explicit other-owner/deferment routes. Each requirement supplies exact source/derivation, rationale and VER link; VER rows provide reverse coverage. Source matrix addendum records this component allocation without promoting original source statuses or executed assurance. Common definitions and existing IF identifiers are preserved.

Changes record exact affected entity/source/criteria/analysis and REQ/CON/VER revisions, rationale, powers, consumer impacts, approval, actual application and outcome. Model changes and research proposals use common governed change rather than silent recalibration. Preserve rejected/deferred/unresolved outcomes and prior permitted histories; no requirement is retired in v0.1.

## 20. Build and handover

No implementation or live activation is authorised by this draft. Eventual bounded handover fixes approved scope/wording, criterion/content inventory, dependency/contract versions, profiles and acceptance evidence. A builder stops at missing mandatory powers/use/data, unresolved applicability, undefined review/coverage, incompatible contracts or unsupported protected-route/recovery assumptions. Implementation choice remains discretionary within approved behaviour. A separate competent reviewer must walk a normal, exception and authority-boundary case before G3. Deferred project independent review is not replaced by author or AI checks.

## 21. Review and control

Author checks cover template sections, stable identifiers, requirement metadata/source precision, singular obligations, requirement-to-case and reverse links, common ownership, three-dimension/review boundaries, table structure and honest dependencies. No extraction/assessment/monitoring/research run, independent review or institutional effectiveness assessment has been executed.

| QS coverage | Author evidence / remaining limit |
| --- | --- |
| QS-01–04 | Document control/status, scope and source versions explicit; IDs stable in initial draft |
| QS-05–10 | §4.3 row metadata/source/rationale/VER plus shared owner/status/origin; §17 owns unresolved values; no inherited defaults |
| QS-11–14 | §§1/3/5/6/9–11 specify boundaries/contracts/lifecycle/failure; later exact schemas/counterparts remain pending |
| QS-15–20 | §§7–13 cover human powers, uncertainty, operational evaluation, audit and governed learning; actual evidence outstanding |
| QS-21–23 | §§14/15/19 give traceability and normal/negative/degraded/cross-component cases; none executed |
| QS-24–28 | §§16/17/20/21 distinguish author quality checks, design judgement, review and build/activation; no gate or tailoring claimed |

Specification-quality conclusion: organised functional review draft with 52 proposed requirements, nine contract views and 32 planned cases. Design-adequacy conclusion: applies approved corroboration, corpus, review, protection and research directions with visible owned operating dependencies; competent human and operational assurance remain required. Mark's wording/whole-document review is pending. No new general architecture question emerged. Mapped GI drafting is complete including AOS-24/25; next GI-set consistency/disposition review, then AOS-40 scenarios.

## Component summary

**Purpose:** assess governance artefacts and their permitted evidence without confusing documents with governance effectiveness.  
**Owns:** scoped assessment, review status, artefact/source monitoring, alerts and cycle contributions.  
**Receives:** exact permitted artefacts, 21 corpus/context/criteria, separate assurance/corroboration, controls and human review/action evidence.  
**Produces:** multidimensional provisional/reviewed findings, canonical contributions, owned alerts/corrections and adaptation proposals.  
**Own research:** assessment/monitoring adequacy remit using common profiles; operational setup remains owned gaps.  
**Reserved human authority:** normative adoption, moral judgement, formal validation, action/board decisions and institutional assessment.  
**Conformant when:** accepted evidence against the approved bounded requirements/contract/profile baseline; no conformance inferred from drafting.  
**Open dependencies:** actual content/appointments/profiles, compatible implementation mappings, counterpart drafting and operational/independent assurance.


**AOS-22 counterpart adoption — 7 October 2026:** 22 CON-001/002 consumes existing corpus/assessment/context; CON-003 produces canonical synthesis/options; CON-007 exchanges exact correction/feedback/oversight. Ownership and existing source/assurance/review/approval semantics are unchanged. Remaining presentation/oversight drafts are 24/25; implementation mapping/assurance remain later dependencies.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**GI consistency closure — 7 October 2026:** Mark authorised GI-CR-01–04 corrections and closure. Functional drafting, reciprocal report-independence wording, decision/outcome consumer allocation, Mode 2 wording and current completion statements are reconciled. AOS-23 changes counterpart/current references only; its REQ/VER/CON rows are unchanged. AOS-00/Map v0.32, DEC-001–091; AOS-20 v0.5/21 v0.6/22 v0.4/23 v0.5/24 v0.3/25 v0.2/30 v0.5; AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.15/Core v0.6/Exchange Register v0.14/source matrix v0.15; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. The review v0.2 records closure evidence; next AOS-40 acceptance scenarios. Earlier dated baseline/next-step statements remain historical. No new DEC/IF/operating power, case execution or build/activation/readiness approval; independent project review remains deferred and operating human independence remains mandatory.

