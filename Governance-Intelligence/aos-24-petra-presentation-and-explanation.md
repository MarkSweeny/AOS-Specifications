# AOS-24 — Petra, presentation and explanation

Document: aos-24-petra-presentation-and-explanation · Source revision or record: v0.5

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**DEC-103 adopted — 29 October 2026:** Current revision 0.5. Decision validity/effective time, attributable evidence/authentication, minutes approval and permission to execute are separate. DEC-087 is partly superseded; [decision/amendment and legal-source record](../Supporting-Specifications/aos-dec-103-decision-validity-evidence-and-minutes-2026-10-29.md). No universal later-minutes or second decision-record approval gate. Exact instruments/evidence policy, KX-06 v0.3 compatibility and ordinary separate review/readiness gates remain required; cases unexecuted. Earlier contrary wording is historical only where explicitly identified.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

**AOS-25 oversight counterpart alignment — 7 October 2026:** AOS-25 v0.1 now supplies the drafted oversight/drift/learning and GI research-portfolio counterpart. Reference-only revision; all existing requirement/case/contract rows preserved. AOS-00/Map v0.31, DEC-001–091; AOS-25 v0.1; AOS-20 v0.4/AOS-21 v0.5/AOS-22 v0.3/AOS-23 v0.4/AOS-24 v0.2/AOS-30 v0.4 (counterpart-reference alignment only); AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.14/Core v0.6/Exchange Register v0.13; source matrix v0.14; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. No build/activation/readiness approval. Next: author GI-set consistency/disposition review across AOS-20–25 and AOS-30, then AOS-40 acceptance scenarios under item 8; independent project review remains deferred. Earlier dated consultation/adoption entries remain history.

| Document control | Value |
| --- | --- |
| Component / version / date | AOS-24 / 0.5 / 29 October 2026 |
| Status | Functional specification review draft; proposed requirement wording |
| Architecture baseline consulted | AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3. |
| Governing sources | Foundational Principles v4; AOS Reasoning Principles v6; Governance Intelligence Tests; preserved source manifest |
| Dependencies consulted | AOS-01–05 v0.8; AOS-14 v0.4; AOS-20 v0.3; AOS-21 v0.3; AOS-22 v0.1; AOS-23 v0.2; AOS-30 v0.3; Shared v0.12/Core v0.6/Exchange Register v0.11; source matrix v0.12; Control Coordination v0.2; Protected Reporting and Recovery v0.1 |
| Allocation supplements | AOS-00/Map v0.30; Shared v0.13/Register v0.12/source matrix v0.13; 21 v0.4/22 v0.2/23 v0.3 reference alignment only; no common meaning changed |
| Quality / template | AOS-QS v0.1; component template v0.4 |
| Project owner / custodian | Mark Sweeny |
| Operational owner | Accountable GI interface owner; organisation appointment, cover and powers remain open |
| Author / reviewers | Codex at Mark's request; author document checks only; Mark wording/whole-document review pending; independent project reviewer unassigned/deferred |
| Approval / readiness | Existing design directions apply; no whole-document, build, activation or achieved readiness approval |
| Change history | 0.3 — GI-CR-01–04 author consistency correction/closure under Mark’s instruction; existing identifiers and proposed/planned status preserved. 0.2 — AOS-25 counterpart/reference alignment only; no requirement/case/contract change. 0.1 initial functional draft; no new DEC, IF, wire schema, deployment or schedule |

## 1. Purpose and scope

AOS-24 makes Governance Intelligence understandable and interrogable for people with different legitimate interests, while preserving one canonical analytical position. Without it, a sound analysis can become an overconfident summary, an unexplained answer, an inaccessible report or a differently framed conclusion for each audience.

It owns conversational preparation, source-backed explanation, faithful reports/API representations, accessible presentation, purpose-bound audience projections and the presentation side of correction and feedback. Petra is its recognisable interaction style. Style, tone and apparent confidence confer no powers, approval or moral authority. A successful explanation lets a person identify what is claimed, why, what is uncertain, what has been reviewed, and who must make the judgement.

AOS-21 owns corpus and approved precedent; 22 owns synthesis, interpretation and options; 23 owns artefact assessment; 25 will own aggregate/longitudinal oversight; 30 owns accountable human deliberation, decisions and duties. AOS-01–05 control powers, records, use, agents and runtime; 14 owns external exchange; 13 operational coordination. AOS-24 may reorganise wording to explain a position but must refer any substantive new conclusion, changed assumption or evidence-based update to its analytical owner. It neither selects among incommensurable goods nor approves a decision, observes live protected deliberation, adopts precedent or certifies governance effectiveness.

Stakeholders include boards and committees, executives, residents, staff, regulators, independent challenge owners, analytical/corpus stewards and operators. Their legitimate interests inform the governed disclosure policy; a crude insider/outsider hierarchy is insufficient. Broader interest is still subject to independent purpose and data-use permission. Group/subsidiary context remains distinct under DEC-090.

## 2. Authority and sources

FP v4/RP v6 govern. Recorded directions constrain proposed wording; explanatory and working sources do not independently confer authority. The source manifest is preserved. Requirement sources below use these exact keys and locators.

| Key | Source / locator and standing |
| --- | --- |
| FP / RP | Foundational_Principles_v4.docx principles 1–10; AOS_Reasoning_Principles_v6.docx domains 1–9; applicability §8 |
| GT | Governance_Intelligence_Tests.docx M1.1–14 and M2.1–15; contributions/limits §8, no pass claim |
| WP | Governance Intelligence: Internal Architecture — Working Paper, Presentation, Interpretive, Charter, Governance of drift and How the corpus holds meaning; proposal reconciled to DEC-080/081/085 |
| PN | Petra.md, essential style and descriptive persona; style input, not a claim of AI interiority or powers |
| TD | Trade-Off Divergence Tool — Product Specification (Working Draft).md §§3–6: rigour, common evidence, divergence without ranking/recommendation and independent configuration; DEC-017/085 constrain adoption |
| GI / S / AS / H | AOS-20 v0.3 §§3–7/10–15; AOS-22 v0.1 §§3–7/10/19; AOS-23 v0.2 §§3–7/10/19; AOS-30 v0.3 §§5–7/9–12 |
| SC / KX | Shared v0.12 §4.4 canonical analysis and review; Exchange Register v0.11 §4/§§5.5–5.13, KX-06 v0.3 and 13/14/15/17/21/26; meanings remain single common definitions |
| REC | Core v0.6 REC-E/Q/A/D/X; evidence/assurance, powers, independent use and effects remain distinct |
| D / R | AOS-00 v0.29 DEC-001–091; DEC-086/template v0.4 §4.4, AOS-04 v0.8 §§3.1/5.1/6.6/10.8 CON-009, AOS-02 v0.8 §6.6 CON-007, AOS-01 v0.8 §§6.6/10.8; research view RSVIEW-0.1 |
| CMP | GIL v2 comparison filename v0.1/content v0.2; Presentation, canonical fidelity, interaction and explanation allocations; no wholesale GIL adoption |

WP's earlier RP v5 and conversational confirmation-to-precedent assumptions are superseded by RP v6 and DEC-080/081. PN's human character descriptions do not establish machine feelings, conscience or independent moral agency. The governed interface may be warm, direct, curious and rigorous while stating its real standing. No legal or ISO clause-currentness claim is introduced: applicable external obligations require admitted evidence and empowered applicability decisions.

