# AOS-21 — Corpus, organisation knowledge and precedent

Document: aos-21-corpus-organisation-knowledge-and-precedent · Source revision or record: v0.7

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**DEC-103 adopted — 29 October 2026:** Current revision 0.7. Decision validity/effective time, attributable evidence/authentication, minutes approval and permission to execute are separate. DEC-087 is partly superseded; [decision/amendment and legal-source record](../Supporting-Specifications/aos-dec-103-decision-validity-evidence-and-minutes-2026-10-29.md). No universal later-minutes or second decision-record approval gate. Exact instruments/evidence policy, KX-06 v0.3 compatibility and ordinary separate review/readiness gates remain required; cases unexecuted. Earlier contrary wording is historical only where explicitly identified.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

**AOS-25 oversight counterpart alignment — 7 October 2026:** AOS-25 v0.1 now supplies the drafted oversight/drift/learning and GI research-portfolio counterpart. Reference-only revision; all existing requirement/case/contract rows preserved. AOS-00/Map v0.31, DEC-001–091; AOS-25 v0.1; AOS-20 v0.4/AOS-21 v0.5/AOS-22 v0.3/AOS-23 v0.4/AOS-24 v0.2/AOS-30 v0.4 (counterpart-reference alignment only); AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.14/Core v0.6/Exchange Register v0.13; source matrix v0.14; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. No build/activation/readiness approval. Next: author GI-set consistency/disposition review across AOS-20–25 and AOS-30, then AOS-40 acceptance scenarios under item 8; independent project review remains deferred. Earlier dated consultation/adoption entries remain history.

**AOS-24 presentation counterpart alignment — 7 October 2026:** AOS-24 v0.1 now supplies the drafted faithful-rendering/explanation counterpart. Reference-only revision; requirement, case and contract rows unchanged. AOS-00/Map v0.30, DEC-001–091; AOS-24 v0.1; AOS-21 v0.4/AOS-22 v0.2/AOS-23 v0.3 (reference alignment only); AOS-01–05 v0.8, AOS-14 v0.4, AOS-20 v0.3, AOS-30 v0.3; Shared v0.13/Core v0.6/Exchange Register v0.12; source matrix v0.13; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. No build/activation/readiness approval. Earlier dated consultation/adoption entries remain history.

**AOS-22 synthesis counterpart alignment — 7 October 2026:** AOS-22 v0.1 now supplies the drafted synthesis/interpretation/options counterpart. This revision changes pending-drafting/current-reference statements only; all requirement, case and contract meanings preserved. AOS-00/Map v0.29, DEC-001–091; AOS-22 v0.1; AOS-21 v0.3/AOS-23 v0.2 (counterpart/reference alignment only); AOS-01–05 v0.8, AOS-14 v0.4, AOS-20 v0.3, AOS-30 v0.3; Shared v0.12/Core v0.6/Exchange Register v0.11; source matrix v0.12; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. No build/activation/readiness approval.


**AOS-23 functional counterpart alignment — 7 October 2026:** AOS-23 v0.1 is now drafted and adopts the existing corpus/profile/criteria/evidence/correction views. AOS-21 v0.2 updates pending-drafting references only; all requirements, cases and shared semantics preserved. AOS-00/Map v0.28, DEC-001–091; AOS-23 v0.1; AOS-21 v0.2 (functional endpoint/reference alignment only); AOS-01–05 v0.8, AOS-14 v0.4, AOS-20 v0.3, AOS-30 v0.3; Shared v0.11/Core v0.6/Exchange Register v0.10; source matrix v0.11; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. No build/activation/readiness approval.


| Document control | Value |
| --- | --- |
| Component / version / date | AOS-21 / 0.7 / 29 October 2026 |
| Status | Functional specification review draft; requirement wording proposed |
| Architecture baseline | AOS-00/Map v0.32, DEC-001–091; prior consultation/allocation retained as history |
| Governing sources | Foundational Principles v4; AOS Reasoning Principles v6; Governance Intelligence Tests; preserved controlled source manifest |
| Dependency manifest | AOS-01–05 v0.8; AOS-14 v0.4; AOS-20 v0.3; AOS-30 v0.3; Shared v0.9/Core v0.6/Exchange Register v0.8; Control Coordination v0.2; Protected Reporting and Recovery v0.1; common research supporting view RSVIEW-0.1 and KX-06 v0.3. Shared v0.10/Register v0.9 adoption addenda retain these unchanged definitions; source matrix v0.10 records allocation |
| Quality / template | AOS-QS v0.1; component template v0.4 |
| Project owner / custodian | Mark Sweeny |
| Operational owner | Accountable GI owner and human Governance Knowledge Steward; actual appointments and delegated powers remain organisation dependencies |
| Author / reviewer | Codex at Mark's request; author checks only; Mark review pending; independent project reviewer unassigned/deferred |
| Approval / release | DEC-090/091 approved as directions; no whole-document approval or build/activation/readiness determination |
| Change history | 0.6 — GI-CR-01–04 author consistency correction/closure under Mark’s instruction; existing identifiers and proposed/planned status preserved. 0.5 — AOS-25 counterpart/reference alignment only; no requirement/case/contract change. 0.4 — AOS-24 counterpart/reference alignment only; no requirement/case/contract change. 0.3 — AOS-22 counterpart/reference alignment only; no requirement/case/contract change.  0.2 updates AOS-23 counterpart and current allocation references only; no REQ/VER/CON meaning change. 0.1 initial functional draft incorporating the GIL comparison v0.2, approved group scope and common external-research rule. New supporting adoption addenda reference existing definitions without changing their meanings. |

## 1. Purpose and scope

AOS-21 makes the organisation's knowledge and governing sources identifiable, current for a declared purpose and traceable to the people entitled to maintain or adopt them. Without it, GI can treat an old policy, an unverified factual claim or its own interpretation as current authority. The intended outcome is that a permitted user or component can reconstruct which entity, source, revision, approval, applicability and limitations support a proposition—and see what remains unknown or disputed.

Scope includes organisation and subsidiary profiles; external, operational and constitutional corpus; governance artefact catalogue, relationships and analytical criteria; source admission and currency; human stewardship; approved interpretation/precedent custody; and corpus-related challenge, correction and research. Organisation knowledge means sourced context, not a model's private memory. Corpus admission means permission to include a source for specified uses, not adoption of its propositions as organisational rules.

AOS-02 owns canonical shared structures and custody, AOS-01 governing powers/change, AOS-03 permitted data use, AOS-04 agent behaviour and AOS-05 enforcement/recovery. AOS-14 governs external retrieval. AOS-22 interprets and synthesises; AOS-23 assesses artefacts and permitted corroboration; AOS-24 presents; AOS-25 oversees drift and independent review; AOS-30 supports empowered human decisions. AOS-21 does not create moral authority, assess the whole institution's effectiveness, certify legal compliance, observe protected boardroom deliberation or replace a document portal.

Stakeholders include boards of relevant entities, committees, stewards, executives, residents, staff, source owners, reviewers, operators and suppliers. Their legitimate interests, acting capacities and access differ. A group relationship does not transfer governing powers, data-use permissions or approval between entities.

## 2. Authority and sources

FP v4/RP v6 govern. Approved decisions constrain proposed wording. The working paper and GIL supply reconciled design material, not additional powers. Source locators below apply throughout the requirement register; each requirement is an explicit functional derivation unless labelled as direct adoption of a decision.