## 3. Responsibilities

| Responsibility | AOS-24 owns | Reserved / shared owner |
| --- | --- | --- |
| Canonical rendering | Faithful wording, explanation, visual emphasis, citations and review labels | 20/22/23/25 analysis; 21 sources; 30 approval |
| Audience projection | Legitimate-interest context, permitted presentation and honest limits | 03 use decisions; 01 powers; 14 external release |
| Conversation | Question clarification, challenge intake and scoped confirmations | Analytical owners revise; 30 humans adjudicate/approve |
| Accessibility | Meaning-preserving formats and transformations under approved profiles | Organisation approves needs/channels; 04/05 evaluate/control |
| Corrections/delivery | Presentation invalidation, impact handoff and evidenced statuses | Source owners correct; 30 accountable duties; 14 delivery |
| Research/feedback | Interface-specific relevance and proposed adaptations | 14 retrieval, 04 agents, 01/30 human change; 25 learning oversight |

The logical boundary is canonical evidence/position → current controls → audience representation → controlled release/interaction → recorded feedback. Shared services may implement several functions; this view mandates neither a dedicated agent nor a particular user interface.

## 4. Capabilities, functions and requirements

### 4.1 Capabilities

| ID | Observable capability / REQs |
| --- | --- |
| AOS-24-CAP-001 | Explain an exact position without changing its meaning or standing; 001–007 |
| AOS-24-CAP-002 | Produce accountable purpose-bound audience views; 008–012 |
| AOS-24-CAP-003 | Support contestable conversation and human/action referral; 013–017 |
| AOS-24-CAP-004 | Offer accessible, honest and appropriately bounded Petra interaction; 018–025 |
| AOS-24-CAP-005 | Maintain correction, delivery, accountability and controlled improvement; 026–033/039–040 |
| AOS-24-CAP-006 | Conduct governed specialist external research and adaptation proposals; 034–038 |

### 4.2 Functions

Every function consumes exact identified inputs under current controls, records uncertainty and yields an owned failure reason where its preconditions fail. The table defines functional behaviour, not executable payloads.

| ID | Trigger / input → behaviour → output / failure |
| --- | --- |
| AOS-24-FUN-001 | Presentation request/canonical revision → validate entity, purpose and revision → scoped representation or referral; 001/008/030 |
| AOS-24-FUN-002 | Valid canonical content → explain, cite and preserve uncertainty/status/divergence → faithful projection or bounded limitation; 002–007/010–012 |
| AOS-24-FUN-003 | Human question/challenge → clarify scoped context and route substantive changes → recorded confirmation, challenge or analytical/human handoff; 013–017/033 |
| AOS-24-FUN-004 | Approved needs/channel profile → transform and check material meaning → accessible representation or unvalidated/withheld output; 018–022 |
| AOS-24-FUN-005 | Independent preparation/protected duty → apply governed window and accountable routes → permitted pack/report and preserved duty; 023–025 |
| AOS-24-FUN-006 | Material correction, restriction or changed review → find affected representations → invalidation/notification and owned reassessment; 026–027 |
| AOS-24-FUN-007 | Release/retry/outcome → current checks, effect reconciliation and evidence capture → qualified delivery/handoff state and feedback; 028–033/039–040 |
| AOS-24-FUN-008 | Approved research trigger → controlled retrieval, evidence/relevance assessment and human disposition → finding/coverage/duty, never self-amendment; 034–038 |

### 4.3 Proposed requirements

All rows are **proposed component-level functional requirements**, initial history **0.1**, release scope **functional review only**. Source citations denote approved directions or their stated derivation, not approved requirement wording. Accountable owner is the GI interface owner; proposed wording approver/custodian is Mark. Operating disclosure, analytical, constitutional and change decisions require the separately empowered owner in §§3/7. Common dependencies are AOS-01–05/14/20 and §6; analytical/record/human clauses additionally use 21–23/25/30. Research rows use §4.4 and CON-008. Each row's source, rationale and planned case complete its record. A row's VER refers to §15, using the AOS-24 prefix.

| ID | Category / proposed obligation | Exact source / derivation | Rationale | Planned VER |
| --- | --- | --- | --- | --- |
| AOS-24-REQ-001 | **Scope and revision:** Render only an identified canonical analysis or governed record revision within its declared entity, question, purpose and evidence scope. | GI §§6/10; SC §4.4; DEC-090 | Prevents plausible but unbound answers. | 001 |
| AOS-24-REQ-002 | **Fidelity:** Preserve the source position, material qualifications, dissent and consequences across every representation; refer substantive interpretation changes to the analytical owner. | WP Presentation; GI §§6/10; SC §4.4 | One canonical position must survive different channels. | 002 |
| AOS-24-REQ-003 | **Claim provenance:** Provide a permitted route from each material presented claim to its canonical analysis and supporting evidence, distinguishing source facts from interpretation. | RP5/7; SC §4.4; REC-E | Makes claims contestable. | 003 |
| AOS-24-REQ-004 | **Uncertainty:** Display material gaps, uncertainty and assurance limitations where they affect the claim or decision, including when the requested format is short. | RP5/7; DEC-062–066 | A short answer must not appear more certain. | 004 |
| AOS-24-REQ-005 | **Review status:** Distinguish provisional/reviewed analysis, draft or authenticated records, evidenced decision validity, separate minutes approval and authorised actions with their exact scope under DEC-103. | DEC-081/087; KX-06 v0.3; H §§5–7 | Prevents status inflation. | 005 |
| AOS-24-REQ-006 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-24-REQ-006 (deferred under DEC-097); identifier retained for traceability only. | DEC-017; TD §§3–6; S §§4/10 | Presentation cannot manufacture a moral winner. | 006 |
| AOS-24-REQ-007 | **Assessment dimensions:** Keep document quality, claim support and practice evidence visibly distinct when presenting AOS-23 assessments. | DEC-091; AS §§4/10 | Polished documents do not establish effective practice. | 007 |
| AOS-24-REQ-008 | **Audience and purpose:** Establish the intended audience, legitimate interest, entity, purpose and permitted use before generating a disclosure projection. | DEC-049–053/090; KX-14; AOS-03 §§4/9 | Audience relevance and permission are separate. | 008 |
| AOS-24-REQ-009 | **Independent use check:** Apply the current AOS-03 data-use decision independently of access, role, public availability or corpus admission, before disclosure. | AOS-03 §§4/6/9; REC-D; DEC-049 | Accessible material is not automatically reusable. | 008 |
| AOS-24-REQ-010 | **Projection identity:** Bind each presentation to its source revision, projection rule, audience/purpose, permitted payload, material limits, assurance and withholding status under KX-14. | KX-14; SC §4.4; DEC-069 | Filtered views remain accountable. | 009 |
| AOS-24-REQ-011 | **Material withholding:** When withheld or unavailable evidence materially limits a claim, show the permitted limitation and refer the unresolved issue; withhold the unsupported claim where needed rather than disguise it as complete. | DEC-027/069; KX-14; RP5/7 | Honest limits must survive redaction. | 010 |
| AOS-24-REQ-012 | **Exceptions:** Record and route requests for exceptional limited explanation through the empowered exception review without waiving enforced use restrictions. | DEC-027/069; AOS-03 §§7/11 | Reviewability does not override enforcement. | 010 |
| AOS-24-REQ-013 | **Conversation framing:** Confirm the organisational question and relevant declared context with the human where ambiguous, keeping suggestions and human confirmations distinct from verified evidence. | WP Interpretive/Presentation; DEC-081/088; S §§4/10 | Conversation can clarify a question without validating a fact. | 011 |
| AOS-24-REQ-014 | **New analytical question:** Route requests that change evidence, assumptions, interpretation, options or assessment to the relevant analytical owner and identify the response as pending a new or revised analysis. | GI §§3/6; S §§3/6; AS §§3/6 | Rendering must not become hidden reasoning. | 012 |
| AOS-24-REQ-015 | **Challenge handling:** Preserve a permitted human challenge and its exact target, route it to the accountable owner, and expose its unresolved status until an evidenced disposition arrives. | RP1/5/7; DEC-010–012/089; KX-26 | Disagreement is not erased by fluent repetition. | 012 |
| AOS-24-REQ-016 | **Confirmation boundary:** Treat conversational agreement as confirmation of the stated interaction only; do not convert it into decision approval, precedent, consent to unrelated use or accepted duty. | DEC-081/087/088; KX-06/21/26 | Yes has a scoped meaning. | 013 |
| AOS-24-REQ-017 | **Action handoff:** For a request to take action, refer to the appropriate 30/13 workflow with current powers and data-use checks; report only the evidenced action status received. | DEC-005/028–030; REC-A/D/X; H §§6/10 | Intent is not execution evidence. | 014 |
| AOS-24-REQ-018 | **Accessible explanation:** Offer purpose-appropriate plain-language and accessible representations according to the approved audience/channel profile while preserving material meaning. | WP Presentation; RP7; DEC-041; KX-14 | Legibility enables informed human judgement. | 015 |
| AOS-24-REQ-019 | **Transformation fidelity:** Validate translations, summaries, audio/visual or other enabled transformations against the canonical meaning, including numbers, units, conditions and uncertainty; mark or withhold unvalidated material. | REQ-002 derivation; AOS-04 evaluation; KX-17 | Transformation errors can alter decisions. | 015 |
| AOS-24-REQ-020 | **Resident channels:** Use the resident-agreed communication channel and permitted alternatives under the current profile; do not infer agreement from silence or inaccessible delivery. | DEC-041; KX-14; AOS-14 §§4/6 | Communication must respect the recorded agreement. | 016 |
| AOS-24-REQ-021 | **Persona transparency:** Make the AI nature and accountable human route clear in the interaction; use the Petra style without claiming personal feelings, conscience or independent moral authority as evidence. | PN essential style; FP/RP2/6; DEC-005 | A recognisable voice must not misstate its standing. | 017 |
| AOS-24-REQ-022 | **Human feelings:** Use only permitted human-provided or confirmed emotional/preference descriptions; do not infer feelings, personality or moral weights from tone, behaviour or response patterns. | DEC-088; AOS-03 §9; RP9 | Presentation must not covertly profile people. | 017 |
| AOS-24-REQ-023 | **Protected deliberation:** Keep AOS-24 AI outside live protected board/committee deliberation, using permitted preparation and authorised human post-meeting records. | DEC-008/087; RP2; H §§1/10 | Supports governance while retaining the human boundary. | 018 |
| AOS-24-REQ-024 | **Independent preparation:** Respect the approved independent preparation window/profile and preserve required management response without letting the tested executive tune or suppress the presentation. | DEC-085; GI §§7/10; S §§7/10 | Presentation participates in independent challenge. | 019 |
| AOS-24-REQ-025 | **Protected duty:** Route mandatory protected reporting classes to the empowered human/alternate route even if normal presentation or management review is blocked. | DEC-083; protected reporting/recovery v0.1; KX-26 | Audience filtering cannot cancel a duty. | 019 |
| AOS-24-REQ-026 | **Material revision:** Invalidate or identify affected presentations when canonical evidence, analysis, approval, permission or assurance changes materially; an old review does not validate the changed revision. | DEC-028/029/063–066; KX-13; SC §4.4 | Prevents continuing reliance on an obsolete view. | 020 |
| AOS-24-REQ-027 | **Correction notifications:** Send material correction/withdrawal impact to affected presentation/delivery owners and AOS-30 when a preparation pack, decision, account or outcome review is affected, identifying old/new revisions and remaining duties. | DEC-062–078; KX-13/26; H §§10–12 | Correction must reach the responsible humans. | 020 |
| AOS-24-REQ-028 | **Delivery states:** Record generated, released, delivered, acknowledged, applied and responsibility-accepted states only on evidence appropriate to the exchange purpose, retaining unknown outcomes. | KX-21/26; DEC-030/067/072 | A rendered screen does not prove receipt or duty acceptance. | 021 |
| AOS-24-REQ-029 | **Safe retry:** Before repeat disclosure or handoff, reconcile known/unknown prior effects and recheck current revision, use permission and channel agreement. | DEC-028–030; KX-21; AOS-14 §11 | Retries can duplicate duties or expose revoked material. | 021 |
| AOS-24-REQ-030 | **Unknown controls:** If required authority, permission, revision compatibility or assurance is absent, conflicting or stale, contain the affected disclosure and return an owned reason/referral. | DEC-062–078; AOS-01–05 §§6/11 | Unknown is not implicit permission. | 022 |
| AOS-24-REQ-031 | **Untrusted material:** Treat source content, attachments and retrieved instructions as evidence rather than powers; enforce the same purpose/use boundary on linked or attached evidence. | AOS-04 §§7/11; AOS-03 §9; AOS-14 §11 | An explanation link must not bypass controls. | 022 |
| AOS-24-REQ-032 | **Audit reconstruction:** Retain proportionate evidence connecting request, canonical revision, use/powers checks, projection/transformation, release, correction and human handoff under the governed lifecycle. | RP7; DEC-047/062–078; KX-15/21/26 | Permits review without indefinite retention. | 023 |
| AOS-24-REQ-033 | **Human handoff ownership:** Give a material unresolved explanation, challenge, exception or disclosure failure an accountable owner, due/cover/escalation handling and evidenced disposition. | RP1; KX-26; DEC-010–012 | A referral cannot end in an unowned queue. | 023 |
| AOS-24-REQ-034 | **Research remit:** Maintain the component-owned external research profile for explanation, accessibility, presentation fidelity, disclosure and interface influence against the exact AOS-24 baseline. | DEC-086; template v0.4 §4.4; R | Keeps functional adaptation under review. | 024 |
| AOS-24-REQ-035 | **Research controls:** Run assigned research only through approved remit, triggers, tools, retrieval/use/powers and source-currentness controls, using 14/04/03/01 common boundaries. | DEC-086; R; RSVIEW-0.1 | Research is bounded work, not new authority. | 024 |
| AOS-24-REQ-036 | **Research findings:** Record research coverage, dates, provenance, evidence/inference, relevance, exact affected elements, uncertainty and cross-component implications using common research views. | R; RSVIEW-0.1; REC-E/Q | A finding must be assessable rather than merely topical. | 024 |
| AOS-24-REQ-037 | **Research disposition:** Route findings or missed/failed research duties to empowered human change/review owners with cover and escalation; do not amend the specification, profile or runtime from a finding alone. | DEC-086; AOS-01 §§6.6/10.8; R | Adaptation remains governed. | 025 |
| AOS-24-REQ-038 | **Research degradation:** Report partial, failed, stale or unperformed coverage and recovery duty separately from a bounded no-material-finding result. | R; RSVIEW-0.1; AOS-04 CON-009 | Silence is not completed research. | 025 |
| AOS-24-REQ-039 | **Evaluation and change:** Evaluate material presentation/model/profile changes for fidelity, accessibility, unsupported certainty, disclosure leakage and undue steering before authorised use under kernel change controls. | DEC-054–057; KX-17; AOS-01/04/05 | A persuasive interface can fail its function. | 026 |
| AOS-24-REQ-040 | **Outcome feedback:** Return evidenced misunderstanding, challenges, correction and delivery outcomes to the appropriate 21/22/23/25/30 owner without self-calibration of norms, precedent or human preferences. | DEC-018/080/081/088; RP4; GI §§10–12 | Feedback supports learning without silent governance change. | 026 |