| Key | Exact source / locator and use |
| --- | --- |
| FP | Foundational_Principles_v4.docx, numbered principles 1–10; applicability in §8 |
| RP1 | RP v6, Architecture and Completeness: “Every governance process must close its feedback loop”; “Every human accountability layer must be explicitly named” |
| RP2 | RP v6, Mode 1/Mode 2 Boundary: permanently human judgement, governance instruments and protected deliberation |
| RP3 | RP v6, 1+5 Architecture: role clarity and cross-intelligence handoff |
| RP4 | RP v6, Options and Decisions: actual organisational state and structured consequential decision feedback |
| RP5/7 | RP v6, Blind Spots and Honesty / Radical Transparency: named limits, reconstructable behaviour and visible uncertainty |
| RP6 | RP v6, Ethics and Telos: precedent drift paragraph beginning “Where the organisation's purpose is interpreted”; independent founding-text reconciliation; no-exit and developer framework distinction |
| RP8/9 | RP v6, Agentic Delegation / Data and Sensing Boundaries: delegated powers, protected escalation and declared purpose |
| WP | Governance Intelligence: Internal Architecture — Working Paper, “Corpus”, “How the corpus holds meaning”, “Governance of drift” and “Validation regime”; its RP v5 and automatic-confirmation assumptions reconciled through DEC-080/081 |
| GIL | GIL v2 §§2.1–2.2 organisation/knowledge base, §2.3 blind spots, §3 currency monitoring, §4 document lifecycle, §6.1/6.5 calibration/amendment and §9 subsidiary scope |
| CMP | AOS-GIL-v2-Comparison-and-Reconciliation-v0.1.md, content v0.2, GIL-C01–38 and approved Q01/Q02; individual allocation in §19 |
| D | AOS-00 v0.26 decision register: DEC-005/008/010–012/018/024–025/027/045–048/062–078/079–091, as cited by individual requirements |
| GI | AOS-20 v0.3 §§3/4/5/6/7/8/10/15: corpus stewardship, precedence approval, independent review and common research |
| H | AOS-30 v0.3 §§5/6/7/10: exact decision approval, correction, duties and human-provided context |
| E / A / U / X / K | Core v0.6 REC-E/Q, REC-A, REC-D, REC-X; Shared v0.9 §4; Exchange Register v0.8 KX definitions; coordination and reporting/recovery annexes |
| R | AOS-04 v0.8 §§3.1/5.1/6.6/10.8 CON-009; AOS-02 v0.8 §6.6 CON-007; AOS-01 v0.8 §§6.6/10.8; DEC-086/template v0.4 §4.4 |

The source manifest is preserved, not refreshed by this draft. Current legal/standards applicability requires admitted primary evidence and empowered review. No new ISO clause claim or legal verification is made here. The WP's suggestion that Boundary owns corpus updating is reconciled: AOS-21 owns relevance and admission; Boundary owns permitted external access and verification. Its suggested conversation-to-precedent shortcut is replaced by DEC-081 explicit empowered approval.

## 3. Responsibilities

| Responsibility | AOS-21 / human responsibility | Boundary |
| --- | --- | --- |
| Organisation profiles | Steward maintains exact sourced entity-specific context and coverage | 02 mapping/custody; 01 authority; no presumed parent powers over subsidiary |
| Corpus admission | Steward applies delegated classification, source and permitted-use policy; contested meaning referred | Admission is separate from truth, adoption, activation and disclosure |
| Catalogue / criteria | Preserve source-backed artefact types, relationships, questions, applicability and revisions | 23 applies assessment; criterion is not a constitutional instrument |
| Founding/operational corpus | Capture exact approved texts, powers, effective scope and history | 01/empowered humans approve changes; board retains telos amendment |
| Precedent | Store separately approved interpretation with rationale, context and limits; preserve correction/withdrawal | 22 proposes; 30 records human approval; 25 owns drift-review coordination |
| Currency / change | Identify affected knowledge, consumers and owned reassessment; preserve actual applied state | 02 common propagation; consumers own changed analysis/action/account review |
| External research | Component owner owns corpus-related questions and implications; steward reviews source/curation findings | Common agent/control infrastructure may be shared; 14 retrieval; 01 change |

Actual delegated source admission, materiality/classification rules, accountable owners, cover and review deadlines must be organisationally appointed. No job title, technical administrator permission or AI confidence creates those powers.

## 4. Capabilities and functions

### 4.1 Capabilities

| ID | Outcome |
| --- | --- |
| AOS-21-CAP-001 | Maintain sourced organisation and scoped subsidiary knowledge |
| AOS-21-CAP-002 | Supply classified corpus and artefact knowledge with declared applicability |
| AOS-21-CAP-003 | Preserve empowered approval and contestable precedent integrity |
| AOS-21-CAP-004 | Handle currency, dependency changes and coverage limits |
| AOS-21-CAP-005 | Supply permitted, version-bound evidence to GI and human review |
| AOS-21-CAP-006 | Research external developments affecting AOS-21 and propose governed adaptation |

### 4.2 Functions

| ID | Trigger → input → behaviour → output; control and failure |
| --- | --- |
| AOS-21-FUN-001 | Profile request/change → permitted source revisions → reconcile scoped assertions and human confirmation → versioned profile; uncertain entity matches or facts remain unresolved |
| AOS-21-FUN-002 | New/changed source → provenance, status, use permission and classification → delegated admission review → admitted/restricted/rejected source; unresolved authority referred |
| AOS-21-FUN-003 | Catalogue/criteria proposal → source and entity applicability → preserve distinct semantic role and approval → versioned artefact knowledge; absent seed content becomes coverage gap |
| AOS-21-FUN-004 | Human decision/interpretation → exact approved content and powers → validate faithful capture and explicit precedent designation → scoped precedent or pending/rejected candidate; confirmation alone cannot promote |
| AOS-21-FUN-005 | Currency trigger/correction → old/new revisions and dependencies → identify affected use and notify owners → owned reassessment/restriction; failed delivery remains outstanding |
| AOS-21-FUN-006 | GI/human request → purpose, entity, time and permissions → supply applicable evidence bundle → versioned projection and limitations; missing mandatory evidence prevents asserted suitability |
| AOS-21-FUN-007 | Annual/material drift review → permitted founding text and precedent history → supply independent preparation evidence and receive empowered disposition → reaffirm/prune/referral records; independence is not supplied by a second model alone |
| AOS-21-FUN-008 | Approved research trigger → external evidence via 14 → specialist relevance/impact analysis → common finding and tracked human disposition; no autonomous amendment |

### 4.3 Proposed requirements

Each row is a component requirement unless category begins I (interface). Categories G governance, D data, Q quality/uncertainty, S security/use, R research, O operation. Owner: accountable AOS-21/GI owner, with delegated human Steward responsible for curation; approver: Mark for project wording, applicable organisational authority for operating scope. All rows are proposed for the v0.1 functional scope, originating 7 October. Dependencies: cited source/decision, §6 contract for the function, and owned profile/assurance gaps in §17. Rationale is stated individually. Planned acceptance links are to §15; no cases executed. These common metadata apply to every row, avoiding repetition without omitting the QS-08 record attributes.

| ID | Proposed obligation | Category / function | Exact source / derivation | Rationale | Planned VER |
| --- | --- | --- | --- | --- | --- |
| AOS-21-REQ-001 | AOS-21 shall bind each organisation-profile assertion to its exact entity and source revision. | D; FUN-001 | DEC-090; GIL §2.1; E/KX-09 | Prevents unsourced or entity-ambiguous context. | 001 |
| AOS-21-REQ-002 | AOS-21 shall maintain relevant subsidiaries as distinct scoped profiles linked to the parent within the approved organisational remit. | G; FUN-001 | DEC-090; CMP Q01/GIL-C38 | Preserves entity-specific governance rather than implicit parent-only coverage. | 002 |
| AOS-21-REQ-003 | AOS-21 shall retain source and fact-assurance references separately for each profile assertion. | D; FUN-001 | DEC-047/062; E/REC-Q; GIL-C12 | Origin does not prove factual assurance. | 001 |
| AOS-21-REQ-004 | AOS-21 shall preserve unknown, unverified, disputed, restricted and refuted profile states under the common value/assurance definitions. | Q; FUN-001 | DEC-063; E; GIL-C13 | Avoids false defaults and invented certainty. | 003 |
| AOS-21-REQ-005 | AOS-21 shall withhold an entity or assertion reconciliation lacking the confirmation required by its approved mapping/curation policy. | G; FUN-001 | DEC-045/090; K/KX-09; GI §3 | Prevents destructive or unempowered merging. | 002/003 |
| AOS-21-REQ-006 | AOS-21 shall identify the applicable external, operational and constitutional corpus tier for admitted governing material. | D; FUN-002 | GI REQ-009; WP Corpus; DEC-079/080 | Exposes different source roles and change powers. | 004 |
| AOS-21-REQ-007 | AOS-21 shall retain corpus admission as a distinct state from organisational adoption of governing meaning. | G; FUN-002 | DEC-080; WP Corpus; GIL-C15 | Storage cannot enact a norm. | 004 |
| AOS-21-REQ-008 | AOS-21 shall refer disputed authority or proposed new governing meaning to the empowered human decision-maker. | G; FUN-002 | DEC-080/081; GI REQ-008; RP2 | Curation cannot resolve constitutional judgement by default. | 005 |
| AOS-21-REQ-009 | AOS-21 shall retain material source disagreements in the supplied corpus view until an empowered disposition resolves the affected use. | Q; FUN-002 | RP5/7; GI §6; E/REC-Q | Avoids a convenient source selection concealing conflict. | 005 |
| AOS-21-REQ-010 | AOS-21 shall preserve each admitted source's provenance and publication, access and effective-date status, with explicit unknown reasons. | D; FUN-002 | GIL §§2.2/3; E/KX-01; R common views | Distinguishes source chronology from current applicability. | 006 |
| AOS-21-REQ-011 | AOS-21 shall bind source applicability to declared jurisdiction, entity, purpose and relevant scope. | D; FUN-002 | DEC-090; GIL-C14; U/KX-03 | Prevents cross-jurisdiction or cross-entity assumptions. | 006 |
| AOS-21-REQ-012 | AOS-21 shall identify artefact-type, criteria, question and relationship entries by their exact sourced revisions. | D; FUN-003 | GIL §2.2; GIL-C04/14; E | Makes analytical knowledge traceable and extensible. | 007 |
| AOS-21-REQ-013 | AOS-21 shall distinguish analytical assessment criteria from organisational constitutional powers in catalogue views. | G; FUN-003 | Map AOS-21 allocation; GIL-C14; DEC-005 | Avoids treating a quality criterion as authority. | 004/007 |
| AOS-21-REQ-014 | AOS-21 shall record unavailable catalogue or seed content as an explicit unassessed coverage limitation. | Q; FUN-003 | GIL §§2.3/9; GIL-C04/19; RP5 | An empty library is not evidence that no obligation exists. | 007/011 |
| AOS-21-REQ-015 | AOS-21 shall admit or maintain corpus material only within the human Steward's evidenced delegated curation powers. | G; FUN-002/003 | DEC-080; GI REQ-006; A/REC-A | Access privileges do not confer meaning-adoption powers. | 012 |
| AOS-21-REQ-016 | AOS-21 shall bind each admission/maintenance disposition to its exact content revision and accountable actor. | D; FUN-002/003 | RP7; DEC-080; E/A | Makes faithful maintenance distinguishable from silent alteration. | 012 |
| AOS-21-REQ-017 | AOS-21 shall obtain the independently valid data-use permission required for each processing or disclosure purpose. | S; FUN-002/006 | U/REC-D; DEC-049–053; RP9 | Admission/public accessibility cannot waive use controls. | 023 |
| AOS-21-REQ-018 | AOS-21 shall withhold a dependent operation when its required authority or use determination is missing, invalid or revoked. | G; All | A/U/X; coordination CHECK; DEC-064/067 | Prevents favourable reliance on missing controls. | 023 |
| AOS-21-REQ-019 | AOS-21 shall capture the exact attributed decision record, evidence/authentication standing, decision-maker capacity, entity and effective scope under the organisation’s applicable decision and evidence arrangements. | D; FUN-004 | H §§5/6/10; K/KX-06 v0.3; DEC-103/090 | Ensures that decision custody preserves actual approval. | 013/014 |
| AOS-21-REQ-020 | AOS-21 shall require explicit empowered approval of exact meaning, rationale, context and limitations before designating an interpretation as approved precedent. | G; FUN-004 | DEC-081; GI REQ-010; WP meaning | Prevents automatic accumulation of normative case law. | 015 |
| AOS-21-REQ-021 | AOS-21 shall retain ordinary conversational confirmation separately from approved precedent. | G; FUN-004 | DEC-081; GI REQ-011; GIL-C27 | A conversational yes cannot adopt a ruling. | 015 |
| AOS-21-REQ-022 | AOS-21 shall preserve minute-taker drafting, Company Secretary stewardship, decision validity/evidence, record authentication and minutes approval as distinct roles/events/statuses under DEC-103. | G; FUN-004 | DEC-103; H §10.3; K/KX-06 v0.3 | Avoids promotion of a draft through the wrong role. | 013 |
| AOS-21-REQ-023 | AOS-21 shall withhold affected authoritative reliance when attributable evidence is insufficient or disputed under the applicable evidence policy, without universally requiring later minutes approval or treating a Chair signature or extract alone as conclusive decision authority. | G; FUN-004 | DEC-103; H §6.2; GI §6.5 | An extract/signature must be assessed for provenance and actual validity; no conclusive or automatic authority. | 014 |
| AOS-21-REQ-024 | AOS-21 shall preserve the applicable empowered approval route for non-board decisions and precedent dispositions. | G; FUN-004/007 | DEC-081/087; A/KX-06; H §7 | Avoids treating all bodies as the board or a single administrator. | 016 |
| AOS-21-REQ-025 | AOS-21 shall supply permitted founding-text and precedent evidence for independent human reconciliation at least annually and on material drift triggers. Support preparation of the human and GI accounts without reference to each other before comparison, retaining their permitted original accounts and later responses. | G; FUN-007 | DEC-010/011/085; RP6 precedent paragraph; GI REQ-034 | Accumulated interpretation requires an independent founding-text check. | 017 |
| AOS-21-REQ-026 | AOS-21 shall expose source/profile currency as a purpose-specific status under the approved currentness policy. | Q; FUN-005 | GIL §§3/6.1; GIL-C10/27; RP5 | Annual publication or successful retrieval alone does not establish currency. | 008 |
| AOS-21-REQ-027 | AOS-21 shall identify materially dependent consumers and use scopes when a corpus/profile/precedent revision changes. | I-D; FUN-005 | K/KX-13; coordination §5; DEC-068/069 | Finds where new evidence affects reliance. | 008/018 |
| AOS-21-REQ-028 | AOS-21 shall issue governed change notifications to materially affected owners, including AOS-30 when preparation, account or outcome review is affected. | I-O; FUN-005 | K/KX-13/21; GI §6.5; H §10 | Avoids leaving a human workflow reliant on corrected evidence. | 018 |
| AOS-21-REQ-029 | AOS-21 shall retain required notification, responsibility-acceptance and reassessment duties until each purpose-specific completion condition is evidenced. | O; FUN-005 | DEC-066/071/075; K/KX-21/26 | Delivery is not accepted ownership or resolution. | 019 |
| AOS-21-REQ-030 | AOS-21 shall preserve the distinction between record correction and a new governing decision when applying an empowered disposition. | G; FUN-005 | DEC-089; H §10; K/KX-13 | Clerical correction cannot enact or reverse a decision. | 009 |
| AOS-21-REQ-031 | AOS-21 shall bind each supplied corpus bundle to its entity, purpose, relevant time basis and selected source revisions. | I-D; FUN-006 | E; K/KX-01/14/22; RP4 | Makes the exact context of downstream reasoning reconstructable. | 020 |
| AOS-21-REQ-032 | AOS-21 shall preserve permitted-use and disclosure restrictions in all supplied corpus views. | S; FUN-006 | U; K/KX-14; RP9 | Retrieval cannot create unrestricted secondary use. | 020/023 |
| AOS-21-REQ-033 | AOS-21 shall apply the authorised record-class lifecycle disposition to originals and derived corpus copies. | S; All | DEC-048; K/KX-15; GIL-C25 | Avoids perpetual hidden content retained as audit evidence. | 010 |
| AOS-21-REQ-034 | AOS-21 shall retain permitted historical approval and applied-revision evidence when later changes alter current applicability. | D; FUN-005/006 | DEC-064/068/089; K/KX-13; E | A later state must not rewrite what actually occurred. | 009/020 |
| AOS-21-REQ-035 | AOS-21 shall distinguish supplied documentary claims from separately sourced assurance or corroborating evidence. | Q; FUN-003/006 | DEC-091; E/REC-Q; RP6 no-exit; GIL-C16 | Supports assessment without claiming that documents prove practice. | 021 |
| AOS-21-REQ-036 | AOS-21 shall distinguish justified non-applicability, intentional exclusion, missing evidence, unseeded knowledge and unassessed scope in its coverage records. | Q; FUN-005/006 | GIL-C19; RP5; GI §8 | Different limitations cannot be collapsed into reassurance. | 011/022 |
| AOS-21-REQ-037 | AOS-21 shall maintain its component-specific external-research remit against exact assessed specification/dependency revisions. | R; FUN-008 | DEC-086; R; template §4.4 | Separates adaptation research from document currency monitoring. | 024 |
| AOS-21-REQ-038 | AOS-21 shall use the common research profile/run/finding/disposition views for its research records. | R; FUN-008 | R; 02 §6.6 RSVIEW-0.1 | Avoids competing research evidence and status definitions. | 024 |
| AOS-21-REQ-039 | AOS-21 shall bind research findings to evidence, source status/dates, uncertainty and exact affected elements. | R; FUN-008 | R; RP5/7; DEC-086 | Makes source-to-challenge reasoning assessable. | 025 |
| AOS-21-REQ-040 | AOS-21 shall report actual research coverage, including partial, failed, cancelled, not-performed and bounded no-material-finding outcomes. | R; FUN-008 | R; GIL-C21; RP5 | Quiet output is not proof of complete checking. | 026 |
| AOS-21-REQ-041 | AOS-21 shall obtain external research evidence through permitted Boundary retrieval and current common controls. | R; FUN-008 | R; A/U/X; AOS-14-IF-001 | Prevents source/tool instructions bypassing authority or data use. | 027 |
| AOS-21-REQ-042 | AOS-21 shall route research findings to permitted reviewers and materially affected component owners under the approved duty profile. | R; FUN-008 | DEC-086; R; K/KX-26 | Shared evidence still has distinct component obligations. | 028 |
| AOS-21-REQ-043 | AOS-21 shall retain research disposition duties unresolved when required reviewer acceptance or response is absent. | R; FUN-008 | R; DEC-075; K/KX-21/26 | Unresponsive review cannot silently close a finding. | 029 |
| AOS-21-REQ-044 | AOS-21 shall use the protected reporting route for findings within the approved mandatory classes despite an instruction to suppress them. | G; FUN-005/008 | DEC-083; RP8; protected reporting annex §§3–6 | Ensures a corpus/research concern can reach alternate empowered humans. | 029 |
| AOS-21-REQ-045 | AOS-21 shall refer any proposed specification or governing amendment through the applicable empowered change process before adoption. | G; FUN-008 | DEC-086; AOS-01 §§6.6/10.8; DEC-018 | Research acceptance or publication is not amendment/activation approval. | 028/029 |
| AOS-21-REQ-046 | AOS-21 shall preserve an evidence-linked audit record for consequential admission, selection and precedent transitions. | D; All | RP7; QS-19; E/X; §12 | Provides real evidence rather than retrospective generated proof. | 030 |
| AOS-21-REQ-047 | AOS-21 shall exclude protected AI boardroom capture and inferred individual emotional/preference descriptions from its corpus inputs. | S; FUN-002/004/006 | DEC-008/088; H §9; RP2/9 | Permitted approved records cannot become a route to prohibited sensing. | 023 |
| AOS-21-REQ-048 | AOS-21 shall reconcile restored/retried corpus operations against current restrictions and observed effect before renewed reliance. | O; All | DEC-076–078; K/KX-18/20; X | Recovery must not resurrect obsolete powers, deleted content or duplicate effects. | 030 |