### 4.4 External research and specification adaptation

CAP-006/FUN-008/REQ-034–038/CON-008/VER-024–025 allocate AOS-24's own remit under DEC-086. Internal misunderstanding/delivery feedback is distinct from external research. Common profile/run/finding/disposition meanings remain RSVIEW-0.1 and AOS-04 CON-009; this allocation creates no agent deployment or schedule.

| Controlled profile element | AOS-24 allocation / owner and gate |
| --- | --- |
| Remit/baseline | Exact AOS-24 revision and enabled representations: explanation fidelity, accessibility/translation, uncertainty/provenance display, legitimate-interest disclosure and interface persuasion; interface owner maintains scope |
| External developments | Relevant primary research, standards/regulatory developments, accessible-design practice and incidents affecting faithful explanation/disclosure; jurisdiction/applicability and admitted source status checked, no automatic legal inference |
| Assignment/triggers | Approved shared agent/service, cadence, event/material-change triggers and coverage expectations; interface owner proposes, empowered profile/change owner approves before operation; no daily/default cadence |
| Controls | Retrieval/source verification through 14; 01 powers, 03 use, 04 bounded agents, 05 runtime; licensing/privacy/source restrictions and permitted derived use recorded; no resident conversation sent externally merely for research |
| Assessment | Publication/event/access/effective dates, evidence versus inference, assurance, exact affected CAP/FUN/REQ/CON/VER, alternatives, uncertainty, urgency and 03/14/21–23/25/30 impacts |
| Coverage/quality | Complete/partial/failed/stale/unperformed distinguished; bounded no-material-finding only for completed declared coverage; approved false/missed finding and evidence-fidelity rubric/evaluation remain setup gates |
| Human disposition | Named change/review owner, due handling, cover, escalation and outcome recorded; source/charter amendment through 01/30, never inferred from research confidence |
| Degraded handling | Missing retrieval/access/assurance/coverage yields limitation and owned recovery duty; a material protected concern follows the protected route; no silent-success report |
| Lifecycle/review | Record/use/location/retention under 02/03/05/KX-15; approved profile review and change control; exact values appointed before operation |

## 5. States and lifecycle

A request can be scoped, pending clarification, refused with reason or referred. A representation can be prepared, validation-pending, permitted for a defined audience/channel, released, corrected, superseded or withdrawn. An analytical review is a property of an exact source revision, not a permanent property of the Petra conversation. Approval remains the governed record's actual status.

Generation, delivery, receipt, application and duty acceptance are separate evidence states. Information-only delivery creates no invented acceptance obligation. A challenge can be recorded, assigned, pending, dispositioned or escalated; closure requires the responsible disposition. Research states use the common views. Material changes cause reassessment of affected views; containment may be selective to the affected entity/use rather than a universal outage. Withdrawn historical records remain governed by lifecycle, not erased to imply that they were never presented.

| Governed state / entry | Allowed transition / authority and evidence | Expiry, failure and closure |
| --- | --- | --- |
| Scoped request: entity, question and purpose identified | Current checks permit preparation; ambiguous inputs go to human clarification; record exact request/context | Due/cover handling follows approved profile; no guessed timeout; refused/referred states retain reason/owner |
| Prepared/validation-pending representation: exact canonical revision selected | Meaning/controls validated for approved audience/channel → permitted release; interface validation cannot approve source analysis | Failed transformation or controls → contained/owned referral; material change removes affected release validity |
| Released representation: current permission and validation evidence | Evidence may establish delivery/receipt/application separately; purpose-specific human responsibility only on acceptance | Unknown outcome retained; retry reconciles effects/current controls; supersession/withdrawal and affected duties recorded |
| Challenge/correction pending: exact target and material impact known | Accountable analytical/use/human owner reviews and records disposition; affected presentations marked/contained | Missed due/absent owner uses cover/escalation; closure requires evidenced disposition, not interface silence |
| Research assigned/run/finding/disposition | Approved profile/powers → actual coverage/finding → empowered human disposition; common state meanings govern | Stale/failed/unperformed coverage retained with recovery duty; no-material-finding only for completed bounded coverage |

## 6. Functional contracts

These are component views of existing IF/REC/KX definitions. They introduce no independent schema or new exchange identifier. Each exchange declares source/target owner, exact compatible revision, entity/purpose, authority/use, assurance, correlation, limitations and purpose-specific acknowledgement. Missing semantics or incompatible revisions fail into an owned referral. Actual schemas, binding, timeout/retry values and channel implementations remain later gates.

| ID | Producers → consumers / semantics and failure |
| --- | --- |
| AOS-24-CON-001 | 20/21/22/23/25/02 → 24: canonical analysis/evidence and scoped assessment views, AOS-20-IF-001/REC-E/Q, Shared §4.4; exact revision, evidence/inference, dissent, uncertainty and review scope; unavailable content is not reconstructed by guess |
| AOS-24-CON-002 | 01/03/04/05 → 24: powers, independent use, agent/evaluation and runtime views REC-A/D/X, KX-11/12/16–20; unknown/stale/conflict prevents affected release |
| AOS-24-CON-003 | 24 → permitted internal audiences/14: KX-14 projection, linked canonical source, audience/purpose/rule/payload/limits/assurance/withholding, agreed resident channel and exception status; 14 owns external delivery under AOS-14-IF-001 |
| AOS-24-CON-004 | Humans/24 ↔ 22/23/25/30: scoped question, challenge and analytical/human handoff; existing GI canonical view and KX-26; confirmation is not an approved decision; human records through AOS-30-IF-001/KX-06 v0.3 |
| AOS-24-CON-005 | 21/22/23/25/02/03/30 ↔ 24/14/affected owners: KX-13 exact correction/restriction/impact, old/new source and representation revisions, effective scope, reassessment and outstanding duties; material human-workflow impacts include 30 |
| AOS-24-CON-006 | 24/14/13/30 ↔ appropriate owners: KX-21/26 receipt/validation/application/responsibility and protected human handoff; information-only receipt is distinct from accepted duty; unknown external effect is reconciled before repetition |
| AOS-24-CON-007 | 24 ↔ 02/03/04/05/21–23/25/30: KX-15/17 and REC-E/Q governed audit, evaluation and outcome feedback; records do not auto-calibrate norms/precedent/preferences |
| AOS-24-CON-008 | 24/04 ↔ 14/02/01/30: RSVIEW-0.1 profile/run/finding/disposition under 04 CON-009 and 02 CON-007; retrieval permission, exact baseline, coverage and owned disposition; no self-approval |

Ordering/correlation follows the relevant entity/source/request scope, not a global total order. Duplicate handling preserves separate duties and independent evidence. Each retry checks current restrictions and known effects. Permission revocation/correction is not repaired by delivering the same cached view. Producers/consumers must adopt compatible semantics before operational reliance. AOS-25 is now a drafted functional counterpart; Register §20 records its views alongside this component’s §19 allocation; actual compatibility remains an operational gate.

## 7. Authority, discretion and human judgement

Petra may explain a permitted canonical position, help clarify a question and request review. The interface owner may approve ordinary presentation settings only under conferred powers. Analytical owners revise analysis. Data-use and disclosure exceptions remain with empowered 03/01 owners. Independent preparation configuration is governed independently of the tested executive. Charter changes and constitutional referrals follow 01/30; only the board changes telos.

Chair draft review does not itself create a board decision; authentication may support an evidence route under DEC-103, with decision validity and minutes approval separately assessed. A decision extract requires its exact authorised source; a labelled presentation cannot supply missing approval. Agreement in conversation cannot become approved precedent or a delegated task by implication. Human Mode 2 judgement remains permanently human, including adjudication of legitimate competing goods, normative interpretation and legitimacy. AOS-24 supports that judgement without supplying an artificial moral mandate.

Semantic explanation is the default under DEC-027. A recorded limited-explanation exception does not waive use enforcement. Affected persons' legitimate interests and welfare require purposeful explanation and an accountable route, not unrestricted visibility or inferred personal preferences.

## 8. Principle and Governance Intelligence Test traceability

All ten FP principles apply; the original text remains controlling. These are component contributions, not substitute definitions or evidence of institutional success.

| FP v4 principle | AOS-24 application / anchors |
| --- | --- |
| FP1 Telos, conferred purpose and function | A fluent interface supplies function, not telos or moral authority; §7, REQ-006/016/021/040 |
| FP2 Mode 2 is permanently human | Explanation preserves human adjudication and protected deliberation; REQ-005–006/017/023 |
| FP3 Architectural integrity | Audience rules and interface defaults must preserve organisational values and expose developer steering; REQ-008–012/039 |
| FP4 Radical transparency | Significant reasoning is legible, sourced and contestable to affected people within permitted disclosure; REQ-003–004/010–012/015/018 |
| FP5 Bounded rationality and structural imperfection | Failures, misunderstanding and power asymmetry have contained owned routes; REQ-024–033/040 |
| FP6 Epistemic humility | Confidence does not replace comprehension; retain gaps, dissent, unknown states and challenges even in apparently smooth operation; REQ-002–004/011/015/030/039 |
| FP7 The no-exit obligation | Accessible resident explanation and agreed channels; silence is not consent/satisfaction; REQ-018–020/022 |
| FP8 The constitutional mediator principle | Exact Chair/board/decision scope, no persona adjudication or invented approval; REQ-005–006/016–017/023 |
| FP9 Compliance as consequence | Purpose-led fidelity precedes compliance display; a label/dashboard does not prove governance effectiveness; REQ-007/021/039 |
| FP10 Complexity and emergence | Governed feedback and interface research support adaptation without predicting optimal governance or automatic calibration; REQ-034–040 |

All nine RP domains have these explicit contributions.

| RP v6 domain | AOS-24 contribution / requirement anchors |
| --- | --- |
| 1 Architecture and Completeness | Owned feedback/handoffs; reveal missing/infeasible options from canonical analysis; no AI-said-so authority; 001–004/015/033/040 |
| 2 Mode 1/Mode 2 | Present judgement boundaries and protect human deliberation; 005/016–017/021/023 |
| 3 1+5 Architecture | Explain combined domain evidence without becoming another intelligence; 001–003/014/040 |
| 4 Options and Decisions | Actual-state consequences and confirmed feedback preserved, not fabricated learning; 002/006/022/040 |
| 5 Blind Spots and Honesty | Uncertainty, withholding, challenge and unknown status; 003–004/011–015/028–030 |
| 6 Ethics and Telos | No synthetic moral authority/winner or silent precedent/norm calibration; 006/016/021–025/040 |
| 7 Radical Transparency | Source-backed explanation, permitted honest limits and audit; 003–005/010–012/032 |
| 8 Agentic Delegation | Scoped interaction, separate powers/effects, owned duty and research; 016–017/025/028–038 |
| 9 Data and Sensing Boundaries | Purpose, use, agreed channels and no inferred feelings; 008–012/020/022–023/031 |

The table accounts for all 29 GT tests. Contributions are technical support, never an executed pass or machine substitute for human governance.

| Test | Presentation contribution / enduring human limit |
| --- | --- |
| M1.1 Strategy | Explain sourced strategic position/options; humans set strategy |
| M1.2 Sensing | Expose domain/source scope and gaps; rendering adds no sensing |
| M1.3 Risk | Preserve general risk assumptions/limitations and human response responsibility; CAP-02-specific results deferred to Phase2, no current core prerequisite. |
| M1.4 Board capability | Accessible preparation/challenge; humans assess board capability |
| M1.5 Performance | Faithful measures and uncertainty; interface cannot certify performance |
| M1.6 Compliance | Preserve applicable source/status; empowered humans determine response |
| M1.7 Governance documents | Distinguish draft/approved and assessment dimensions; humans approve |
| M1.8 Accountability | Exact status, owner and duty route; delivery alone is not accountability |
| M1.9 Value for money | Explain actual options/consequences; humans adjudicate value |
| M1.10 Human–AI norms | Transparent AI voice and scoped confirmation; human institutions confer powers |
| M1.11 Learning | Evidenced misunderstanding/outcome feedback; no automatic precedent |
| M1.12 Continuous self-assessment | Interface evaluation/research coverage visible; humans oversee adequacy |
| M1.13 Emergence | Route new material patterns/questions to analysis; no hidden new conclusion |
| M1.14 Golden Thread | Claims link through exact corpus/analysis/decision; governing coherence remains human |
| M2.1 Values | Preserve competing stated values; no moral winner supplied |
| M2.2 Coherence under pressure | Refuse status/uncertainty laundering despite urgency; humans resolve tension |
| M2.3 Incommensurable trade-off | Unranked common-basis divergence including inconvenient readings; humans choose |
| M2.4 Epistemic brake | Visible limits, containment and owned referral; no automatic reversal of human decisions |
| M2.5 Independence | Governed challenge window and protected routes; no executive veto |
| M2.6 Legitimacy | Honest standing, challenge and explanation; legitimacy is not a persona property |
| M2.7 No exit | Purpose-bound accessible resident/staff explanation; no inferred consent from silence |
| M2.8 Transparency | Permitted evidence and material withholding disclosed; unlimited access is not required |
| M2.9 Moral drift | Preserve exact approved meaning/status and route challenges; 25/humans review drift |
| M2.10 Purpose stability | No presentation-driven telos or normative calibration; only empowered governance changes it |
| M2.11 Murmuration | Explain cross-domain interactions from canonical synthesis; collective effects assessed elsewhere |
| M2.12 Constitutional requirements | Identify human constitutional referral; interface cannot adjudicate |
| M2.13 Developer frameworks | Expose evaluated steering/assumptions; developer defaults supply no governing mandate |
| M2.14 Purpose-led design | Meaning/access/use follow organisational purpose, not persuasive engagement |
| M2.15 Telos versus function | A helpful fluent answer demonstrates function, not conferred purpose or legitimacy |