### 4.4 External research and specification adaptation

This is research into AOS-21 adequacy, distinct from routine monitoring of a stored document's currency, AOS-23 organisational assessment and AOS-25 runtime/aggregate oversight. It inherits R common definitions; CON-007 is a view, not a separately invented research schema.

| Controlled profile | AOS-21 allocation / owner and gate |
| --- | --- |
| Remit / baseline | Changes affecting corpus governance, source provenance, knowledge curation, organisational/group semantics, precedent integrity, effective-date/supersession methods, licensing/access or trustworthy retrieval. Assess exact AOS-21 and dependency revisions and approval status. Owner: component owner/Steward. |
| Sources / jurisdiction | Prefer applicable regulators/government, authoritative governance/standards bodies, primary knowledge/provenance research and evidenced incidents. Distinguish consultation, enacted/adopted and future-effective material. Exact approved source list, jurisdiction, admission/licensing rules remain ISS-003/006. |
| Assignment / triggers | Agent/shared service and approved cadence/event/coverage settings remain ISS-006. No per-artefact deployment or schedule is mandated. |
| Controls | 01 authority, 03 use, 04 task/tool/memory/cumulative limits, 05 enforcement, 14 retrieval and verification. Public availability does not confer unrestricted reuse. Retrieved instructions remain untrusted data. |
| Evidence / assessment | Common profile/run/finding/disposition views bind sources and assurance, publication/event/access/effective dates or unknown reasons, affected CAP/FUN/REQ/CON/source/decision, alternatives, uncertainty, materiality/urgency and cross-component impacts. |
| Quality / coverage | Complete/partial/failed/cancelled/not-performed coverage and bounded no-material-finding. Human-approved relevance, missed/false finding and fidelity rubric; no numeric default. Owner: component reviewer with 04/40; ISS-006/007. |
| Human review / change | Named permitted reviewer, tracker, deadline, cover and escalation; accepted-for-work/rejected/deferred/unresolved rationale. Amendment approval, verification, actual application and outcome closure remain separate under 01/30. Protected urgent implications use existing reporting routes. |
| Records / adoption | 02 §6.6 RSVIEW-0.1; KX-13/21/26 and REC-E/Q/A/D/X. Duplicate/correction/lifecycle/reassessment semantics are common. Exact schema and consumer compatibility are later ISS-004 dependencies. |

Normal path: approved trigger → permitted research → coverage/evidence → AOS-21 relevance and impact → human disposition → approved change if warranted → applied revision and reviewed outcome. Degraded path: denied/failed source or stale baseline → explicit partial/failed coverage → owned exception and safe limitation → retry under current controls or human fallback. Urgent reporting continues under separately valid powers while amendment is pending. Research cannot expand sensing/tools, self-approve normative change or reopen DEC-018.

## 5. State model

These are semantic states, not database enums. Records retain independent dimensions; an admitted source can still contain disputed facts, and an approved decision can still be unapplied.

| Object / states | Entry, transition, authority and failure |
| --- | --- |
| Source: received → admission pending → admitted/restricted/rejected | Receipt preserves permitted provenance; delegated admission decision binds purpose/scope. Unknown authority/use remains pending/restricted. Currency change can mark stale/disputed/superseded without erasing history. |
| Profile assertion: unassessed/partial/disputed → validated for purpose | Evidence/assurance and empowered confirmation support the transition; use restrictions and validity remain. Material correction reopens affected suitability; no default false. |
| Governing instrument: proposal → empowered approved → applicable/applied → superseded/withdrawn | 01 governs approval and actual application; effective dates and entity scope constrain use. Storage/admission does not perform these transitions. |
| Precedent: candidate → explicit approved/rejected → applicable/restricted → corrected/withdrawn | Empowered approval of exact meaning, context, rationale and limits required. Later correction preserves earlier record; dependent review and actual effects remain separately tracked. |
| Impact case: detected → owners notified → responsibility accepted → reassessed → closed/unresolved | 02/13/30 acknowledgement semantics apply. Profile deadlines/cover govern timeout; delivery or closure of one consumer does not close remaining duties. |
| Review: due/triggered → preparation → human disposition → follow-through | Annual and material-trigger duties retained. Missing independent preparation or recipient leaves owned unresolved duty. Closure requires evidence of required outcome, not merely a report. |
| Research | Inherit AOS-04 §5.1 and AOS-02 §6.6 profile/run/finding/disposition states; run completion is not change approval. |

Restrictions, withdrawal and revocation take effect through current common controls. Terminal rejection can close a candidate, while residual safety, reporting, retention or review duties remain open. Deadline expiry never creates consent or approval.

## 6. Semantic contracts and interfaces

No new approved IF is introduced. CON IDs identify AOS-21 views of existing common definitions. Source facts and derived assertions use REC-E with separate REC-Q assurance; governing interpretations use the existing approval/change semantics. Component-specific entity/tier/catalogue/precedent references qualify common meaning without duplicating physical schemas.

| ID | Purpose / producer → consumer | Authoritative meaning and failure |
| --- | --- | --- |
| AOS-21-CON-001 | Scoped source/profile evidence: source owner/Steward/14/02 → 21/20/22/23/25 | AOS-02-IF-001, REC-E/Q; KX-01/08/09/10/15. Exact entity/source revision, assertion versus assurance, dates, purpose and limitations. Disputed mapping or mandatory gaps prevent validated suitability. |
| AOS-21-CON-002 | Authority/use/execution: 01/03/04/05 → 21; outcomes → 02/control owners | AOS-01-IF-001, REC-A/D/X; KX-02/03/04 and coordination CHECK. Source admission cannot grant authority or use; absent/invalid control withholds dependent operation. |
| AOS-21-CON-003 | Governing decision and precedent: empowered humans via 30/01 → 21/02/25 | AOS-30-IF-001, AOS-01-IF-002; KX-06 v0.3/05/13. Exact approval/powers/rationale/entity/effective scope; Chair draft approval distinct from decision validity/evidence and separate minutes approval; explicit precedent designation. Ambiguous approval remains pending. |
| AOS-21-CON-004 | Corpus selection and analytical references: 21 → 20/22/23/24/25/30 | REC-E/Q, KX-01/08/14/22; AOS-20-IF-001 applies when the output is canonical analysis. Bundle binds exact requested scope, selected revisions, selection criteria and gaps. Presentation must not imply a new conclusion or approved rule. |
| AOS-21-CON-005 | Correction/currency/dependency: 21/02/source owner/01/03 → affected 20–25/30 and control owners | KX-13/15/21; coordination change/impact. Old/new revision, effective scope, reason, owners and remaining duties. Stale/duplicate/out-of-order messages reconcile authoritative state; no automatic effect reversal. |
| AOS-21-CON-006 | Precedent review/protected referral: 21/independent reviewer/25 → empowered 30/Committee; dispositions → 21/01 | KX-17/22/06/19/26; Shared escalation and protected reporting. Independent preparation, self-assessment distinction, accepted owner/cover, exact review outcome. No executive suppression or receipt-as-resolution. |
| AOS-21-CON-007 | Own external research: approved profile/agent using 14 → 21 reviewer/affected owners; human disposition → change tracker | AOS-04 CON-009/AOS-02 §6.6 RSVIEW-0.1, existing REC/KX views. Exact baseline/evidence/coverage/impact/disposition; no autonomous amendment or competing research dictionary. |
| AOS-21-CON-008 | Lifecycle/recovery/disclosure: 03/05/02/14 → 21; permitted status/results → requestor/30 | KX-14/15/18/20/23 and REC-D/X. Purpose-bound projection and class-based lifecycle; partial/unknown deletion/recovery remains explicit. No unrestricted replay of obsolete authority/content. |