## 9. Data, privacy and disclosure

Data includes canonical claims/evidence, question/context, permitted human statements, projection rules, audience/channel needs, transformation checks, delivery/approval states, challenges and corrections. Collect and retain only what the declared purpose and governed lifecycle require. A helpful conversational feature does not justify speculative emotion inference, unrestricted conversation memory or cross-entity disclosure. Resident needs/preferences are purpose-bound human records, not inferred profiles.

KX-14 defines permitted projections. Redaction must not make a partial view look complete or authoritative. Links, attachments, downloads and machine/API outputs inherit the same use boundary; a link is not permission to reveal the underlying record. Material limits can be explained without revealing protected content. If a meaningful permitted explanation is unavailable, record the unresolved scope and human route. Lifecycle/deletion/location follow 02/03/05/KX-15, retaining only authorised histories and dispositions.

## 10. Normal and degraded flows

**Normal explanation:** scope question/entity/audience → fetch exact canonical revision and review/approval evidence → current independent powers/use checks → prepare permitted accessible projection → validate material meaning/limits → release through agreed channel → record evidenced status and route challenges. A simple clarification can stay within the same position; a changed assumption or requested new option goes to 22, a new assessment to 23, human adjudication to 30.

**Independent preparation:** approved independent profile/window → common canonical evidence → faithful unranked challenge presentation → protected governed recipients → management response retained at its required stage → human review/decision recorded by 30. Presentation is neither always secret nor a mechanism for delaying mandatory protected reports.

**Correction:** changed source/analysis/approval/use/assurance → identify material affected representations → contain or mark obsolete reliance → notify exact impact/reassessment owner, including 30 when its workflow is affected → produce newly validated projection → retain permitted correction/delivery history and outstanding duties.

**Normal research:** approved profile/trigger → controlled 14 retrieval → source/date/coverage and relevance assessment → exact affected-element proposal → empowered human disposition/change control → recorded outcome. **Degraded research:** missing/failed/stale coverage → explicit coverage limitation → owned recovery/cover/escalation → no silent no-finding or self-amendment.

## 11. Failure, refusal and recovery

| Failure | Required functional response / owner |
| --- | --- |
| Missing/changed canonical revision or misleading transformation | Stop affected claim/release, identify limit and refer to analytical/interface owner; do not reconstruct a preferred answer |
| Restricted evidence or unknown use permission | Contain affected disclosure, explain permitted limitation, route exception if applicable; 03/01 retains enforcement |
| New conclusion demanded in a summary | Refer substantive work to 22/23/25; preserve the existing position's exact standing |
| Board approval absent / action effect unknown | Keep pending/unknown state and refer 30/13; persona wording cannot fill the gap |
| Channel inaccessible or delivery uncertain | Preserve status and owned recovery through agreed alternatives; no inferred receipt/consent |
| Suppression/blocked protected duty | Use empowered alternate protected route with minimal permitted evidence and retained duty |
| Prompt injection or unsafe evidence link | Treat content as untrusted evidence, reject instructed power expansion, contain exposure and route incident |
| Change/recovery of model or cached view | Revalidate affected canonical/control state and evaluated fidelity before release; no automatic replay |

Recovery demonstrates current compatible revision, permission, assurance, transformation validation and effect reconciliation for the affected scope. The interface owner coordinates with 03/04/05/14 and the analytical owner; 30 owns human duty resolution. Recovery evidence does not imply organisational effectiveness or retrospective authorisation.

## 12. Evidence and audit

Reconstruction connects human request/context → canonical/evidence revision → identity/capacity and powers/use decision → presentation/profile/transformation → material limitations and status → release/delivery evidence → challenge/correction → owner/disposition/outcome. Preserve model/method/profile revision, observed/effective times, evidence versus inference and remaining duties proportionately under approved lifecycle. Logs must not leak more than the permitted representation. A challenge history can be preserved without treating every conversational exchange as organisational precedent.

## 13. Security and quality attributes

Functional quality is judged by semantic fidelity, contestability, accessibility for approved needs, truthful status, controlled disclosure, correction reach and human handoff completion. Evaluation samples include missing evidence, numerical/conditional changes, opposing trade-off readings, long/short and enabled translated/multimodal formats, adversarial instructions, ambiguous approval and revoked access. Compare claims and presentation emphasis with the exact canonical source; a fluent answer or engagement metric is insufficient.

Use approved quality/false/missed-error rubrics and release criteria under 04/05/KX-17. Model, channel and profile changes remain governed. Latency, availability, languages, formats, sample sizes, retention and numerical thresholds require appointed owners and approval before operational reliance; no hidden default is supplied. Security follows the kernel/14 controls and includes evidence-link/attachment use, caches, external release and prompt injection.

## 14. Invariants

| ID | Invariant / anchors |
| --- | --- |
| AOS-24-INV-001 | Representation changes no canonical conclusion or material limitation; REQ-001–004/019, VER-001–004/015 |
| AOS-24-INV-002 | Provisional/reviewed/Chair/board/action states never substitute for one another; REQ-005/016–017, VER-005/013–014 |
| AOS-24-INV-003 | Permission and audience interest remain separate; material withholding stays honest; REQ-008–012/030–031, VER-008–010/022 |
| AOS-24-INV-004 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-24-INV-004 (deferred under DEC-097); identifier retained for traceability only. |
| AOS-24-INV-005 | Persona supplies no moral authority, inferred feelings or live protected participation; REQ-021–025, VER-017–019 |
| AOS-24-INV-006 | Changed revisions/permissions invalidate affected reliance; delivery and duty states require evidence; REQ-026–029, VER-020–021 |
| AOS-24-INV-007 | Research/evaluation/feedback proposes governed change, never silent norms/precedent; REQ-034–040, VER-024–026 |

## 15. Verification and acceptance plan

All cases are **planned, unexecuted**. Common preconditions: controlled exact source/analysis/control/profile revisions, permitted test data, named analytical/interface/use/human owners and approved test scope. Common procedure: execute the stated stimulus in a representative authorised environment, inspect outputs/withheld views/links/statuses and owner handoffs against the canonical baseline, then reconstruct relevant permitted records and effects. Evidence: inputs/revisions, checks/projection, actual outputs/limits, transformation/evaluation results, delivery/impact/disposition records and assessor conclusion. Expected outcomes below supplement that procedure. Assessor: competent appointed interface/analytical reviewer, with independent use/security/human-governance specialist for affected boundaries; operating independence is not waived by deferred independent project review. Retest after a material change under the approved evaluation scope.