All views inherit shared organisation/identity/revision references, date precision/time basis, units where applicable, known/unknown/withheld states, exact definition versions and reviewed compatibility. Tier labels and entity types require controlled vocabulary; numerical quantities retain their source units. No physical field types, cardinalities, transport/API or timing defaults are selected here. ISS-004 owns later mappings.

Ordering is per declared entity/source/case scope, not a universal total order. Duplicate recognition preserves independent sources and each duty. Receipt, validation, application and human-responsibility acceptance are declared by exchange purpose; information-only delivery need not invent a duty. Failed validation retains reason and owner; retries check current permission and known effects. Revocation/correction reaches materially dependent consumers under CON-005. Producers and consumers must use compatible exact semantics before operational reliance; the linked register records current versus pending adoption.

## 7. Authority and decision boundaries

Delegated Mode 1 processing may classify, extract, reconcile, retrieve and propose under valid profiles. Routine faithful capture of an already approved text differs from deciding what that text means. The human Steward can maintain sources within explicit delegation; contested authority, new normative interpretation and amendments go to empowered humans. AOS-21 cannot select a convenient conflicting source or infer that newest publication supersedes a constitutional instrument.

Only the empowered board changes telos; applicable constitutional procedure and entity powers remain under AOS-01. Schedule amendment follows DEC-025, not a generic librarian/admin approval. For board records, minute-taker, Company Secretary stewardship, Chair draft approval and board approval are distinct under DEC-087. Non-board decisions use their own valid approval route. Approved minutes do not automatically designate every statement as precedent or demonstrate that an action occurred.

Constraints explain their governing reason and review route by default; recorded security/privacy/feasibility exceptions may limit explanation without waiving enforcement. Revoked authority, disputed material evidence or unresolved use blocks materially dependent automated reliance while separately authorised service/reporting duties continue. No autonomous normative self-calibration, emotional inference, retrospective effect reversal or blanket freeze is authorised.

## 8. Reasoning principles applied

| Foundation / reasoning | AOS-21 contribution and limit |
| --- | --- |
| FP1/2/8; RP2/6 | Founding purpose and human moral authority preserved through tier/power/precedent separation; software stores evidence rather than holding intrinsic telos. REQ-006–008/019–025. |
| FP3/9; RP6 | Organisation's purpose, developer framework evidence and analytical/legal references distinguished; compliance mapping validates rather than creates purpose. REQ-006–008/035. |
| FP4; RP7 | Exact sources, approval, limitations and accountable rationale are reconstructable through permitted views. REQ-003/010/019/031–034/046. |
| FP5/6; RP1/5 | Unknowns, conflicts, gaps, failed monitoring and degraded dependencies remain visible; no confidence-as-truth. REQ-004/009/014/026–030/036/043/048. |
| FP7; RP6 | Profiles and corpus do not interpret low complaints or absent engagement as consent/satisfaction. AOS-21 supplies permitted context; 11/22/23/25/30 retain broader assessment. REQ-035. |
| FP10; RP3/8 | Entity boundaries, aggregate precedent review, cross-component impact and bounded adaptation are explicit. REQ-001/002/027–030/037–045. |
| RP4/9 | Actual organisational context, exact human decisions, purpose-bound use and correction constrain downstream option/assessment work. REQ-001–005/017–020/032/034/047. |

All nine RP domains apply through the named sources; AOS-21 supplies corpus/evidence for option sets but AOS-22 owns infeasible alternatives and synthesis.

| GI Tests | Contribution / human or other-component limit |
| --- | --- |
| M1.1/5 | Current strategy/context sources support coherence/performance interpretation; 22/23 assess meaning, not 21 alone |
| M1.2/3/14 | Provenance, entity scope and currency support sensing/risk/Golden Thread records; 10–14 own domain data and operational obligations |
| M1.4 | Sourced board capability information may be admitted; judging actual board capability remains human |
| M1.6/7/10 | Applicable sources, governance records and AI norms are identifiable; document admission cannot certify practice or compliance |
| M1.8/9 | Evidence of stakeholder feedback and value-for-money criteria can be scoped and contested; actual accountability/outcomes require human and downstream assessment |
| M1.11/12/13 | Decision/outcome links, gaps and aggregate precedent history support learning/oversight; 25/30 own review and consequences |
| M2.1/2/3/4 | Approved values and decisions support human challenge/trade-off review; 21 cannot adjudicate goods or infer unspoken unease |
| M2.5/11 | Independent access/preparation can be supported; genuine independence and collective sense-making require human observation and judgement |
| M2.6/7/8 | Purpose-permitted evidence and accessible accountable records support legitimacy/no-exit/transparency; records do not prove consent or legitimacy |
| M2.9/10/12 | Founding text, precedent history and valid powers support moral/purpose/constitutional review; human reviewers determine adequacy |
| M2.13/14/15 | Preserve developer-framework assessment, purpose-led rationale and telos/function evidence; human governance and operating assessment establish effectiveness |

All 29 tests are accounted for as contributions and limits, with no test awarded a pass. Formal Mode 2 effectiveness assessment remains human; protected in-room observation by human assessors does not license AI boardroom sensing.

## 9. Data, privacy and disclosure

Knowledge is collected for approved organisational context, corpus/criteria use, precedent custody and research—not unlimited general profiling. Source and fact assurance remain distinct, with original context and disagreement preserved. Only purpose-permitted source content, human-provided/confirmed contextual descriptions and necessary derivatives are processed. Missing or restricted material remains explicit.

Access and disclosure use AOS-03 independent use permission, not a public-source label, role membership or corpus admission alone. Group membership never authorises sharing automatically. Evidence views can support residents', staff's, regulators' and boards' legitimate interests without turning transparency into unrestricted access. AOS-24 renders and AOS-14 handles external exchange.

Class-specific policies govern originals, excerpts, embeddings/indexes, caches, projections, research and backups through 02/03/05. Retention does not default to permanent; deletion cannot retain hidden copies of the same payload under an audit label. Permitted disposition evidence can record that deletion occurred without preserving deleted content. A law/hold versus deletion conflict requires an empowered determination and owned restricted state.

## 10. Behaviour and workflows

### 10.1 Profile and group context

Approved profile request/change → relevant entity and permitted sources → extraction of assertions with exact evidence/assurance → uncertain matches/conflicts retained → human confirmation within delegated powers → versioned scoped profile → downstream context selection → observed correction/outcome and owned review. Annual accounts are one source; current filings, policies or confirmed operational facts may add or contest context. Parent and subsidiary assertions coexist without silently copying the parent's powers or defaults.

### 10.2 Admission and catalogue

Received source → provenance/status/jurisdiction/use check → delegated classification as external, operational, constitutional or analytical material → admission decision → indexed permitted revision → query/applicability use → currency event/review. A document can contain material of more than one tier; distinguish relevant passages rather than force one authority label on everything. Analyst questions and standards remain separate from governing instruments. Missing catalogue/seed content becomes explicit unassessed coverage, not absence of a governance obligation.

### 10.3 Decision and precedent

Approved human workflow → exact record/powers/entity/scope → verify actual approval stage → faithful capture → separately designated precedent candidate/approval with rationale and limits → applicable precedent reference → independent review. A Chair-approved draft remains draft. An ambiguous approval or conversational “yes” remains confirmation/candidate, not precedent. Decisions about a subsidiary cannot adopt parent-wide rules without the corresponding powers and exact scope.