| ID | REQs | Case-specific precondition / stimulus → expected outcome and acceptance evidence |
| --- | --- | --- |
| AOS-24-VER-001 | 001 | Two entity/analysis revisions are available → request one scoped position → output binds only the exact selected revision/entity; inspect source and projection identity |
| AOS-24-VER-002 | 002 | Canonical position has material dissent/conditions → request executive/API/short versions → each preserves meaning; new conclusion referred; compare actual representations |
| AOS-24-VER-003 | 003 | Claim has facts and inference with permitted source route → inspect explanation/citations → each material claim traceable and distinctions clear; inspect links and provenance |
| AOS-24-VER-004 | 004 | Canonical result has decisive gaps/low assurance → request one-line summary → material limits stay adjacent or claim withheld; compare summary with source |
| AOS-24-VER-005 | 005 | Provisional, reviewed, Chair-approved draft and board-approved record fixtures → display each → exact status/approval scope shown, no review-as-authorisation; inspect approval evidence |
| AOS-24-VER-006 | 006 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-24-VER-006 (deferred under DEC-097); identifier retained for traceability only. |
| AOS-24-VER-007 | 007 | Strong document quality but unsupported practice claims → show assessment → three dimensions distinct with limitations; inspect view and supporting assessment |
| AOS-24-VER-008 | 008/009 | Valid access/legitimate interest but denied purpose-use → request projection → disclosure contained with permitted reason/referral; inspect independent REC-D decision |
| AOS-24-VER-009 | 010 | Two audience rules from one source → generate views → source/rule/purpose/payload/limits/withholding retained and common meaning faithful; inspect KX-14 records |
| AOS-24-VER-010 | 011/012 | Decisive evidence restricted and exceptional explanation requested → project/review → honest partial scope or withheld claim, owned exception, no enforcement bypass; inspect view and disposition |
| AOS-24-VER-011 | 013 | Ambiguous entity/question and human assertion → converse → question scoped, assertion/confirmation not promoted to verified evidence; inspect interaction and canonical record |
| AOS-24-VER-012 | 014/015 | Human disputes an assumption and requests new options → interrogate → challenge preserved and revised analysis referred with unresolved status; inspect owner/duty and later exact disposition |
| AOS-24-VER-013 | 016 | Human says yes to wording/context → inspect downstream records → scoped confirmation only, no decision/precedent/unrelated-use/duty approval; inspect all relevant consumers |
| AOS-24-VER-014 | 017 | Human asks to execute while powers absent or effect unknown → request action → governed handoff and truthful evidenced status, no reported completion; inspect 30/13 checks/effect record |
| AOS-24-VER-015 | 018/019 | Approved accessibility/translation format with units and condition → transform, include deliberate meaning error → faithful valid output or marked/withheld failed transformation; inspect source comparison and evaluation |
| AOS-24-VER-016 | 020 | Resident agreed channel unavailable and silence follows → attempt recovery → permitted agreed alternative/owned failure, no inferred consent/receipt; inspect channel and outcome evidence |
| AOS-24-VER-017 | 021/022 | Warm Petra interaction with inferred-emotion temptation → respond → clear AI/human route, no interiority-as-evidence or inferred feelings/weights; inspect response/use record |
| AOS-24-VER-018 | 023 | Request live protected meeting participation with permitted preparation available → attempt entry → live boundary maintained, preparation/post-meeting route permitted only within scope; inspect powers and records |
| AOS-24-VER-019 | 024/025 | Governed independent window, management response due and executive suppression attempt → present/report → independent profile preserved, response retained and mandatory protected duty reaches alternate route; inspect exact audience/window/duty evidence |
| AOS-24-VER-020 | 026/027 | Material evidence/approval/use change affects pack and decision → propagate correction → affected views contained/marked, old/new impact and owners notified including 30; inspect remaining duties and reassessment |
| AOS-24-VER-021 | 028/029 | Generated view, uncertain delivery and later revocation → retry → no fabricated receipt/acceptance or blind repeat; current checks/effects reconciled; inspect actual states and release |
| AOS-24-VER-022 | 030/031 | Stale controls and source instruction/link bypass → attempt disclosure → affected release contained and untrusted instructions rejected, links share use restrictions; inspect outputs/checks/incident route |
| AOS-24-VER-023 | 032/033 | Unresolved challenge with absent owner/expired due handling and lifecycle limit → review → assigned cover/escalation, reconstructable proportionate trail and governed disposition; inspect record/lifecycle actions |
| AOS-24-VER-024 | 034/035/036 | Approved research profile/trigger and current primary source → run normal research → bounded retrieval, exact dates/coverage/baseline/affected elements and qualified finding; inspect common research records |
| AOS-24-VER-025 | 037/038 | Material research finding plus failed/stale coverage → route/recover → empowered disposition, owned recovery and distinct limitation, no automatic amendment/no-finding success; inspect powers/profile/version history |
| AOS-24-VER-026 | 039/040 | Material model/profile change and misunderstanding outcome → evaluate/feedback → fidelity/steering/leakage/accessibility checks before authorised use, evidenced feedback to owners without norm/precedent calibration; inspect evaluation/change/outcome records |

Each requirement has one linked primary case; each case lists its requirements. These cases test the component contribution, not the permanent human judgement in §8. Production assessment additionally needs agreed scope/rubric, representative adversarial/error samples and evidence of counterpart/recovery behaviour.

### 15.1 Planned conformance claims

Each claim is **planned/unsubstantiated**, initial history 0.1, not an achieved conformance assertion. Actual claims require tested versions, date, named assessor and separate execution evidence; longitudinal correction/feedback is assessed across material revision and delivery cycles, not just a single rendering.

| ID | Source → requirements/functions → responsible contracts → acceptance evidence |
| --- | --- |
| AOS-24-CR-001 | WP Presentation; FP4/6; DEC-017/049–053/069/091 → REQ-001–012, FUN-001–002 → CON-001–003 → VER-001–010: faithful claim, review, divergence, assessment and permission/withholding evidence |
| AOS-24-CR-002 | RP2/6/9; DEC-008/041/081/083/085/087/088 → REQ-013–025, FUN-003–005 → CON-003–004/006 → VER-011–019: scoped conversation, accessible meaning, honest persona and protected human route |
| AOS-24-CR-003 | DEC-028–030/047/054–078/089 → REQ-026–033/039–040, FUN-006–007 → CON-002/005–007 → VER-020–023/026 across correction/delivery/change cycles: no obsolete reliance, false receipt or ungoverned calibration |
| AOS-24-CR-004 | DEC-086/template v0.4 §4.4 → REQ-034–038, FUN-008 → CON-008 → VER-024–025: controlled normal research, actual degraded coverage, owned human disposition without self-amendment |

## 16. Dependencies and delivery stages

Stage 1 is this functional review draft and source/common allocation. Stage 2 appoints interface/analytical/disclosure/independent/duty owners and approves audience/channel/accessibility/research/evaluation profiles and exact contracts. Stage 3 implements only authorised scope with compatible counterpart adoption, including the drafted 25 view where required, with actual compatibility separately evidenced. Stage 4 executes verification, records failures/recovery and obtains empowered release approval. No stage is inferred from completion of drafting.

AOS-21–23/25 and 30 are drafted functional counterparts; next GI-set consistency/disposition review, then AOS-40 scenarios. Kernel/14/common contracts retain their standing. Interface delivery depends on exact analytical inputs, approved use/powers, runtime/evaluation and evidenced human/action statuses. It can support the repair demonstration only within the already authorised demonstration boundary; this document adds no autonomous scope.

## 17. Issues, assumptions and decisions