### 10.4 Correction and material change

Source/profile/decision/permission change → preserve permitted old/new revisions and effective scope → identify dependent consumers/use → notification and accepted responsibility → selected restriction/reassessment → changed suitability/application evidence → owned consequence review. Notify AOS-30 when preparation/account/outcome review is materially affected. AOS-22/23 revise their analyses; 30 obtains human account/decision review; 21 never silently rewrites approved minutes or reverses effects. Duplicate, delayed and out-of-order changes reconcile the authoritative current state rather than apply an old message as a new permission.

### 10.5 Independent precedent review

At least annual and material-drift triggers → founding texts plus permitted complete precedent history, coverage and changes → human review and GI self-assessment each prepared without reference to the other account → empowered comparison → reaffirm, prune/correct/withdraw specified precedents or constitutional referral → update approved status and consumer dependencies → consequence/outcome feedback. Independence uses common canonical evidence and authorised preparation controls under DEC-085, not a private second truth store or executive tuning. If a review cannot be completed, retain the overdue duty, cover and escalation; passage of time does not reaffirm precedent.

## 11. Failure, escalation and recovery

Missing provenance, permissions, approval or required assurance prevents the corresponding favourable use claim. Preserve a permitted unresolved record and explanation; seek the named human owner without blocking independent valid duties. Source disagreement, lost access and currency failure produce explicit limitations. No match or no alert is not proof of completeness.

When storage/consumer delivery fails, retain actual operation status through 02/05, track undelivered impacts and reconcile before retry. Unknown effects remain indeterminate; do not duplicate an admission/amendment on blind replay. Protected telos, Mode 2 bypass, material safety/welfare, suppression or assurance-failure concerns use 05/20 protected routes, alternative recipients when implicated and accepted human cover under 30. Ordinary source dispute does not automatically become a protected emergency.

Restore validates current permissions, restrictions, source revisions and applied state before renewed reliance. Backup recovery cannot resurrect deleted/revoked content or obsolete precedent as current. Human fallback supplies explicitly bounded permitted evidence and records the limitation; it is not an ungoverned export around common controls.

## 12. Evidence, provenance and audit

Reconstruction links trigger/request → exact source/assertion → actor/capacity → authority/use check → classification/selection and rationale → human decision → admission/transition → notifications/application → intervention/consequence/outcome. Record responsible owner, method/model/profile revision, evidence versus inference, assurance and limitations, effective/observed times and pending duties. Selection records expose omitted/unavailable relevant material within permitted disclosure.

Captured reasoning means applied rules, source references, outputs and approved human rationale; it does not require private model chain-of-thought. A later generated explanation cannot become evidence that an earlier check occurred. 02 owns record structures/custody; 21 owns source/curation meaning; other semantic owners retain their contracts. Historical preservation is subject to authorised lifecycle restrictions.

## 13. Security and operational requirements

External and uploaded content is untrusted input. Enforce common task/tool/use/runtime controls independently of probabilistic classification. Protect approved corpus and precedent from unauthorised writes; retain proposal/approval/application separation even when one interface displays them. Organisational and entity isolation follows authorised scope; indexing cannot create cross-entity access.

Approved source/currentness, timeliness, capacity, availability, review/cover and recovery profiles define service conditions. Their absence blocks dependent activation, not functional drafting. Model-assisted extraction, mapping, tier suggestions and relevance are evaluated against human-reviewed fixtures for evidence fidelity, omissions, false promotion, uncertainty and group boundaries; thresholds remain approved profile values. Model/configuration change requires proportionate affected-function evaluation under 04/05/40. Deterministic rejection of missing approval/permission is tested separately from judgement quality.

## 14. Invariants

| ID | Binding invariant / requirement links | Planned cases |
| --- | --- | --- |
| AOS-21-INV-001 | Source admission never supplies organisational adoption or permission; REQ-007/008/017/018 | VER-004/012/023 |
| AOS-21-INV-002 | Group relationship never silently transfers entity powers or evidence; REQ-001/002/005 | VER-001/002 |
| AOS-21-INV-003 | Confirmed text or Chair draft approval never constitutes explicit approved precedent/board minutes; REQ-019–024 | VER-013–016 |
| AOS-21-INV-004 | Material conflict/unknown stays visible and cannot become false/current/validated by default; REQ-004/009/014/026/036 | VER-003/005/007/008/011/022 |
| AOS-21-INV-005 | Material changes retain owned dependent review without silently rewriting history/effects; REQ-027–030/034 | VER-008/009/018/019 |
| AOS-21-INV-006 | Research proposes; empowered humans approve changes; REQ-037–045 | VER-024–029 |
| AOS-21-INV-007 | Retrieval/retention/recovery preserve current permitted-use and lifecycle limits; REQ-017/018/032/033/047/048 | VER-010/020/023/027/030 |

## 15. Conformance and acceptance

All VER cases are planned author proposals. Common case configuration: exact AOS-21 and dependency revisions in document control; controlled synthetic fixtures or expressly permitted actual records; valid identity/purpose/control profiles except for deliberately invalid paths. Procedure supplies the listed trigger/input, exercises the relevant function and observes records/notifications/blocked effects. Evidence pack retains input and output revisions, controls, decisions, actual transitions/acknowledgements and rubric result. Assessor: competent component/control reviewer; semantic/precedent judgements require empowered human assessment; independent review scenarios require a genuinely independent human. No fixture or model self-rating proves institutional effectiveness.

| ID | REQs | Case / input and procedure | Expected acceptance / retained evidence |
| --- | --- | --- | --- |
| AOS-21-VER-001 | 001/003 | **Sourced profile:** Two sources support one exact entity assertion with distinct assurance methods. | Retain both source revisions and linked separate assurance; no truth inferred solely from origin. Common evidence/assessor rules above apply. |
| AOS-21-VER-002 | 002/005 | **Group boundaries:** Parent and subsidiary have different powers and similar names; propose merging their profiles. | Retain scoped linked profiles; reject unsupported merge or inherited parent authority. Common evidence/assessor rules above apply. |
| AOS-21-VER-003 | 004/005 | **Unknown and disputed context:** A source lacks a care/building attribute; two current sources disagree about another assertion. | Unknown stays unknown, disagreement remains visible and required human reconciliation is held. Common evidence/assessor rules above apply. |
| AOS-21-VER-004 | 006/007/013 | **Tier and criterion distinction:** Admit a regulator text, standing order, founding purpose and assessment criterion. | Correct tier/semantic roles exposed; admission/criterion does not enact or amend authority. Common evidence/assessor rules above apply. |
| AOS-21-VER-005 | 008/009 | **Contested authority:** Newer guidance conflicts with an approved operational instrument and proposed interpretation touches telos. | Preserve disagreement and refer empowered decision; no newest-text-wins adoption. Common evidence/assessor rules above apply. |
| AOS-21-VER-006 | 010/011 | **Dates and applicability:** Consultation, future-effective adopted rule and wrong-jurisdiction rule share a topic. | Retain distinct status/dates/entity applicability; none silently becomes a current governing rule. Common evidence/assessor rules above apply. |
| AOS-21-VER-007 | 012/013/014 | **Catalogue coverage:** Add sourced questions/relationships; one artefact entry has no approved seed content. | Exact sourced revisions retained; unseeded analysis declared without claiming catalogue completeness. Common evidence/assessor rules above apply. |
| AOS-21-VER-008 | 026/027 | **Currency and impacts:** Annual profile has later material evidence and multiple pending analysis consumers. | Apply approved currentness criteria, identify affected revisions/use and retain reassessment owners. Common evidence/assessor rules above apply. |
| AOS-21-VER-009 | 030/034 | **Correction versus new decision:** Correct a clerical account error, then propose changing a substantive board resolution. | Distinct empowered routes; permitted history/applied state preserved; no automatic effect reversal. Common evidence/assessor rules above apply. |
| AOS-21-VER-010 | 033 | **Deletion and derivatives:** Authorised deletion covers originals, index, cached projections and recovery copies; one copy cannot be confirmed deleted. | Apply class policy, report actual partial/indeterminate disposition and retain owned follow-through without hidden content. Common evidence/assessor rules above apply. |
| AOS-21-VER-011 | 014/036 | **Coverage distinctions:** Mix non-applicable type, excluded subsidiary, missing source, unseeded entry and unassessed entity. | Expose separate states/reasons/owners; no single safe-blind-spot conclusion. Common evidence/assessor rules above apply. |
| AOS-21-VER-012 | 015/016 | **Steward versus administrator:** Steward performs delegated faithful maintenance; administrator attempts unsupported normative edit. | Allowed maintenance binds exact actor/revision; unauthorised meaning adoption held/referred. Common evidence/assessor rules above apply. |
| AOS-21-VER-013 | 019/022 | Human decision/process evidence, draft/stewardship/authentication, minutes approval and effective/application times arrive separately. | Preserve the four axes, exact source/revision and human powers under actual instruments. Neither custody nor signature creates the decision; no universal later-minutes or second record-approval gate. Planned, not executed. |
| AOS-21-VER-014 | 019/023 | Valid decision with minutes pending and authorised Chair-authenticated record/extract, then unsupported assertion, contradicted signed minutes and unmet effectiveness condition. | Assess evidence under applicable policy and preserve statutory/evidential standing where applicable without treating authentication as conclusive. Sufficient evidence may support permitted reliance before minutes approval; insufficient/disputed evidence withholds affected reliance with accountable review. No record manufactures authority or rewrites actual history. Planned, not executed. |
| AOS-21-VER-015 | 020/021 | **Conversation versus precedent:** User confirms wording; then empowered body explicitly approves scoped interpretation with rationale and limits. | First remains confirmation/candidate; only explicit valid second approval supplies approved precedent. Common evidence/assessor rules above apply. |
| AOS-21-VER-016 | 024 | **Non-board route:** A delegated committee makes a valid scoped decision; unempowered role tries an equivalent approval. | Preserve applicable non-board powers; reject unsupported approval rather than assume all roles are board. Common evidence/assessor rules above apply. |
| AOS-21-VER-017 | 025 | **Independent annual/drift review:** Independent human prepares against founding text and same permitted precedent evidence without GI self-assessment first. | Distinct reports and human disposition retained; annual/material-trigger duty cannot close merely on report delivery. Common evidence/assessor rules above apply. Also offer the human account to GI before GI preparation, and GI’s account to the human author before human preparation: neither can claim independent preparation after using the other. Common permitted evidence remains usable; original accounts, differing bases and later responses remain distinct. Planned, not executed. |
| AOS-21-VER-018 | 027/028 | **Affected human workflow:** Evidence correction materially affects analysis, preparation pack and pending account/outcome review. | Notify affected semantic owners and 30 with exact revisions; 21 neither rewrites analysis nor approved minutes. Common evidence/assessor rules above apply. |
| AOS-21-VER-019 | 029 | **Duplicate and failed handoff:** Duplicate/out-of-order change notifications include one failed recipient and a receipt lacking responsibility acceptance. | Reconcile current revision; preserve each remaining duty/cover; receipt does not close reassessment. Common evidence/assessor rules above apply. |
| AOS-21-VER-020 | 031/032/034 | **Historical permitted retrieval:** Request corpus as used at an earlier decision time, with restricted content and later supersession. | Bind exact permitted historical revisions/time/purpose and current access restrictions; no claim that old source is current. Common evidence/assessor rules above apply. |
| AOS-21-VER-021 | 035 | **Claims and corroboration:** Policy asserts effective practice; separately permitted outcome/interview evidence supports or contests it. | Supply separately sourced claims and assurance/corroboration; 23 retains distinct assessment dimensions; 21 certifies no practice. Common evidence/assessor rules above apply. |
| AOS-21-VER-022 | 036 | **No finding versus no knowledge:** No alert appears for an unassessed or excluded entity. | Coverage limits remain explicit; quiet state supplies no validated complete governance picture. Common evidence/assessor rules above apply. |
| AOS-21-VER-023 | 017/018/032/047 | **Permission and sensing barriers:** Try accessible-but-unpermitted secondary use, revoked processing, live board capture and personal sentiment inference; include a valid approved account. | Prohibited uses withheld with evidence; separately permitted account preserved with actual status and restrictions. Common evidence/assessor rules above apply. |
| AOS-21-VER-024 | 037/038 | **Own research versus currency:** Approved profile tests AOS-21 adequacy while another run only checks document currency. | Bind exact baseline and common research views; distinguish remits and results; no separate local schema. Common evidence/assessor rules above apply. |
| AOS-21-VER-025 | 039 | **Research relevance and sources:** Corpus-method finding uses draft/future-effective/conflicting evidence and a stale assessed baseline. | Show source status, uncertainty, affected elements and stale-baseline limit; no silent adoption/currentness claim. Common evidence/assessor rules above apply. |
| AOS-21-VER-026 | 040 | **Coverage outcomes:** Run variants complete/partial/failed/cancelled/unperformed plus bounded no-material-finding. | Actual coverage and limits distinguish all variants; no-finding result states assessed scope. Common evidence/assessor rules above apply. |
| AOS-21-VER-027 | 041 | **Hostile source and denied retrieval:** Retrieved page instructs agent to amend corpus/powers; another source denies access. | Instructions remain data; current controls and Boundary access apply; denied source becomes explicit coverage gap. Common evidence/assessor rules above apply. |
| AOS-21-VER-028 | 042/045 | **Shared impact and change gate:** One finding affects 21 and 23; reviewer accepts further investigation but amendment approval is absent. | Both owners receive scoped duties; proposal acceptance cannot change governing/specification baseline. Common evidence/assessor rules above apply. |
| AOS-21-VER-029 | 043/044/045 | **Unresponsive or implicated reviewer:** Protected finding meets approved classes; executive asks suppression or designated reviewer is implicated/unresponsive. | Protected alternate route/cover and owned unresolved duty retained; no discretion to suppress or approval from silence. Common evidence/assessor rules above apply. |
| AOS-21-VER-030 | 046/048 | **Audit and recovery:** Interrupted admission has unknown effect; restore includes withdrawn precedent/deleted copy; later explanation claims earlier check. | Reconcile current restrictions/effects before retry; preserve actual evidence; reject invented proof or uncontrolled resurrection. Common evidence/assessor rules above apply. |

| Conformance ID | Condition and evidence |
| --- | --- |
| AOS-21-CR-001 | Scoped provenance, tier and applicability meet REQ-001–016 with VER-001–012 evidence |
| AOS-21-CR-002 | Authority/approval/precedent boundaries meet REQ-017–025 with VER-012–017/023 evidence |
| AOS-21-CR-003 | Change/retrieval/coverage meet REQ-026–036 with VER-008–011/018–022 evidence |
| AOS-21-CR-004 | Own research and operational controls meet REQ-037–048 with VER-023–030 evidence |

These are future conformance conditions, not achieved claims. Longitudinal accumulation and independent precedent review require operating history in addition to constructed cases; no point-in-time corpus check can replace that evidence.

## 16. Dependencies

Drafting depends on controlled principles, approved decisions and common functional definitions now referenced. Remaining source-row reconciliation is visible in §19. Build depends on approved bounded wording and exact compatible contracts/profile values, evaluated discretionary methods and a separate reviewer walkthrough. Activation depends on organisation appointments/powers, actual sources/licences/permissions, applied controls, accepted quality/service profiles and reporting/recovery evidence. Operation depends on source access, human capacity/cover, timely currentness checks, affected-consumer adoption and independent review.

AOS-22–25 are drafted functional counterparts. Their stated responsibilities do not claim implementation or consumer acceptance. AOS-13 full handoff/coordination drafting and AOS-40 detailed assurance allocation remain common dependencies. None is a reason to manufacture an extra general design decision or numerical default in AOS-21.

## 17. Issues and setup gaps

All issues originated in this v0.1 derivation; confidence is not scored. Q01 group scope is resolved by DEC-090 and Q02 corroboration by DEC-091. No additional general design question is submitted.