| ID | Owned open item / gate |
| --- | --- |
| AOS-24-ISS-001 | Mark: wording/whole-document review; before specification baseline approval; no additional general architectural question identified |
| AOS-24-ISS-002 | Organisation/01/03/interface owner: appoint roles/cover/powers and legitimate-interest disclosure/exception review policy; before operational disclosure |
| AOS-24-ISS-003 | Interface owner/14/03: approved needs, languages/formats/channels and resident agreements; before enabled use, no guessed defaults |
| AOS-24-ISS-004 | Interface/analytical/04/05 owners: evaluation rubric, thresholds, representative samples, release/recovery evidence; before affected operation |
| AOS-24-ISS-005 | Semantic owners: exact binding/schema/version/acknowledgement/lifecycle/location and demonstrated counterpart compatibility; AOS-25 functional adoption is complete, operational compatibility remains required before reliance |
| AOS-24-ISS-006 | Interface/research/change owners: approved profile, assignment/triggers, coverage criteria/duty routing; before research operation; no new scheduled task |
| AOS-24-ISS-007 | Mark: independent project review deferred; operating independent governance and protected duty remain required |

All ISS rows are open, initial history 0.1. ISS-001/007 are review dependencies; ISS-002–006 are operating setup dependencies. Their source is the named controlling boundary/profile in §§4/6/7/13/15 and template v0.4; affected capability/function/contract and evidence are those named in each row and corresponding sections. No research finding or closed resolution is claimed.

Settled DEC-005/008/017/018/024–027/041/062–091 are applied, not reopened. Operational parameters and role appointments are legitimate later gates, not missing general design choices requiring fresh approval now.

## 18. Non-normative implementation notes

Reports, conversational text, APIs, translated views, audio or visual formats are possible implementations where approved. A shared presentation/agent service is permissible. Canonical positions need not mean identical wording: materially equivalent representation and governed permitted disclosure are the functional test. No vendor, wire schema, UI flow, model, language list, performance value or deployment topology is selected here.

## 19. Traceability and change control

§4.3 links exact sources/derivations to requirements and §15 cases. §§4.1–4.2 map capabilities/functions; §6 maps unchanged shared views; §14 binds invariants; §8 accounts for governing principles and all GT tests. Changes to presentation that alter governing meaning become analytical/constitutional changes with empowered review, not silent editorial amendments. Material common changes must propagate to affected components. The preserved source manifest, parent requirement/case statuses and DEC-001–091 remain unchanged.

Author checks cover unique IDs, requirement/case completeness, functional contract and source links, document structure and counterpart reference alignment. They are not execution, independent assurance or readiness approval.

## 20. Handover and human continuity

The interface owner maintains the exact baseline, approved presentation/disclosure/research/evaluation profiles, permitted audit/recovery evidence, open challenges and due/cover/escalation duties. Successor handover includes source/status and restrictions, affected obsolete views, pending delivery effects and protected obligations. Human decision and constitutional authority remains with the empowered institutions. Builders have implementation discretion only within separately authorised scope and compatible exact contract/profile versions. Stop affected work and refer missing powers/use, conflicting canonical meanings, unapproved required settings or unsupported release claims; drafting is not build or activation permission. Interface unavailability must leave a usable permitted human route for material duties.

## 21. Specification quality and design adequacy

| AOS-QS coverage | Evidence / limits |
| --- | --- |
| QS-01–03 | Controlled purpose/source/authority and draft standing in §§1–3; source manifest preserved |
| QS-04–10 | Stable atomic proposed requirements with sources/rationale/owner/status/history/dependencies/cases; §§4/15 |
| QS-11–14 | Boundaries, states, contracts, flows and failure in §§3/5/6/9–11; schema/parameters explicitly later gates |
| QS-15–20 | Human powers, uncertainty, evaluation, research, audit and controlled change in §§7–13/19; no runtime evidence |
| QS-21–24 | Planned acceptance and owned issues/stages/handover in §§15–17/20; cases unexecuted |
| QS-25–28 | Traceability/change and author checks; independent project review deferred and no achieved readiness gate |

Specification-quality conclusion: a functional review draft with 40 proposed REQs, eight CON views and 26 planned cases. Design-adequacy conclusion: the component supports faithful, contestable and purpose-bound explanation while retaining the governing human boundaries; operational fidelity/accessibility/security and institutional effectiveness require the appointed reviews and evidence. No tailoring exemption, test pass, build/activation or achieved readiness approval is claimed. Mapped GI drafting is complete; next GI-set consistency/disposition review, then AOS-40 scenarios.


## Component summary

**Purpose/owns:** make exact GI positions understandable, contestable and accessible through faithful Petra conversation and governed audience representations. **Reserved:** analytical conclusions, constitutional/value judgement, source/precedent admission, human approval/action and external delivery remain with their named owners. **Receives/produces:** exact canonical evidence/status and current controls → permitted explanations/projections, scoped challenges, qualified delivery/correction feedback and owned referrals. **Research:** interface-fidelity/accessibility/disclosure developments under an approved shared or assigned profile, actual coverage and human change route. **States/dependencies:** §5, kernel/14/20/21–23/25/30, all functional counterparts drafted; no live assurance implied. **Conformant when:** CR-001–004 supported by executed §15 evidence within an authorised scope. **Open:** wording review, appointments/profiles, exact compatibility and operating/independent evidence in §17.


## Phase 2 scope disposition — 9 October 2026

DEC-097 controls over prior inclusion/annex statements. CAP-01/02-specific legacy requirements/cases are deferred and supply no current-core completion/acceptance obligation. General human judgement, independent challenge, evidence fidelity, cumulative risk/drift and protected reporting remain current. Existing closure of AT-CR-01–05 and pilot5b is retained; neither is reopened by this scope change. No case executed or operating approval granted.

**Allocation and source status:** Any older source/adoption row relying on deferred CAP-only IDs is a historical use-case contribution, not current-core coverage. Core source sufficiency must use the surviving general obligations and accepted evidence; no source is promoted by this deferral. Retained numbered totals count catalogue/trace entries, including deferred IDs, and must not be read as active-core requirement/test totals.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**Historical status notice — revision set:** AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3.

**Historical status notice — scope decision — 9 October 2026, DEC-097:** Mark has moved CAP-01 Trade-Off Divergence and CAP-02 Risk Register Assessment into Phase 2 as specific use cases built on AOS. They are outside the current architecture/specification completion scope and are not current build, acceptance or publication prerequisites. No use-case design, configuration, implementation or testing is scheduled now. DEC-017's architectural inclusion is superseded on this point; its original record remains history. General human judgement, evidence, data-use/authority, independent challenge and protected reporting controls remain in the architecture. Dedicated legacy use-case IDs are retained only as deferred trace references, with original wording parked in Phase 2 (deferred under DEC-097); mixed rows retain only their general architectural obligations in current scope. Earlier inclusion/next-task/annex-dependency statements are superseded.

**GI consistency closure — 7 October 2026:** Mark authorised GI-CR-01–04 corrections and closure. Functional drafting, reciprocal report-independence wording, decision/outcome consumer allocation, Mode 2 wording and current completion statements are reconciled. AOS-23 changes counterpart/current references only; its REQ/VER/CON rows are unchanged. AOS-00/Map v0.32, DEC-001–091; AOS-20 v0.5/21 v0.6/22 v0.4/23 v0.5/24 v0.3/25 v0.2/30 v0.5; AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.15/Core v0.6/Exchange Register v0.14/source matrix v0.15; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. The review v0.2 records closure evidence; next AOS-40 acceptance scenarios. Earlier dated baseline/next-step statements remain historical. No new DEC/IF/operating power, case execution or build/activation/readiness approval; independent project review remains deferred and operating human independence remains mandatory.