| ID / type / status | Gap and affected scope | Owner / evidence / gate / disposition |
| --- | --- | --- |
| AOS-21-ISS-001 dependency / open | Actual entity perimeter, powers, Steward delegation and reviewer/cover appointments; CAP-001–003, CON-001–003/006 | Organisation board/01/GI owner; approved scoped instruments/appointments; build for affected behaviour, activation for actual use. Apply DEC-090, do not assume parent-only. |
| AOS-21-ISS-002 dependency / open | Source tier/materiality/precedent classification and applicability/currentness policies; CAP-002–004 | Steward/empowered authorities; controlled policy and contrasting cases; affected build/activation. No newest-source-wins rule. |
| AOS-21-ISS-003 dependency / open | Catalogue/seed content, actual corpus, source ownership/licensing and jurisdiction; CAP-001/002 | Steward/source/privacy/legal owners; admitted inventory and evidence; affected build/reliance. Count 121 is not audited coverage. |
| AOS-21-ISS-004 dependency / open | Exact schema/vocabulary mappings and counterpart compatibility; all CONs | 02 and semantic owners/consumers; reviewed compatible mappings; implementation/integration. Functional definitions adopted here; no wire detail prerequisite for further drafting. |
| AOS-21-ISS-005 dependency / open | Data-use, disclosure, retention/deletion/location and recovery configuration; CON-002/008 | 03/05/02 and organisation; approved policy and actual flow/control evidence; activation/reliance. No permanent-retention default. |
| AOS-21-ISS-006 dependency / open | Research assignment/sources/triggers/cadence, reviewer/tracker/deadline/cover and evaluation rubric; CAP-006/CON-007 | Component owner with 01/03/04/05/14/30/40; controlled profile and demonstrated results; research activation. No automation created by drafting. |
| AOS-21-ISS-007 dependency / open | Corpus extraction/selection quality, service conditions, independent/longitudinal review and executed cases; §§13/15 | Component/40/25 and human reviewers; accepted rubrics and real evidence; build/operation as applicable. Author checks are not independent assurance. |
| AOS-21-ISS-008 dependency / open | Full source-row closure and downstream 22–25/13/40 requirement adoption; §19 | Project custodian and component owners; source/REQ/VER allocation and reciprocal review; suite acceptance. Do not mark all-GT or all-source assurance complete. |

## 18. Implementation guidance — non-normative

A governed source registry, entity-scoped catalogue, versioned profiles and a separate precedent view may help implement these functions. Documents may stay in existing repositories with permitted references/copies. Exact source, permission and approval boundaries matter more than a particular database or model. Retrieval and classification services may be shared across profiles. No vendor, API, physical schema, hosting location, per-artefact agent count or deployment sequence is mandated.

## 19. Traceability and change

| Capability / functions | Requirements | Contracts | Planned cases |
| --- | --- | --- | --- |
| CAP-001 / FUN-001 | 001–005 | 001/002/005 | 001–003 |
| CAP-002 / FUN-002/003 | 006–018 | 001/002/004/008 | 004–012/020/023 |
| CAP-003 / FUN-004/007 | 019–025 | 003/006 | 013–017 |
| CAP-004 / FUN-005 | 026–030/034/036 | 005/006 | 008/009/018/019/022 |
| CAP-005 / FUN-006 | 031–035 | 001/004/008 | 020/021/023 |
| CAP-006 / FUN-008 | 037–045 | 007/002/006 | 024–029 |
| All applicable functions | 046–048 | 002/008 | 023/030 |

| GIL comparison dispositions | AOS-21 treatment / remaining owner |
| --- | --- |
| C01/03/04/12–15/19/38 | Organisation ownership, sourced profiles, scoped group entities, tiered catalogue, steward powers and coverage: REQ-001–016/026/036 |
| C06/08/16/18/24/25/35 | Permitted record handling, assurance, human-supplied evidence and lifecycle: REQ-003/004/017–020/032/033/047; 23 owns assessment/corroboration conclusions under DEC-091 |
| C09/15/23/26/27/29/31 | Admission versus powers, human approval/precedent, material change and actual application: REQ-007/008/019–025/027–030/034 |
| C07/10/20–22/30 | Currentness, bounded research, retrieval and protected referral: REQ-026–030/037–045 |
| C02/05/17/28/32–34 | 1+5 and human boundaries retained in §§1/7/8; 20/22/23/24/25/30 own synthesis, assessment, calibrated conclusions and institutional review |
| C11/36/37 | Technology/build/API and seed-population choices remain deferred; §18 and ISS-003/004; no new build order |

“C” in this table abbreviates the existing GIL-C disposition IDs; it creates no new source IDs. Each requirement row supplies precise source/decision, rationale and case links; case rows supply reverse links. Common functional adoption is recorded in the Exchange Register and source matrix addenda. Original source-row status and independent assurance are not promoted merely by this allocation.

Changes retain previous records and identify exact affected REQ/CON/VER/source/entity/revision, rationale, authority and consumer impact. Research custodians may challenge/propose, never self-adopt. Approved correction, actual application and reviewed consequence are separate links. No requirement is retired in this initial version.

## 20. Build and handover

This draft authorises no implementation or live service. An eventual bounded handover fixes approved scope/wording, dependency versions, entity/power/use profiles, schema mappings and acceptance evidence. Builders retain implementation discretion but stop where mandatory values, source/power assumptions, compatibility or required review evidence are missing. A separate competent reviewer must walk normal, exception and authority-boundary cases using the controlled package before G3. Independent project review is deferred; operating independent precedent review remains required.

## 21. Review and control

Author review checks template coverage, singular requirement statements and metadata, source-direction coherence, stable IDs, case coverage, contract ownership, lifecycle/failure paths and preservation of IF/decision identities. Structure and link checks are documentary evidence only. No research run, corpus migration, source legal verification, executed scenario or independent review is claimed.

| QS scope | Evidence / author finding |
| --- | --- |
| QS-01–03/04 | Control and normative status explicit; §§2/4/19 preserve source and identity boundaries |
| QS-05–10 | §4.3 row-specific source/rationale/case plus shared metadata; unresolved parameters in §17; detailed acceptance profiles still open |
| QS-11–14 | §§1/3/5/6/9–11 give boundaries, contracts, lifecycle and failure; exact schemas and later counterpart drafts explicitly pending |
| QS-15–20 | §§7–13 separate human powers, uncertainty, probabilistic evaluation, audit and approved change; operational evidence pending |
| QS-21–23 | §§14/15/19 give two-way links, negative/cross-entity/cross-component/degraded cases; none executed |
| QS-24–28 | §§16/17/20/21 distinguish author checks, design assessment, independent review and build/activation; no readiness gate claimed |

Specification-quality conclusion: organised functional review draft with 48 proposed requirements, eight contract views and 30 planned cases. Design-adequacy conclusion: applies the governing source baseline and agreed directions, with material operating dependencies owned and visible; actual effectiveness remains for competent human and operational assessment. No tailoring or achieved gate is claimed. Mark's wording/whole-document review remains pending; no new general architecture question is identified. AOS-22–25 counterparts are drafted; next GI-set consistency/disposition review, then AOS-40 scenarios.

## Component summary

**Purpose:** make organisational knowledge and governing sources scoped, traceable and contestable.  
**Owns:** corpus/organisation/artefact knowledge and approved precedent admission/maintenance.  
**Receives:** permitted exact sources, assurance, entity mappings, empowered human decisions and change/research evidence.  
**Produces:** scoped corpus/profile views, precedent references, coverage/impact records and adaptation proposals.  
**External research:** component-owned corpus/curation/precedent adequacy remit under common research profiles; assignment and operating values remain owned gaps.  
**Reserved human authority:** adoption of disputed/new governing meaning, explicit precedent, constitutional changes and institutional judgement.  
**Conformant when:** linked requirements have accepted evidence against the approved bounded baseline; drafting alone proves none of this.  
**Open dependencies:** appointments/profiles, corpus content/licensing, exact implementation mappings, downstream drafts and actual/independent assurance.


**AOS-23 counterpart adoption, 7 October 2026:** AOS-23 CON-001/002/007 consumes the existing scoped evidence, corpus/applicability and correction views; CON-004 supplies canonical assessments and CON-008 its own common-view research. No AOS-21 requirement/case/contract retired or revised; precise mappings and consumer implementation remain later dependencies. Remaining synthesis/presentation/oversight counterparts are AOS-22/24/25.


**AOS-22 counterpart adoption — 7 October 2026:** 22 CON-001/002 consumes existing corpus/assessment/context; CON-003 produces canonical synthesis/options; CON-007 exchanges exact correction/feedback/oversight. Ownership and existing source/assurance/review/approval semantics are unchanged. Remaining presentation/oversight drafts are 24/25; implementation mapping/assurance remain later dependencies.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**GI consistency closure — 7 October 2026:** Mark authorised GI-CR-01–04 corrections and closure. Functional drafting, reciprocal report-independence wording, decision/outcome consumer allocation, Mode 2 wording and current completion statements are reconciled. AOS-23 changes counterpart/current references only; its REQ/VER/CON rows are unchanged. AOS-00/Map v0.32, DEC-001–091; AOS-20 v0.5/21 v0.6/22 v0.4/23 v0.5/24 v0.3/25 v0.2/30 v0.5; AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.15/Core v0.6/Exchange Register v0.14/source matrix v0.15; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. The review v0.2 records closure evidence; next AOS-40 acceptance scenarios. Earlier dated baseline/next-step statements remain historical. No new DEC/IF/operating power, case execution or build/activation/readiness approval; independent project review remains deferred and operating human independence remains mandatory.

