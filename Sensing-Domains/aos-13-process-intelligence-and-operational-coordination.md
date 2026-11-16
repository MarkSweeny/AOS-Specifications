# AOS-13 — Process Intelligence and operational coordination

Document: aos-13-process-intelligence-and-operational-coordination · Source revision or record: v0.2 functional baseline, editorial edition 29 October 2026

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

| Document control | Value |
| --- | --- |
| Identifier / version / date | AOS-13 / 0.2 / 9 October 2026 |
| Status | Functional specification review draft; proposed requirements and planned verification |
| Architecture baseline | AOS-00 / Specification Mapv0.42; DEC001–096;9October2026 |
| Current component baseline |01–05v0.8;10v0.4/11v0.3/12v0.3/13v0.2/14v0.8/40v0.6;20v0.5/21v0.6/22v0.4/23v0.5/24v0.3/25v0.2/30v0.5 |
| Common baseline | Sharedv0.18/Corev0.6/ExchangeRegisterv0.17/COORDv0.2/KPRv0.1/Profilesv0.1 |
| Source / quality baseline | Preserved source manifest; FP v4; RP v6; Governance Intelligence Tests; AOS-QS v0.1; template v0.4 |
| Project owner / custodian | Mark Sweeny |
| Accountable operating owner | Process/operations owner; organisational appointment pending; each service, control and human-review duty has its own appointed owner/cover |
| Author / reviewers | Codex at Mark's request; author document checks; Mark functional review pending; independent project review deferred |
| Approval / gate | Existing directions govern drafting; exact requirements proposed; no whole-document approval, executed verification, G3/G4 or operating activation |
| Release scope | Process functional architecture and selected repair demonstration allocation; executable organisation/supplier/profile scope not yet authorised |
| Change history | 0.1 initial drafting; existing AOS-13-IF-001 preserved; no new DEC, approved schema, technology choice, numeric default or automatic deployment |

## 1. Purpose and scope

Process Intelligence keeps authorised work coherent from its trigger to its actual outcome. It records what should happen, compares that with what happened, coordinates bounded steps and ensures that exceptions reach an accountable human. It prevents a message receipt, a completed technical task or a cancelled automation from silently being treated as an accepted duty or a completed service.

The intended outcome is a reconstructable workflow: attributable evidence → current permissions and controls → accepted responsibility where required → authorised action → observed consequence → evidenced disposition and feedback. Every unresolved effect, missing source and failed handoff retains its actual standing and an accountable route.

Scope includes versioned process definitions, instance state, conformance/coverage monitoring, pattern and obligation signals, divergence dashboards, bounded workflow execution, exception queues, technical multi-agent coordination, handoff/cover, change impact, retries/partial effects/compensation, operational memory, recovery, cross-domain service integration, own external research and supplier realisation.

Process Intelligence coordinates; it does not grant authority, redefine source evidence, decide moral priority or make reserved human decisions. 01 owns authority; 02 shared records; 03 identity/use; 04 bounded tasks/effect meaning; 05 final runtime gate, shared accounting and recovery enforcement; 10–12 domain evidence/interaction boundaries; 14 external exchange; 22 canonical synthesis; 25 oversight; 30 software support for actual human decision-makers; 40 assurance. Risk is intrinsic to this domain. Logical coordination is not a requirement to replace every existing case-management system with one central engine.

## 2. Authority and sources

FP v4 and RP v6 govern. Approved decisions constrain the proposed requirement wording. Book 4 explains intent; it is not current law, a supplier commitment or evidence of implemented control. Common semantic owners remain authoritative even if one platform implements several functions.

| Key | Exact source / locator and use |
| --- | --- |
| ARCH | AOS-00 v0.37 §§3.1/4.2/6/9; Map §4 AOS-13; REQ-041–044/VER-019; v0.38 adds allocation only |
| FP / RP / GT | FP v4 principles 1–10; RP v6 domains 1–9, especially closed feedback/named human layers, Mode2, explicit delegation and purpose limitation; all 29 GT tests in Appendix A |
| B4 | Book 4 Process Intelligence: Capabilities pattern detection, obligation monitoring, workflow coherence, divergence dashboard and organisational memory; Constraints edge cases, audit, fallback, coherence paradox and bias; Compliance independent oversight |
| CONTROL | 01–05 v0.8; DEC-028–030/042–044/062–078; Control Coordination v0.2 CHECK/ACT/CHG/ACC/RSV/WHD/BRK; Protected Reporting and Recovery v0.1 |
| DATA | 02 v0.8; Core v0.6 REC-E/Q/A/D/X; Shared v0.15 §4.3 escalation and delivery/recovery; Register v0.14 KX-07/AOS-13-IF-001, KX-21, KX-26 and research views; DEC-045–048 |
| DOMAIN | 10 v0.2 REQ-013–020/032 and CON-004; 11 v0.1 REQ-017–030 and CON-003/004; 12 v0.1 human/rights/protected routes; counterpart revisions above retain all those obligations |
| REPAIR / HUMAN | DEC-036–041; Operational Profiles §§4/5; 30 v0.5 REQ-021–033; 40 v0.5 VER-007–010/038 |
| GI / RESEARCH | Current 20–25/30; DEC-086/088–091; 04 CON-009, 02 CON-007/RSVIEW-0.1; 14 collection, component specialist assessment and 01 human amendment remain distinct |
| SUPPLIER / QS | Mark's 8 October supplier-participation direction and build-agent/plain-language preference; AOS-QS v0.1 QS-04–28; template v0.4 |

### 2.1 External primary research checked 8 October 2026

| Source | Standing / bounded implication |
| --- | --- |
| EXT-01 | [OMG BPMN 2.0.2 specification catalogue](https://www.omg.org/spec/BPMN/), formal process-modelling reference with normative schemas and separate examples. A candidate representation, not a selected engine or an adopted executable AOS schema. Any modelling choice must preserve AOS permissions, states and human boundaries. |
| EXT-02 | [IETF RFC9110 §9.2.2](https://www.rfc-editor.org/rfc/rfc9110.html#section-9.2.2), HTTP standard; supports distinguishing repeated requests from safe repetition of business effects. Method semantics alone cannot prove that an external service action is reconciled or currently authorised. No HTTP transport is selected. |
| EXT-03 | [NIST AI RMF Core](https://airc.nist.gov/airmf-resources/airmf/5-sec-core/), voluntary risk-management framework; GOVERN roles and MAP3.5 human oversight inform evaluation responsibilities. It does not grant AOS operating authority or provide a compliance certificate. |

Book claims of perpetual full-population assurance, absence of a need for independent audits and examples implying an already-overdue legal inspection is merely a scheduling problem are not adopted. Coverage must be evidenced; independent assessment remains necessary; competent current-source profiles determine legal breach meaning. “Routine” or “clean transaction” is not a delegation rule. A workflow executes only its exact approved actions/conditions. Selected repair demonstration human expenditure/promise rules do not become universal production defaults. No ongoing monitoring/research schedule is activated by this draft.

## 3. Responsibilities and context

**Responsibility cross-reference (DEC-094; editorial clarification, 29 October 2026):** AOS-14 recognises an exchange-associated obligation and its source/context; the relevant domain steward determines substantive meaning/applicability. AOS-02 owns the common obligation-record semantics and structure/custody. AOS-13 tracks routing, accepted responsibility, fulfilment and unresolved duties. AOS-30 owns the human-workflow meaning of accepted responsibility and supports empowered human disposition/account. These are distinct responsibilities: recognition, record ownership and dispatch do not constitute human acceptance. The existing tracking owner retains the duty until explicit scoped transfer is accepted; failed delivery or exhausted cover does not create an ownerless success. Actual people, cover and response powers remain organisation-appointed prerequisites. No semantic ownership is transferred by this clarification.

| Responsibility | Process owns / authoritative counterpart |
| --- | --- |
| Definition and instance | Process owner stewards purpose, steps, dependencies, states and outcome rules; 01 authorises instruments; 02 holds records; 04 bounded task semantics |
| Execution coordination | 13 requests permitted work and tracks dependency/effect state; 04 executor and 05 final gate/accounting enforce; 13 cannot issue a substitute grant or private budget |
| Human handoff | 13 retains tracker, duty scope, deadline/cover and acceptance evidence; 30 supports actual empowered humans; KX-21 distinguishes stages; KPR protected route |
| Domain service | 10 owns condition/promise/completion evidence; 11 agreed-channel communication/private boundaries; 12 workforce/human decision limits; 13 connects duties without rewriting meaning |
| Cross-domain conflict | 13 preserves technical inconsistency and routes permitted evidence; 22 prepares canonical analysis; 30 humans adjudicate moral/authority questions |
| Learning and oversight | 13 supplies current scope/divergence/outcome and definition rationale; 21 knowledge custody, 25 drift oversight, 40 independent assessment; no self-amending optimiser |
| Research | 13 tracks findings for all components but owns only its specialist process research relevance; 14 retrieves, 02 stores, 30/01 disposition/amendment |

Trust boundaries include source to admitted evidence, definition to approved/applied execution, coordinator to independently enforced runtime, task to task, internal to external effect, sender to recipient/human acceptance, private/sensitive domain to permitted projection, old state to current recovered state, and technical ordering to moral judgement. Each commissioned route names role/cover/capacity; no personal recipient is invented here.

### 3.1 Supplier participation

Existing case/workflow/BPM tools, automation platforms, process-mining/conformance analytics, event/integration services and operational reporting can implement these logical functions. One platform can realise 13/14/30 support and parts of domain services; several products can contribute to 13. AOS does not require replacing capable supplier software or rebuilding its analytics internally.

| Supplier offering | Candidate fit / what must be demonstrated |
| --- | --- |
| Case/workflow/BPM platform | Definitions/instances/accepted duties and outcomes; CON-001–003; versioned source/case master, human acceptance, exceptions and closure |
| Automation/RPA/agent runtime | Bounded step execution; CON-004; exact current shared checks, attempt/effect evidence, partial result and retry reconciliation |
| Process mining/conformance analytics | Coverage, divergence/patterns; CON-006; actual admitted populations, applicable definitions, uncertainty and no silent individual inference |
| Integration/event services | 14/02 exchange with 13 correlation; identity/ordering/duplicates/exact versions/access and effect acknowledgement |
| Operational dashboards/memory | CON-006/007; role-limited unsmoothed exceptions, current owner/state, actual outcome and historical rationale |
| Service/HR/resident suites | May realise domain functions plus 13 lifecycle; source purposes/private barriers/human decisions preserved across internal product flows |

Standalone/manual, API/event and combined arrangements are assessed against declared scope. Manual assistance cannot claim automatic integration. A vendor's “exactly once”,“compliant” or “case closed” label cannot replace observed AOS effect, permission, ownership or outcome evidence. Declare one authoritative source per meaning and responsibility for reconciliation; not one universally authoritative product. §18's example and §20's response matrix distinguish functional fit from executable mapping and tested conformance.

## 4. Capabilities and functions

### 4.1 Capabilities

| CAP | Outcome / REQ allocation |
| --- | --- |
| AOS-13-CAP-001 | Versioned process/evidence and bounded monitoring; 001–010 |
| AOS-13-CAP-002 | Currently controlled execution/change/accounting; 011–015 |
| AOS-13-CAP-003 | Accepted human/protected handoffs and continuing duties; 016–020 |
| AOS-13-CAP-004 | Reconciled effects, coordination, closure and operational memory; 021–029 |
| AOS-13-CAP-005 | Repair and other domain/human service integration; 030–042 |
| AOS-13-CAP-006 | Secure correctable recoverable assurance; 043–049/056–057 |
| AOS-13-CAP-007 | Own specialist external research; 050–054 |
| AOS-13-CAP-008 | Attributable supplier realisation; 055 |

### 4.2 Functions

| FUN | Trigger →inputs →behaviour/output / authority and failure |
| --- | --- |
| AOS-13-FUN-001 Define/activate | Approved process/change →exact manifest and applied acknowledgements →usable scoped definition or held gap; CON-001; CAP-001/002 |
| AOS-13-FUN-002 Admit/correlate | Permitted event →source/identity/revision checks →instance update with lineage or explicit conflict; CON-002; CAP-001 |
| AOS-13-FUN-003 Monitor/explain | Admitted event/time/profile trigger →actual versus intended evidence/coverage →bounded divergence/pattern/view; no complete assurance from silence; CON-006; CAP-001/006 |
| AOS-13-FUN-004 Coordinate effects | Ready permitted step →exact request/current controls/reservations →bounded attempted/prevented/partial/actual effect; CON-004; CAP-002/004 |
| AOS-13-FUN-005 Track human duty | Finding/blocker/rejection →permitted route/duty/cover →receipt/validation/accepted responsibility or owned exception; CON-003; CAP-003 |
| AOS-13-FUN-006 Coordinate repair |10 evidence +clock/profile →promise/completion classification →30 accepted owner and 11 agreed-channel contact/actual outcome; CON-005; CAP-005 |
| AOS-13-FUN-007 Coordinate domain review | Service/people/GI/research input →purpose-scoped evidence/independent human route →accepted duty/decision/application/outcome links; CON-003/007; CAP-005 |
| AOS-13-FUN-008 Reconcile/change/recover | Unknown effect/change/outage →current authority/use/account/evidence →selective reassessment, manual continuity and authorised continuation; all CON; CAP-004/006 |
| AOS-13-FUN-009 Learn without amendment | Actual outcome/near miss →permitted rationale/history →bounded lesson/proposal for human change; CON-007; CAP-004 |
| AOS-13-FUN-010 Research/assess supplier | Approved specialist trigger or supplier proposal →source/profile/evidence allocation →owned finding/gap/review; no activation from fit; CON-008/all CON; CAP-007/008 |

### 4.3 Proposed requirements and metadata

Each row is a proposed component-level obligation. Category, source and planned VER are explicit. Rationale is the relevant function's prevention of false outcomes, unowned duties, unapproved effects or concealed gaps. Owner: process/operations owner with §3 semantic/service/control stewards. Specification approver Mark; application approver empowered organisational authority. Every row has status **proposed**, scope **0.2 functional draft**; normative obligations retained from0.1, history **initial allocation 8 October 2026**. Dependencies are cited §2 sources/common definitions and §§6/16/17; CAP/FUN allocations above and case contracts supply unambiguous links. An unresolved profile value is not a build default.

| Requirement | Independently verifiable obligation | Source / derivation | Planned VER |
| --- | --- | --- | --- |
| AOS-13-REQ-001 | **Definition:** Each process definition shall identify its exact revision, purpose, scope, owner, governing instruments, permitted steps, human boundaries, exceptions and outcome/closure criteria. | ARCH/Map 13; B4 Constraints; 01; QS-14 | AOS-13-VER-001 |
| AOS-13-REQ-002 | **Activation:** A process function shall become usable only when its approved scope has compatible applied-state evidence from every required dependency. | DEC-068; COORD ACT; 01/05 | AOS-13-VER-002 |
| AOS-13-REQ-003 | **Instance:** Each workflow instance shall retain stable identity and the exact definition, source, organisation and profile revisions governing its current work. | 02; 04; QS-12/19; B4 audit | AOS-13-VER-003 |
| AOS-13-REQ-004 | **Evidence admission:** AOS-13 shall consume domain evidence without changing its source assurance, uncertainty, event/effective time or permitted-use standing. | 02 REC-E/Q; DEC-046; 10–12 | AOS-13-VER-003 |
| AOS-13-REQ-005 | **Coverage:** Process monitoring shall disclose its observed population, period, admitted events and missing, stale or failed coverage rather than claim completeness from a quiet feed. | RP5/7; B4 assurance limits; QS-18 | AOS-13-VER-004 |
| AOS-13-REQ-006 | **Divergence:** AOS-13 shall compare observed process behaviour with the applicable exact approved definition and retain the evidence of each material divergence. | B4 divergence dashboard; RP7; 02 | AOS-13-VER-005 |
| AOS-13-REQ-007 | **Dashboard:** Divergence views shall expose permitted transaction-level exceptions, ownership, uncertainty and outcome standing through role-appropriate projections. | B4 real-time assurance; 03; 22/24 | AOS-13-VER-005 |
| AOS-13-REQ-008 | **Pattern:** Process pattern outputs shall disclose source population, comparison baseline, assumptions, coverage and uncertain implications separately from facts. | B4 pattern detection; RP5/7; QS-18 | AOS-13-VER-006 |
| AOS-13-REQ-009 | **Obligations:** Obligation monitoring shall use a competent human-approved applicability and timing profile that distinguishes governing duties from internal targets and predictions. | B4 predictive compliance; 01/02; RP7 | AOS-13-VER-007 |
| AOS-13-REQ-010 | **No compliance certificate:** AOS-13 shall not treat successful workflow execution or early-warning prediction as proof that a legal duty or institutional governance test has been fulfilled. | FP9; DEC-091; 40; B4 assurance subject | AOS-13-VER-007 |
| AOS-13-REQ-011 | **Current effects:** Before each consequential effect, AOS-13 shall supply the exact operation/attempt to the shared current authority, use, runtime and applicable capacity checks. | DEC-067; COORD CHECK; 01/03/04/05 | AOS-13-VER-008 |
| AOS-13-REQ-012 | **No delegated expansion:** A workflow or coordinator shall not expand an agent's authority, tools, data use or task scope merely because a parent workflow was approved. | RP8/9; 04; DEC-042–044 | AOS-13-VER-008 |
| AOS-13-REQ-013 | **Reservations:** Linked work shall use the authoritative shared cumulative-account and reservation meanings rather than local counters that can be evaded by parallel tasks, splits or retries. | DEC-070; COORD ACC/RSV; 04/05 | AOS-13-VER-009 |
| AOS-13-REQ-014 | **Change impact:** A material definition, evidence, role, permission or channel change shall identify dependent pending work and required applied acknowledgements for selective reassessment. | DEC-069/089; COORD CHG; 02 | AOS-13-VER-010 |
| AOS-13-REQ-015 | **Revocation:** Late, duplicate or out-of-order change events shall reconcile current authoritative state and shall not revive superseded permission. | DEC-069; 01/03/05 | AOS-13-VER-010 |
| AOS-13-REQ-016 | **Tracking owner:** A duty-bearing handoff shall retain an accountable tracker until an empowered human explicitly accepts its defined responsibility scope. | RP1; DEC-066/075; COORD ACC; KX-21/26 | AOS-13-VER-011 |
| AOS-13-REQ-017 | **Acknowledgement:** AOS-13 shall distinguish receipt, validation, application and human responsibility acceptance according to the exchange's required acknowledgement profile. | DEC-066; KX-21; KXR-06 | AOS-13-VER-011 |
| AOS-13-REQ-018 | **Rejection and cover:** Rejected, unaccepted, expired or unavailable human handoffs shall remain owned with approved cover/escalation rather than silently becoming successful transfer. | RP1; KPR-03; 30 | AOS-13-VER-012 |
| AOS-13-REQ-019 | **Protected duties:** Required protected findings shall retain their permitted required audience and owned delivery/acceptance duty despite suppression or an implicated normal recipient. | RP8; DEC-073–075; KPR-01–03 | AOS-13-VER-013 |
| AOS-13-REQ-020 | **Blocker explanation:** Withheld work shall carry permitted blocker reasons, uncertainty and an authorised review/service-continuity route without disclosing forbidden content. | DEC-027/071; COORD WHD/BRK; 03 | AOS-13-VER-014 |
| AOS-13-REQ-021 | **Unknown effect:** Partial or unknown external effects shall remain explicit and undergo authorised reconciliation before consequential repetition. | DEC-030; COORD/KPR; 14/05 | AOS-13-VER-015 |
| AOS-13-REQ-022 | **Retry identity:** Retries shall preserve request/attempt correlation and prior-effect evidence while obtaining fresh exact-operation checks for each new attempt. | 04; DEC-028–030; Shared; EXT-02 | AOS-13-VER-015 |
| AOS-13-REQ-023 | **Compensation:** A compensating or reversing operation shall have its own current authority/use checks and preserve the original action and actual consequence history. | 01/03/04; DEC-029/030; REC-X | AOS-13-VER-016 |
| AOS-13-REQ-024 | **Multi-agent coordination:** Technical coordination shall declare bounded tasks, dependencies, recipient scopes and completion evidence without adjudicating incommensurable moral priorities. | Map 13; 04; 22/30; FP2; RP2 | AOS-13-VER-017 |
| AOS-13-REQ-025 | **Concurrency:** Concurrent or stale workflow workers shall not perform duplicate consequential effects or evade current shared-control and reservation scope. | DEC-067/070; 04/05; QS-23 | AOS-13-VER-018 |
| AOS-13-REQ-026 | **Cancellation and holds:** Holding or cancelling automation shall preserve known effects and separately authorised outstanding human/service duties. | DEC-072/075; COORD WHD/BRK; KPR | AOS-13-VER-019 |
| AOS-13-REQ-027 | **Closure:** Workflow closure shall require its defined outcome evidence and empowered disposition of outstanding obligations rather than equate terminal technical state with completed service. | RP1/4; 10–12/30; DEC-066/075 | AOS-13-VER-020 |
| AOS-13-REQ-028 | **Operational memory:** Process history shall preserve the exact definition rationale, changes, source/effect evidence and actual outcomes under governed access and lifecycle. | B4 organisational memory; 02/21; DEC-047 | AOS-13-VER-021 |
| AOS-13-REQ-029 | **No automatic optimisation:** A learned pattern or improvement proposal shall not change governing definitions, thresholds, priorities or permissions without authorised amendment and applied activation. | DEC-018/068/086; 01; B4 coherence paradox | AOS-13-VER-021 |
| AOS-13-REQ-030 | **Promise comparison:** The repair comparison shall use the resident-communicated completion commitment and approved date/time meaning supplied by 10/02, separately from internal targets. | DEC-036; 10 REQ-013/014; ARCH REQ-041–044 | AOS-13-VER-022 |
| AOS-13-REQ-031 | **Verified incomplete:** After the promised boundary, evidenced outstanding promised work shall generate the approved overdue-incomplete human route. | DEC-036/040; 10; Profiles; ARCH REQ-042/043 | AOS-13-VER-022 |
| AOS-13-REQ-032 | **Unverified completion:** Unknown completion after the promised boundary shall generate “completion unverified after promised date” with an owned verification escalation rather than definite incompletion. | DEC-039; 10 REQ-017; 40 VER-008 | AOS-13-VER-023 |
| AOS-13-REQ-033 | **Promise exception:** Missing or contradictory communicated promise evidence shall produce an owned evidence exception without an invented deadline or grace period. | DEC-036/037; 10; 02; RP7 | AOS-13-VER-023 |
| AOS-13-REQ-034 | **Promise changes:** Authorised communicated promise revisions shall preserve the original promise and breach history without automatically closing an existing escalation. | DEC-037; 10 REQ-015; 11 REQ-025 | AOS-13-VER-024 |
| AOS-13-REQ-035 | **Repair scope and dispute:** Partial or disputed repair evidence shall retain completed/outstanding scope and human dispute resolution without contractor flags or resident silence establishing completion. | DEC-038/040; 10 REQ-016–019; 11 REQ-026 | AOS-13-VER-024 |
| AOS-13-REQ-036 | **Repair human ownership:** The repair workflow shall obtain explicit empowered human responsibility and approved named-owner/accountable-team cover through 30. | ARCH REQ-043/044; 30 REQ-021–033; RP1 | AOS-13-VER-025 |
| AOS-13-REQ-037 | **Resident contacts:** AOS-13 shall coordinate 11's permitted agreed-channel delivery of current named-owner and accountable-team contact details and retain failed communication duties. | ARCH REQ-044; DEC-041; 11 REQ-017–024 | AOS-13-VER-025 |
| AOS-13-REQ-038 | **Repair outcome:** Repair-workflow closure shall preserve actual completion evidence, accepted human disposition, communication standing and any residual dispute or service obligation. | DEC-038–040; 10/11/30; RP1/4 | AOS-13-VER-026 |
| AOS-13-REQ-039 | **Complaint and service:** Service request, complaint response and outstanding repair/remedy actions shall remain distinct linked duties so a response or complaint does not silently end service work. | 11 REQ-027–030; 13 remit; 30 | AOS-13-VER-027 |
| AOS-13-REQ-040 | **People handoff:** People concerns, development proposals and rights requests shall use 12's permitted evidence and independent human routes without becoming automatic employment decisions. | 12 REQ-005–007/029/030/032; 30; RP2/9 | AOS-13-VER-028 |
| AOS-13-REQ-041 | **Governance/research handoff:** Governance and specialist research findings shall preserve distinct component reviewer duties, human disposition and separate amendment/activation standing. | 20–25/30; DEC-086; RSVIEW-0.1 | AOS-13-VER-029 |
| AOS-13-REQ-042 | **Cross-domain boundaries:** Coordination shall preserve source-purpose and audience restrictions, including resident private content and workforce sensitive/individual-inference boundaries. | 03; 11/12; RP9; DEC-050/088 | AOS-13-VER-030 |
| AOS-13-REQ-043 | **Correction and lifecycle:** Workflow records and derived/restored views shall apply governed correction, restriction, retention and deletion without erasing actual past effects or hiding deleted content. | 02/03; DEC-047/089; KPR | AOS-13-VER-031 |
| AOS-13-REQ-044 | **Security:** AOS-13 shall treat tool/source/model instructions as untrusted content rather than new authority and enforce organisation/task/recipient boundaries through approved controls. | 01/03/04/05; DEC-014; RP8/9 | AOS-13-VER-032 |
| AOS-13-REQ-045 | **Continuity:** When workflow infrastructure or evidence fails, AOS-13 shall disclose coverage and effect uncertainty and support the approved human/manual continuity route. | 05; B4 failure/fallback; KPR | AOS-13-VER-033 |
| AOS-13-REQ-046 | **Recovery:** Recovered coordination shall establish current authority/use/configuration/lifecycle and reconcile effects/reservations before scoped continuation. | DEC-076–078; KPR-04–06; COORD; 05 | AOS-13-VER-033 |
| AOS-13-REQ-047 | **Evaluation:** Probabilistic pattern, routing or interpretation claims shall use a human-approved task/population/error rubric and remain separate from deterministic enforcement results. | QS-18; 04; 40; B4 bias/novelty | AOS-13-VER-034 |
| AOS-13-REQ-048 | **Audit:** Consequential workflow evidence shall reconstruct trigger, exact inputs, actor, checks, applied rules, human decision, action and actual consequence without private chain-of-thought. | RP7; QS-19; REC-E/Q/A/D/X | AOS-13-VER-035 |
| AOS-13-REQ-049 | **Compatibility:** Each process producer and consumer shall declare exact common contract/view/profile versions and reject or hold unsupported meaning rather than silently coerce it. | DEC-065; 02; Register v0.14; QS-12 | AOS-13-VER-035 |
| AOS-13-REQ-050 | **Research profile:** AOS-13 external adaptation research shall use an approved component-owned specialist profile and common research meanings through permitted 14 retrieval. | DEC-086; 04 CON-009; 02 CON-007 | AOS-13-VER-036 |
| AOS-13-REQ-051 | **Research finding:** Own research findings shall distinguish verified source standing/dates, specialist interpretation and exact affected process-specification elements. | DEC-086; 14; RSVIEW-0.1 | AOS-13-VER-036 |
| AOS-13-REQ-052 | **Research coverage:** Own research runs shall expose actual complete, partial, failed or unperformed coverage and bound no-finding claims to their searched perimeter. | DEC-086; 04/02 §6.6 | AOS-13-VER-037 |
| AOS-13-REQ-053 | **Research human review:** Material own research findings shall have an accepted empowered reviewer or an owned unresolved handoff with approved cover/escalation. | DEC-086; 30; COORD ACC | AOS-13-VER-038 |
| AOS-13-REQ-054 | **Research amendment:** Own research acceptance or source publication shall not amend process controls, expand sensing or activate changed execution without authorised change and verification. | DEC-086/018; 01; COORD ACT | AOS-13-VER-038 |
| AOS-13-REQ-055 | **Supplier realisation:** Each supplier implementation scope shall maintain a versioned capability-to-requirement/contract allocation with actual conformance evidence or owned gaps/dependencies. | Mark 8 October supplier direction; QS-11/12/21/26 | AOS-13-VER-039 |
| AOS-13-REQ-056 | **Independent assurance:** AOS-13 shall expose permitted monitoring evidence and limitations for independent assessment while preserving that the monitoring/execution system is itself an assurance subject. | B4 Compliance; 40; DEC-091; GT | AOS-13-VER-040 |
| AOS-13-REQ-057 | **No forced fit:** An instance outside the approved process model shall produce an owned divergence rather than be forced into a nearest template that conceals material circumstances. | B4 coherence paradox; RP5/6; 04 | AOS-13-VER-040 |

### 4.4 External research and specification adaptation

Inherit 04 CON-009 and 02 CON-007/RSVIEW-0.1 unchanged. 13's coordination of other research handoffs is separate from its own specialist external research and from internal process monitoring.

| Profile element | Component-owned allocation |
| --- | --- |
| Remit/baseline | Exact 13 revision; workflow/modelling/coordination, service handoffs, distributed effects/retry/recovery, conformance/coverage, process analytics/novelty, bias and operational memory; exact affected elements |
| Developments/sources | Primary workflow/protocol/security/standards/research/incident and applicable service/regulatory sources; version/jurisdiction/effective standing explicit; source admission/currentness through 14 |
| Assignment/triggers | Process owner appoints bounded agent/shared service and approves cadence/event triggers/coverage; no schedule/tool expansion activated; ISS-006 |
| Controls | 14 retrieval; 01/03/04/05 purpose/tool/data/runtime limits; licensing/access constraints; no private/sensitive domain data merely for research, no source-instruction execution or calibration |
| Evidence/assessment | Publication/event/access/effective dates/status; verified content versus interpretation; exact affected CAP/FUN/REQ/CON; alternatives/uncertainty/materiality/urgency and cross-component effects |
| Coverage/quality | Complete/partial/failed/unperformed, bounded no-finding; approved relevance/fidelity/false-missed finding rubric; actual search perimeter and limitations |
| Human review/change | Accepted reviewer/window/cover/escalation; accepted/rejected/deferred/unresolved with reasons; separate 01 amendment, verification/applied activation and actual outcome |
| Records/adoption | Common exact profile/run/finding/disposition views; 02 custody, 14 collection, 13 duty tracking, 30 disposition, 01 amendment; deduplication/correction/lifecycle/impact meanings inherited |

Normal: approved trigger →permitted verification →specialist relevance/implications →finding/bounded no-finding →accepted human disposition →separate amendment/verification/activation →outcome. Degraded: failed/denied/stale/conflicting/partial source keeps actual coverage; unresponsive reviewer uses approved cover; urgent live consequences use separately permitted human response while amendment pending. VER-036–038 covers the eight required research dimensions. Shared findings have separately accepted component duties; collection/delivery is not review completion.

## 5. State model

Every transition identifies object/revision, actor, current authority, event/effective time, evidence and resulting scope. Profile deadlines can create expiry/owned exception; they never fabricate successful effect or human acceptance. Terminal technical state and continuing service duty are separate.

| Object | States / entry and transition / closure |
| --- | --- |
| Definition | Draft →authorised scope →compatibility/application pending →usable exact scope →held/superseded/retired. Approval alone not usability; new restriction blocks affected effects even during partial activation. |
| Instance | Received/identity unresolved →admitted →ready/running/waiting source or human →held/exception/reconciliation →outcome pending →evidenced disposition or technically cancelled/failed with residual duty. |
| Attempt/effect | Prepared →checked/reserved where applicable →prevented/dispatched →observed applied/partial/not applied/unknown →reconciled; new attempt needs current checks; compensation independent. |
| Handoff | Prepared/submitted/received/validated →empowered human acceptance of exact duty →in progress →actual disposition/outcome; rejected/partial/unresponsive retains tracker/residual cover. |
| Repair | Promise unresolved or established; comparison not-yet-due/evidenced overdue-incomplete/completion unverified after date/date exception; partial/disputed/completed evidence distinct; human escalation/communication/residual duty tracked independently. |
| Change/recovery | Impact identified →required acknowledgements pending →applied/no material dependency/unresolved; recovered isolated →current scope/effects reconciled →authorised continuation or held. |
| Research/lesson | Common research states; operational lesson/proposal is not amendment approval or activation. |

## 6. Semantic contracts and interfaces

Preserve **AOS-13-IF-001** for escalation/lifecycle meaning in Shared §4.3 and Register KX-07. CON views complement it; they do not replace common definitions or create an approved IF family. 02 owns record/acknowledgement structure, 01 authority, 03 use, 04 task/effect semantics, 05 runtime/account enforcement, source domains their evidence, 30 human decision support and 14 external exchange.

| CON | Producer →consumer / minimum meaning / failure and authority |
| --- | --- |
| AOS-13-CON-001 Process definition/application | Authorised owner/01/05/dependencies →13/02/executors: exact scope/revision/purpose/steps/states/conditions/source instruments/human boundary, closure/fallback rules, rationale and compatible actual applied manifest; unapplied/unknown meaning not usable |
| AOS-13-CON-002 Instance/event | Permitted domain/source/02/runtime →13→02/executors/reviewers: stable case/request/event/attempt identities, definition/profile/version, source assurance, time/standing, dependencies/pending work, current state/effects/residual duties; duplicates/order do not redefine truth |
| AOS-13-CON-003 Escalation/accepted duty |13/domain/control finding →permitted 30/human/recipient; stage result →13/02: existing 13-IF-001/KX-07, KX-21 and KX-26/WHD meaning; exact duty/source/limits, tracker, recipient/role/power, deadline/cover, receipt/validation/application/responsibility and residual rejected/unresolved scope; KPR protected route |
| AOS-13-CON-004 Controlled work/effect |13 →04/05/shared controls/external route 14; result →13/02: exact task/request/attempt/arguments/actor/current source vector, authority/use, CHECK/applied configuration, shared account/reservations, observed prevented/applied/partial/unknown effect and reconciliation; no private copy of grant or account semantics |
| AOS-13-CON-005 Repair/service coordination |10/02 evidence +30 human scope →13↔11/14/service source: original communicated promise/precision/scope/revisions, completion rule/work/inspection/dispute standing, comparison classification, accepted owner/team cover, permitted both-contact communication result, actual outcome/residual duty; domain meanings unchanged |
| AOS-13-CON-006 Monitoring/divergence |13/02 admitted observation →permitted service/22/24/25/40: population/period/coverage, exact intended definition versus observed transaction, source/assurance/uncertainty, baseline/rubric/interpretation, owner/remedy/outcome and suppressed/unobserved scope; no completeness/legal pass inferred |
| AOS-13-CON-007 Outcome/memory/change | Execution/humans/domain stewards →13/02/21/25/30: actual consequences, approved human rationale, definition history/lesson/proposal, change impacts/applied acknowledgements and residual duties; governed lifecycle; no self-amendment |
| AOS-13-CON-008 Own research | Assigned specialist/14/13 →02/30/01/affected owners: common RSVIEW-0.1 profile/run/finding/disposition plus exact process implications; actual coverage/reviewer duties/change standing explicit |

Every exchange identifies stable entity/object/revision IDs, organisation/actor/role/purpose/audience, exact common view/profile, source assurance, event/admission/effective time and actual status. Units and comparison precision are explicit. Missing/invalid/unsupported fields remain rejected/unresolved, not guessed favourable values. Ordering applies only within declared scopes; no global total order or atomic external effects presumed. Duplicates do not create independent evidence or repeatable permission. Receipt, validation, actual application, human responsibility and actual effect stay distinct; information-only exchanges require only their declared stages, no invented human acknowledgement for every record and no recursive acknowledgement loop.

Revocation/correction identifies dependent pending work; consequential retry reconciles effects/current checks. Exact field types, enumerations/cardinalities, source/case-master mappings, time/freshness, duplicate keys/retry/fencing/service limits and transport remain approved executable gates, not local replacements for shared semantics.

### 6.1 Supplier integration ownership

Each arrangement declares authoritative definition/source/case master and which product/role enforces each control and maintains each mapping. Agree exact API/view/profile versions, identity/time/units, read/write/command rights, authentication/transport/ordering/acknowledgement, duplicate/retry/revocation/effect-reconciliation, availability/capacity/human cover and lifecycle/provider/exit arrangements before dependent build/activation. Product-internal exchange does not remove observable permission/acceptance/effect evidence. 13 coordinates final gate checks; 05 enforces them. An implementation must not substitute local state for authoritative shared accounts or permissions.

## 7. Authority and decision boundaries

Technical readiness is not organisational permission. Each step needs exact current authority/use and applied runtime/control evidence. 04 supplies bounded task/effect semantics; 05 enforces final checks and cumulative capacity. 13 schedules/coordinates under those constraints; it cannot grant, raise a budget or release a brake merely to clear its queue.

Mode1 routing/order/defined comparisons can be automated within approved instruments. Human Mode2, value trade-offs, welfare/consent conflicts, substantive employment decisions, repair promise/scope/disputed closure and other reserved decisions remain human. 22 prepares canonical cross-domain interpretation; 30 supports empowered humans. Technical multi-agent coordination cannot silently determine moral priority. 04 task delegation still applies to every child/context; parent approval is not an unbounded grant.

Stop or cancellation affects its exact automation scope, not all human/legal/service duties. Compensation and resumption have independent authority/use checks. Explain constraint meaning, basis and route by default under DEC-027; reviewed necessary privacy/security/feasibility restriction limits disclosure, not enforcement. Protected audience/continuing duties remain independently permitted under KPR. No new emergency powers, inference or boardroom observation is granted.

## 8. Reasoning principles applied

FP1 ties workflow to purpose; FP2 reserves incommensurable judgement; FP3 requires independent enforced controls; FP4 makes actual steps/reasons legible; FP5/6 require uncertainty/edge/failure paths; FP7 protects credible service and challenge; FP8 retains human constitutional authority; FP9 separates purpose-led design from legal validation; FP10 requires cumulative/concurrent/cross-domain assessment. Technical contributions do not establish whole-principle/institutional passes.

| RP v6 domain / thematic locator | Application / cases |
| --- | --- |
| 1 Architecture/closed feedback/named human layers | VER-011/012/020/025–029; tracker until actual accepted duty/outcome |
| 2 Modes/permanently human/protected space | VER-008/017/028/029; coordination cannot make moral/employment/board decisions |
| 3 1+5/intrinsic risk/safety/Golden Thread | VER-007/013/022–028; source-domain safety and human routes retained |
| 4 Options/actual state/consequence feedback | VER-015/016/020/021/026; attempt, proposal and actual effects distinct |
| 5 Blind spots/perimeter/coherence paradox | VER-004/006/034/040; quiet monitoring and non-modelled cases explicit |
| 6 Ethics/telos/no-exit/purpose drift | VER-013/014/027/028/030; continued service/protected duty and human review |
| 7 Radical transparency/uncertainty | VER-003/005/007/035; source, time, definition, reasons and limits reconstructable |
| 8 Explicit/contextual delegation/required audience | VER-008–014/017/038; exact current powers and protected accepted handoff |
| 9 Sensing/source-purpose boundaries | VER-006/028/030–032; operational data not private profiling or individual surveillance |

Appendix A allocates all 29 GT tests. Material conflicts remain evidenced and referred; no institution-wide favourable result is inferred from smooth process execution.

## 9. Data, privacy and disclosure

Workflow correlation creates new access/inference opportunities, but no new rights. Maintain 03 source-purpose and audience restrictions at each intake, processing, tool and disclosure boundary. Use permitted projections, not full resident private conversations or general sensitive-worker records. Derived dashboards/memory inherit restrictions and lifecycle; role-appropriate views disclose necessary limits without exposing protected substance.

Operational timing/workload/error evidence must not drift into individual emotional/vulnerability/productivity surveillance. Human-provided/confirmed context follows DEC-088, not inference from silence/activity. A resident's channel agreement and selected sharing remain distinct from organisation permission. Worker/refusal/rights/protected-source boundaries from 12 persist in coordinated cases. Aggregate/process insight cannot excuse unlawful source processing.

Govern retention/correction/restriction/deletion across source logs, derived views, indices, exports/backups/restoration. Minimal permitted disposition evidence is not a licence for hidden sensitive payload. Required protected reporting uses its independently verified minimal route; diagnostics cannot bypass it. Private chain-of-thought is not required. Genuine professional/human challenge can proceed even when automated evidence is absent.

## 10. Behaviour and workflows

### 10.1 General authorised workflow

Trigger →admit exact scoped evidence →bind applicable definition/profile/instance →assess readiness and uncertainty →perform exact current controls →coordinate permitted step →observe actual effect →obtain required recipient/human acceptance →track residual duties →apply actual outcome/closure rule →feedback/owned lesson. A ready queue item with unavailable permission remains held, with continuing permitted human/service route. A terminal worker result is only technical evidence for its defined scope.

### 10.2 Selected overdue-repair demonstration

Use synthetic repair R, original resident-communicated commitment P, promised scope S, named owner O and accountable repairs team T.10/02 supply authoritative promise/precision/timezone, revision/communication evidence, repair-specific completion rule and work/inspection/dispute evidence. 13 owns comparison and accepted-duty tracking; 30 supports actual human ownership; 11 owns current agreed-channel resident delivery. B denotes the approved comparison boundary, not a new grace period. Date-only commitments become past due only when the promised date has ended in the approved organisation timezone; exact-time commitments retain their precision.

| Evidence/time condition |13 classification and permitted next step |
| --- | --- |
| Promise missing/contradictory | Owned promise-evidence exception; no invented date or definite lateness |
| Before or at B with no established breach | No overdue-incomplete classification; ordinary permitted repair tracking continues |
| After B, evidenced outstanding promised work | Overdue-incomplete; approved human escalation/cover and 11 communication duty |
| After B, completion cannot be established | **Completion unverified after promised date**; owned verification escalation under DEC-039, not definite incomplete/complete |
| Acceptable on-time completion evidence | No overdue-repair alert from that comparison; actual outcome retained |
| Acceptable completion after B | Work now completed within evidenced scope; original lateness/breach and residual escalation duties retained |
| Partial scope or disputed closure | Preserve completed/outstanding/disputed evidence; apply incomplete rule where established, otherwise verify; human dispute/scope route, no silent closure |

OriginalP/internal target/revised P2 are separate. Only authorised human revision plus resident communication gives P2 commitment standing; original/breach retained. A split/scope change cannot erase promised work. New promise does not automatically close escalation. Contractor flag alone and resident silence cannot establish completion.

13 maintains tracker until empowered human accepts exact duty; 30 supplies actual named-owner/team cover. 11 provides both current contacts through agreed authorised channels; failed/unknown delivery and missing owner stay owned. Sending details, accepting responsibility and completing the repair are separate. Approved retries reconcile effects and current channel/use; no unilateral alternate contact. Closure needs repair-specific actual evidence, human disposition and explicit residual duty/challenge standing. Actual condition/work outcome returns to 10 and permitted 11/30/25 review.

### 10.3 Other service, people and governance work

11 request/complaint input →13 distinct linked service/response/remedy duties →accepted human owner/cover →permitted communication →actual remedy/outcome. Complaint response does not end outstanding repair. 12 people/rights/protected concern →exact permitted evidence →independent empowered human review →actual reasoning/action/outcome; no automated personnel judgement. GI/research findings →separate component reviewer duties →canonical/human disposition →01 amendment and applied activation where needed; shared retrieval/delivery not all-duty completion.

### 10.4 Change, partial effect and recovery

Changed definition/evidence/permission →material impact/current sources →affected pending step held/reassessed →required acknowledgements of actual application/no dependency/unresolved →only compatible scope continues. Late events never revive old permission. Partial/unknown effect →observe target/ledger under permitted scope →authorised reconciliation →fresh check for retry or separately authorised compensation →actual residual duty/outcome. Restore isolated state under 05/KPR, establish authoritative currentness/completeness, apply restrictions/lifecycle and reconcile effects/accounts before authorised scoped continuation. No claimed atomic external transaction or global exactly-once guarantee.

## 11. Failure, escalation and recovery

Missing/conflicting evidence withholds dependent favourable claims/effects and creates an owned source/service exception. Lost event/clock/feed/broker/model exposes affected coverage; approved manual service/tracking continues. Human absence/rejection uses approved cover and explicit duty tracking; no acceptance from timeout. If normal and protected reporting paths fail, retain owned unresolved duty and approved human fallback without expanding disclosure.

Unknown outcome is not confirmed failure or safe repetition. Reconcile actual external effects/reservations before retry; each attempt/compensation/resumption has current exact checks. Cancelled technical work retains separately authorised service duties and historic effects. An exceptional novel case is divergence, not nearest-template success.

Recovery requires isolated candidate state, current 01/03/04/05/02 evidence, restrictions/deletions and known/unknown effects reconciled, then scoped release. Protected backups may still be stale/incomplete. Continuation cannot revive revoked permissions or erase a failed process/compliance/service duty. Compliance-critical failures need owned cause/related-instance review and actual remedy; restoring a service alone does not establish root-cause resolution.

## 12. Evidence, provenance and audit

Consequential records link trigger, source/assurance/scope, definition/profile/instance/request/attempt, actor/current authority/use/applied configuration/reservation/checkpoint, applied rule/model output, human assessment, observed prevented/partial/actual effect, intervention, accepted duty and outcome/residual. Include event/admission/effective time, units, uncertainty, coverage, source correction and lifecycle/audience references.

02 owns custody; process steward definition/instance meaning; 04/05 task/control/effect/account evidence; domains source meaning; 30 human decision support. Original evaluation and later enforcement are distinct. Generated explanations cannot prove prior checks or human judgement. Capture applied rules/output/approved human rationale, not private chain-of-thought. Operational memory retains permitted rationale and actual context without hindsight rewriting. Independent 40/25/human review treats 13 as both an evidence producer and an assurance subject.

## 13. Security and operational requirements

05 owns independent runtime/final effects/accounting. 13 adds demonstrable case/attempt correlation, task/destination isolation, current-definition application, stale/coordinator concurrency handling, owned queues/cover, permitted event/replay processing and manual continuity. Hostile source/tool/model instructions cannot create tasks/tools/rights beyond approved scope. Source compromise/quarantine preserves visible coverage and approved human duties.

Owners commission exact clocks/precision, currentness/fencing, queue/deadline/cover/capacity, reservation units/groups, ordering/duplicate/retry/reconciliation, availability/recovery/lifecycle and analytical evaluation profiles. No default response time, grace, pass percentage, capacity or transport is invented. Deterministic comparison/enforcement is assessed separately from probabilistic pattern/routing interpretation. Approved task/population/error rubric covers false/missed divergences, novel cases, coverage, fidelity, bias/unequal service effects and provider changes. Critical control failures cannot average away. Concurrent/cumulative and longitudinal effects require evidence beyond a single smooth run.

## 14. Invariants

| INV | Invariant / REQ / VER |
| --- | --- |
| AOS-13-INV-001 | Coordination creates no powers; 011/012/024 →008/017 |
| AOS-13-INV-002 | Delivery is not accepted human responsibility; 016–018 →011/012 |
| AOS-13-INV-003 | Unknown effect is not permission to retry; 021–023 →015/016 |
| AOS-13-INV-004 | Cumulative bounds cannot be evaded by splitting/concurrency; 013/025 →009/018 |
| AOS-13-INV-005 | Unknown completion after B remains unverified; 032/033/035 →023/024 |
| AOS-13-INV-006 | Terminal automation is not completed service; 026/027/038/039 →019/020/026/027 |
| AOS-13-INV-007 | Process optimisation/research cannot self-amend; 029/054 →021/038 |
| AOS-13-INV-008 | Quiet monitoring/technical success is not complete independent assurance; 005/010/056/057 →004/007/040 |

## 15. Conformance and acceptance

All claims are **unsubstantiated planned claims**. None of the cases is executed. Later records identify exact versions/fixtures, date/environment, method, assessor, observed evidence/limits and findings/accepted owner/remedy/retest. Blocked/not-performed/inconclusive differ from failed/passed. Document walkthrough establishes logic review only, not implementation enforcement or actual institutional judgement.

| CR | Bounded proposed claim | REQ / cases |
| --- | --- | --- |
| AOS-13-CR-001 | Definition/evidence/bounded monitoring |001–010; VER-001–007 |
| AOS-13-CR-002 | Current controls/change/accounting |011–015; VER-008–010 |
| AOS-13-CR-003 | Accepted protected handoffs/continuing duties |016–020; VER-011–014 |
| AOS-13-CR-004 | Reconciled coordination/effects/closure/memory |021–029; VER-015–021 |
| AOS-13-CR-005 | Domain service/human integration |030–042; VER-022–030 |
| AOS-13-CR-006 | Secure recoverable evidence/independent assurance |043–049/056–057; VER-031–035/040 |
| AOS-13-CR-007 | Own research |050–054; VER-036–038 |
| AOS-13-CR-008 | Supplier realisation |055; VER-039 and declared functional cases |

Common prerequisites: fixed exact source/component/common manifest; approved isolated synthetic fixtures/destinations or explicitly labelled walkthrough; competent assessors; approved role/authority/use/applied-definition/channel/handoff/continuity/time/account profiles and expected-result rubric where relevant. Missing prerequisites mean blocked/not-performed. Methods combine component/integration boundary tests with competent human review. Evidence includes fixture truth/expected outputs, actual ordered inputs/checks/outputs/effects, versions, human scoring/rationale, coverage and findings/remedy/retest. Actual control/duplicate/prevention observations are required for enforcement claims; model refusal and dashboard colour do not prove enforcement.

### AOS-13-VER-001 — Process definition and ownership

**Requirements:** AOS-13-REQ-001. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Versioned synthetic process, permitted steps/roles/outcomes and missing human boundary or governing rationale.

**Procedure:** Inspect definition fields, owners and sources; attempt activation with an unspecified material rule.

**Expected result:** Missing consequential semantics are owned build gaps; no interpretation by guesswork.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Process/authority human assessors; CON-001.

### AOS-13-VER-002 — Applied activation

**Requirements:** AOS-13-REQ-002. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Approved new definition with one incompatible/unapplied dependency and separately valid unaffected function.

**Procedure:** Collect actual application acknowledgements; attempt dependent execution and then authorised compatible activation.

**Expected result:** Affected function held until compatible applied evidence; unaffected valid scope can continue; approval/receipt not application.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Control/platform/process assessors; CON-001/004.

### AOS-13-VER-003 — Instance and evidence identity

**Requirements:** AOS-13-REQ-003, AOS-13-REQ-004. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Duplicate/reordered source events, two organisations, revised process and uncertain domain evidence.

**Procedure:** Admit and correlate instances; round-trip exact source/definition standing; try latest-arrival truth/permission.

**Expected result:** Stable identity/revisions/uncertainty preserved; no cross-organisation scope or silent source reinterpretation.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Data/domain/process assessors; CON-002.

### AOS-13-VER-004 — Monitoring coverage

**Requirements:** AOS-13-REQ-005. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Observed/omitted transaction populations, stale/missing feeds and a quiet monitoring period.

**Procedure:** Compute declared coverage; display gaps; attempt full-population assurance from absent alerts.

**Expected result:** Scope/time/event loss explicit; quiet feed not complete monitoring or safety.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Operations/assurance assessors; CON-006.

### AOS-13-VER-005 — Divergence dashboard

**Requirements:** AOS-13-REQ-006, AOS-13-REQ-007. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Actual versus intended step/time/outcome, conflicted evidence and role-limited audiences.

**Procedure:** Detect/display transaction exception with source/definition/owner; attempt a smoothed favourable aggregate hiding it.

**Expected result:** Material divergence visible to permitted responsible role with uncertainty/standing; no suppressed exception from aggregation.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Process/service/privacy assessors; CON-006.

### AOS-13-VER-006 — Pattern and comparison

**Requirements:** AOS-13-REQ-008. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Permitted process population, changing baseline, subgroup gaps and uncertain correlations.

**Procedure:** Produce findings; vary assumptions; request causal blame or certainty beyond evidence.

**Expected result:** Pattern/observation distinct; population/baseline/coverage/limits explicit; no individual surveillance inference.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Process/model/privacy assessors; CON-006.

### AOS-13-VER-007 — Obligation timing and claims

**Requirements:** AOS-13-REQ-009, AOS-13-REQ-010. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Human-approved statutory/contractual/internal timing profiles, changed applicability and unverified completion.

**Procedure:** Evaluate each distinct profile; seed an overdue obligation and future/draft source; attempt compliance certification from workflow success.

**Expected result:** Timing/standing not conflated; breach/uncertainty referred under exact profile; no grace or legal pass invented.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Competent obligation/legal/service assessors; CON-001/006.

### AOS-13-VER-008 — Exact effect and delegation

**Requirements:** AOS-13-REQ-011, AOS-13-REQ-012. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Approved parent workflow, changed step arguments/recipient, revoked child permission and valid exact-operation control receipt.

**Procedure:** Attempt each effect at actual final gate; inspect current 01/03/04/05 checks and actor/task scope.

**Expected result:** Parent approval does not grant changed/child powers; denied/unresolved effects prevented; each actual attempt checked.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Authority/use/runtime assessors; CON-004.

### AOS-13-VER-009 — Shared cumulative accounting

**Requirements:** AOS-13-REQ-013. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Parallel tasks, split requests/retries/provider changes and authoritative 05 account/reservations.

**Procedure:** Reserve/consume/reconcile common scope; try independent counters and duplicate capacity consumption.

**Expected result:** No budget evasion or double consumption; shared current account/effect evidence authoritative; values from approved profile.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Runtime/agent/process assessors; CON-004.

### AOS-13-VER-010 — Change and event ordering

**Requirements:** AOS-13-REQ-014, AOS-13-REQ-015. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Permission/channel/definition/evidence change during pending work, late duplicate event and no-material-dependency branch.

**Procedure:** Identify impacts/owners; request application acknowledgements; attempt obsolete-effect execution and old-permission revival.

**Expected result:** Affected work reassessed/held as required; actual applied/unresolved/no-dependency standing distinct; valid unrelated work not blanket frozen.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Control/data/process assessors; CON-002/004.

### AOS-13-VER-011 — Tracker and acceptance

**Requirements:** AOS-13-REQ-016, AOS-13-REQ-017. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Duty-bearing handoff, receipt/validation/application messages and empowered human accepting only part of scope.

**Procedure:** Record stages, attempt tracker relinquishment at delivery, capture exact human acceptance and residual duty.

**Expected result:** Tracker persists until accepted defined responsibility; partial residual owned; stage does not imply later stage.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Workflow/human-service assessors; CON-003; KX-21/26.

### AOS-13-VER-012 — Rejection, absence and cover

**Requirements:** AOS-13-REQ-018. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Unresponsive/rejecting/unavailable primary human, approved team cover and failed cover route.

**Procedure:** Expire approved response window, route cover/escalation, separate accepted and unaccepted duty.

**Expected result:** No silent handoff success; current tracker/cover/residual owner and evidence remain explicit.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Human-workflow/service assessors; CON-003.

### AOS-13-VER-013 — Protected finding

**Requirements:** AOS-13-REQ-019. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Suppression instruction, implicated recipient and simultaneous ordinary/protected route failure.

**Procedure:** Use independently permitted minimal protected route; track actual delivery/acceptance and last approved human fallback.

**Expected result:** Required audience duty cannot quietly disappear; no broader disclosure power; compound failure remains owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Protected-reporting/privacy assessors; CON-003; 40 VER-021.

### AOS-13-VER-014 — Withheld work and continuing service

**Requirements:** AOS-13-REQ-020. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Denied/unavailable authority or capacity, required resident update and forbidden sensitive explanation.

**Procedure:** Hold dependent effect, produce permitted reason/review route, continue separately authorised service/reporting duty.

**Expected result:** Enforcement not waived; blocker understandable within restrictions; stop automation not stop all human service.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Control/privacy/service assessors; CON-003/004.

### AOS-13-VER-015 — Unknown effect and retry

**Requirements:** AOS-13-REQ-021, AOS-13-REQ-022. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus External step applied with lost response, partially applied step and confirmed-not-applied variant.

**Procedure:** Reconcile observed target/effect before retry; preserve request and new attempt identity; recheck current permissions.

**Expected result:** Unknown not automatically failed/safe-to-repeat; no duplicated consequence; attempt history and fresh checks retained.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Execution/exchange/process assessors; CON-004; 40 VER-023.

### AOS-13-VER-016 — Compensating action

**Requirements:** AOS-13-REQ-023. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Original actual effect, proposed reversal, revoked reversal rights and irreversible residual consequence.

**Procedure:** Seek independent authority/use for compensation; execute only permitted variant; inspect original/history/residual duty.

**Expected result:** Compensation does not erase original or create rollback permission; irreversible effects and outstanding duties remain explicit.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Authority/execution/human assessors; CON-004/007.

### AOS-13-VER-017 — Technical coordination and moral boundary

**Requirements:** AOS-13-REQ-024. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Several bounded agents/dependencies, conflicting task results and incommensurable human priorities.

**Procedure:** Coordinate permitted work/joins, inspect each delegated scope, refer conflict rather than resolve by technical score.

**Expected result:** Technical ordering not moral authority; missing/contradictory results visible; source purposes/Mode2 boundaries retained.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Agent/process/governance assessors; CON-002/004.

### AOS-13-VER-018 — Concurrent/stale workers

**Requirements:** AOS-13-REQ-025. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Two workers racing an effect, stale lease/state and shared reservation/current-check evidence.

**Procedure:** Inject concurrent dispatch/recovery, reconcile already attempted effects and enforce accepted runtime ownership/fencing profile.

**Expected result:** No duplicate consequence or split accounting; stale coordinator cannot grant effects; no universal exactly-once claim inferred.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Platform/execution/process assessors; CON-004.

### AOS-13-VER-019 — Hold, cancel and residual duties

**Requirements:** AOS-13-REQ-026. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Pending multi-step case with completed/unknown effects and continuing service obligations.

**Procedure:** Hold/cancel automation under authority, reconcile completed effects, retain human duties and attempt blind resumption.

**Expected result:** Automation terminal/held state not service closure; exact residual owners/effects visible; resumption separately checked.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Control/human-service assessors; CON-002/003/004.

### AOS-13-VER-020 — Outcome-based closure

**Requirements:** AOS-13-REQ-027. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Technical success, actual service outcome, unresolved dispute/handoff and authorised negative disposition.

**Procedure:** Apply exact closure rule; attempt closing on last task/message; record actual human disposition/outcome and residual obligations.

**Expected result:** Only defined evidence/disposition supports closure; failure/cancellation can end technical path while service duty remains.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Service/process/human assessors; CON-002/007.

### AOS-13-VER-021 — Operational memory and improvement

**Requirements:** AOS-13-REQ-028, AOS-13-REQ-029. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Old/current definition rationale, outcome/near miss, permitted lesson and proposed automatic parameter optimisation.

**Procedure:** Trace historical decision basis/effect; prepare improvement; attempt deploying it without amendment/applied activation.

**Expected result:** History/rationale retained under lifecycle; pattern is proposal not authority; hindsight not rewritten as prior reasoning.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Process/knowledge/authority assessors; CON-007.

### AOS-13-VER-022 — Repair promise boundary and incomplete work

**Requirements:** AOS-13-REQ-030, AOS-13-REQ-031. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Communicated promise P/internal T, approved date-only timezone or exact time, before/at/after boundary B and evidenced outstanding work.

**Procedure:** Apply approved comparison; reject internal target substitution/grace; send permitted overdue route only after boundary.

**Expected result:** No overdue-incomplete at/before B; after B evidenced incomplete routes to human; correct source/time meaning retained.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Repairs/time-profile/process assessors; CON-005; 10 VER-010/011/015.

### AOS-13-VER-023 — Repair unknown/date exceptions

**Requirements:** AOS-13-REQ-032, AOS-13-REQ-033. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus t>B with no acceptable completion evidence, separate missing/conflicting promise and established on-time/late completion.

**Procedure:** Classify each variant; route verification/date evidence exception; preserve history when late completion later arrives.

**Expected result:** Unknown is completion unverified after promised date; missing promise not fabricated lateness; on-time not overdue; late completion preserves breach without asserting work still incomplete.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Repairs/data/process assessors; CON-005; 10 VER-013/014; 40 VER-008.

### AOS-13-VER-024 — Repair revision, partial scope and dispute

**Requirements:** AOS-13-REQ-034, AOS-13-REQ-035. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Authorised communicated P2 versus internal reschedule, partial task scope, contractor closed flag, silence and contested completion.

**Procedure:** Preserve original/breach; require human/communication for revision/scope changes; route disputed/unverified evidence without auto-closure.

**Expected result:** New promise cannot erase escalation/history; partial scope remains incomplete; contractor flag/silence alone not completion.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Repairs/human/resident assessors; CON-005; 10 VER-012/013/015/016; 11 VER-013.

### AOS-13-VER-025 — Repair ownership and both contacts

**Requirements:** AOS-13-REQ-036, AOS-13-REQ-037. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Named owner O, accountable team T, current verified contacts/agreed channel, owner absence and failed resident delivery.

**Procedure:** Obtain 30 exact accepted duty/cover; coordinate 11 both contacts through checked channel; retain duplicate/failure/unaccepted exceptions.

**Expected result:** Both actual contacts delivered when available; missing owner not fabricated; cover/unresolved duty remain tracked; delivery not human acceptance or completed repair.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Repairs/resident/human-workflow assessors; CON-003/005; 11 VER-010–012; 40 VER-007/009.

### AOS-13-VER-026 — Repair closure and feedback

**Requirements:** AOS-13-REQ-038. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Actual work/inspection completion evidence, human disposition, delivered contacts, residual dispute and callback/new concern.

**Procedure:** Apply repair-specific rule, close only authorised evidenced scope, retain breach/residual duties and return actual consequence to 10/11/30.

**Expected result:** Actual outcome and communication separate; disputed/residual work not silently lost; callback handled as linked evidence/new duty as appropriate.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Repairs/service/process assessors; CON-005/007; 10 VER-018; 40 VER-010.

### AOS-13-VER-027 — Complaint and outstanding service

**Requirements:** AOS-13-REQ-039. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Service request with complaint, human complaint response/remedy offer and outstanding repair/remedy tasks.

**Procedure:** Track linked duties and permitted 11 response, continue service action and inspect closure attempt on response alone.

**Expected result:** No duplicate complaint barrier or stopped repair; response/remedy offer not actual remedy; remaining duties/owners visible.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Complaint/resident/workflow assessors; CON-003/005; 11 VER-014/015.

### AOS-13-VER-028 — People and rights routes

**Requirements:** AOS-13-REQ-040. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus 12 capability/rights/protected concern with permitted evidence, implicated normal reviewer and proposed automatic personnel action.

**Procedure:** Coordinate independent accepted human review, preserve 12 scope/standing and compare proposal versus actual human decision.

**Expected result:** No automated employment judgement or sensitive-data expansion; accepted independent human duty/outcome reconstructable.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; People/privacy/human-workflow assessors; CON-003; 12 VER-004/005/020/022.

### AOS-13-VER-029 — Governance and shared research duties

**Requirements:** AOS-13-REQ-041. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus One finding relevant to several components, separate specialist reviewers and pending human amendment.

**Procedure:** Track per-component duties/acceptance, canonical analysis/decision links and independent correction/amendment status.

**Expected result:** Shared collection/delivery not completion of every review; approval/board decision/application and research disposition remain distinct.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Research/GI/human assessors; CON-003/007/008.

### AOS-13-VER-030 — Cross-domain privacy

**Requirements:** AOS-13-REQ-042. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Unshared resident chat, sensitive workforce record, ordinary case data and proposed join/individual inference.

**Procedure:** Route only exact permitted projections; attempt coordination-based rights inheritance and privacy override.

**Expected result:** Private/sensitive/inference barriers enforced; workflow orchestration not blanket access; minimal protected evidence preserved.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Privacy/security/domain assessors; all CON.

### AOS-13-VER-031 — Record correction and lifecycle

**Requirements:** AOS-13-REQ-043. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Corrected source, permission change, derived dashboard/history, deleted content and restored copy.

**Procedure:** Map material dependencies, apply selective restriction/correction/deletion and preserve actual effect/disposition standing.

**Expected result:** No hidden deleted payload, blanket freeze or rewritten past consequence; current restriction survives derived/restored state.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Data/privacy/process assessors; CON-002/006/007.

### AOS-13-VER-032 — Hostile instructions and isolation

**Requirements:** AOS-13-REQ-044. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Injected event/tool/model instruction, changed destination and two organisation/task scopes.

**Procedure:** Attempt bypass/tool expansion at actual controls, preserve permitted incident evidence and valid unaffected operation.

**Expected result:** No unauthorised effect/cross-scope leak; source content grants no powers; failure owned without excess sensitive logs.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Security/control/process assessors; all CON.

### AOS-13-VER-033 — Outage and recovery

**Requirements:** AOS-13-REQ-045, AOS-13-REQ-046. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Lost broker/workflow/model/feed, manual case continuity, stale recovered authority/use/configuration and unknown effects/reservations.

**Procedure:** Expose coverage, continue approved human route, restore isolated state, establish authoritative currentness/completeness and reconcile before scoped release.

**Expected result:** No phantom success or revived permission; effects/accounts/duties reconciled; manual continuity retained and restart authorised.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Platform/control/service assessors; CON-002/003/004; 40 VER-022.

### AOS-13-VER-034 — Analytical quality and unequal effects

**Requirements:** AOS-13-REQ-047. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Approved pattern/routing task/population/rubric, critical errors, omitted cases, provider change and distributional service impacts.

**Procedure:** Evaluate representative/adversarial and changed-baseline cases independently of supplier claims; inspect false/missed/biased interpretations.

**Expected result:** Quality evidence bounded; enforcement not rescued by accuracy average; unequal effects/novelty limits exposed and human remedy owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Independent competent model/process/service assessors; CON-006.

### AOS-13-VER-035 — Audit and common compatibility

**Requirements:** AOS-13-REQ-048, AOS-13-REQ-049. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Exact common manifest, unsupported version, deterministic/checkpoint and human action records, retrospective explanation.

**Procedure:** Round-trip views and reconstruct trigger-to-outcome; reject unsupported meaning; compare prior evidence with generated narrative.

**Expected result:** One shared meaning/standing; actual checks/human actions evidenced; no private chain-of-thought or hindsight proof.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Data/audit/process assessors; all CON; 40 VER-025.

### AOS-13-VER-036 — Own research remit/source standing

**Requirements:** AOS-13-REQ-050, AOS-13-REQ-051. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Approved process research profile, shared researcher and relevant workflow/retry development; draft/future/wrong-jurisdiction/stale/conflicting source.

**Procedure:** Retrieve through 14, verify dates/standing, assess exact affected 13 obligations and distinct component impacts.

**Expected result:** Specialist relevance/uncertainty explicit; source verified not automatically adopted; shared collection does not discharge own review.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Process/research/competent source assessors; CON-008.

### AOS-13-VER-037 — Own research coverage/hostile source

**Requirements:** AOS-13-REQ-052. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Partial/denied/failed retrieval, bounded no-finding and instruction to expand tools/change workflow.

**Procedure:** Run variants; assess relevance/fidelity/false-missed rubric; attempt execution of source instructions.

**Expected result:** Actual coverage/gaps retained; no-finding scoped; source text grants no permission or amendment.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Research/security assessors; CON-008.

### AOS-13-VER-038 — Own research reviewer/change

**Requirements:** AOS-13-REQ-053, AOS-13-REQ-054. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Urgent material finding, unavailable reviewer/cover, accepted proposal and unapproved amended process.

**Procedure:** Track receipt versus acceptance/escalation, support separately permitted urgent human response, attempt premature deployment.

**Expected result:** Owned review persists; disposition/amendment/verification/activation separate; no new sensing/calibration/execution from finding.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Research/authority/human-workflow assessors; CON-008.

### AOS-13-VER-039 — Supplier participation

**Requirements:** AOS-13-REQ-055. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Hypothetical case/BPM/workflow, automation, process-mining and integration products in standalone/API/combined configurations.

**Procedure:** Map exact requirements/control/source/case-master ownership; run evidence-to-accepted-human-to-action-to-outcome walkthrough and inspect unsupported fields/hidden handoffs.

**Expected result:** Existing tools may realise several functions; each declared obligation has actual scoped evidence or owned gap; no product certification or implicit authority.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Process/data/privacy/exchange/service assessors; all CON.

### AOS-13-VER-040 — Independent assurance and edge of model

**Requirements:** AOS-13-REQ-056, AOS-13-REQ-057. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Non-modelled novel case, quiet feed, monitoring self-report and independent human oversight/effect evidence.

**Procedure:** Refuse forced template fit, produce owned divergence, compare independent assessment and actual coverage/controls.

**Expected result:** Monitoring system remains assurance subject; gaps/novelty visible; no full-population/independent assurance from self-report.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings, transitions, control/effect observations and accepted human judgement; Independent competent process/governance assessors; CON-006/007; 40 VER-027/028.

## 16. Dependencies

Drafting uses approved directions and logical common/domain meanings. Build requires exact executable process definitions/schemas/source mappings, required acknowledgement/human duties, time/completion/closure/control/account profiles, fixture/rubric, concurrency/effect-reconciliation and enforced boundaries. Activation additionally needs appointed process/service/control/independent human owners, cover/capacity, permitted channels/private/sensitive routes, actual compatibility/evaluation/continuity/recovery evidence and scoped release. Operations require current instruments/application/evidence, accepted duties, outcomes, incident/root-cause review, lifecycle and governed research.

01–05/02/10–12/14/20–25/30/40 retain authoritative responsibilities. Process engines, transport/schema/model/supplier choices, legal applicability, timers/freshness/retries/fences, limits/grouping, resident agreement/human cover and research/evaluation values are unresolved organisation/build profiles, not invented defaults. HACT preferred-reference status does not automatically define every process event or approve a licence. 10–12 counterpart revisions add logical 13 links; exact endpoints and observed runtime adoption remain gates.

## 17. Issues and controlled unknowns

All are open dependencies with high confidence that the need exists; organisation-specific values/adequacy are unassessed. Recording an issue does not resolve it or authorise execution.

| ISS / type | Description/source/affected capability | Owner / evidence / gate / disposition |
| --- | --- | --- |
| AOS-13-ISS-001 dependency | Exact process/domain/common schemas, IF-001/view/API mappings and supplier/source/case-master ownership; §6/all CAP | Process/data/exchange owners; versioned mappings/round-trip/control evidence before affected build; open |
| AOS-13-ISS-002 dependency | Definition/closure/time/promise/completion/handoff/cover/continuity profiles and actual human capacity; CAP-001/003/005 | Service/process/30/domain owners; approved instruments/fixtures and accepted routes before affected build/activation; open |
| AOS-13-ISS-003 dependency | Current-state/application/impact/concurrency/fencing/reservations/grouping/effect observation/retry/compensation mechanisms; CAP-002/004/006 |01–05/13/platform owners; exact shared profiles and adversarial/concurrent observed evidence before effects; open |
| AOS-13-ISS-004 dependency | Legal/obligation/source applicability and purpose/privacy/lifecycle/protected paths; CAP-001/003/005/006 | Competent legal/service/privacy/protected owners; current-source mapping/permitted routes and actual restrictions before compliance/activation claims; open |
| AOS-13-ISS-005 dependency | Analytical tasks/populations/benchmarks/quality/bias/provider choices and independent/longitudinal assurance; CAP-001/006 | Process/model/40/qualified independent humans; approved rubric and actual scoped outcomes before claims; open |
| AOS-13-ISS-006 dependency | Own research assignment/triggers/coverage/reviewer windows/cover/rubric; CAP-007 | Process/research/14/30 owners; approved common profile and VER-036–038 evidence before research activation; open |
| AOS-13-ISS-007 dependency | Supplier realisation/source sufficiency and actual evidence after current row allocation, Mark review, whole-set reciprocal compatibility and bounded release evidence; CAP-008/all CAP | Mark/source/40/qualified owners; exact response/disposition/manifest/executed scope before readiness; independent project review deferred; open |

No issue permits weakening protected duties, moral/human boundaries or source-purpose restrictions. Unknown exact mechanisms require gap resolution before dependent effects, not plausible build-agent invention.

## 18. Implementation guidance — non-normative

A versioned process graph/state machine can represent definitions/conditions/human steps; an event/case log can preserve source/attempt/outcome links. A durable duty queue can distinguish receipt from empowered acceptance. Workflow/saga patterns may help reconcile multi-step external effects, but compensation is a separately authorised action, not a guaranteed atomic rollback. No framework, broker, engine or transport is selected.

### 18.1 Worked supplier example

An existing repairs case-management platform receives 10's controlled promise/completion evidence through an integration service. It realises 13's comparison/duty lifecycle while the supplier's process analytics exposes observed deviations/coverage. A task runner executes only permitted steps through the shared 04/05 controls; the case platform cannot authorise effects just because it can call an API.

After B, evidenced outstanding work—or a separately classified unknown completion—creates the appropriate human duty. 30 supplies accepted named owner/team cover; an existing resident messaging/app service realises 11's agreed-channel both-contact delivery. Inspection/work later establishes actual 10 outcome; the case platform applies the authorised closure rule and retains any dispute/residual communication/service duty. If a tool applies an effect but its response is lost, the coordinator reconciles actual state before retry rather than creating a second work order or message.

One suite may provide case, analytics, automation and resident interfaces; several suppliers may share the arrangement. Each declares authoritative records, control locations and actual evidence. The example is a candidate mapping, not product selection or certification. Standalone/manual scope is permitted when explicitly declared and cannot claim automated-service conformance.

## 19. Traceability and change

§2 source/approved decision →§4 CAP/FUN/REQ →§5 states/§6 CON →§14 INV →§15 VER →future exact executed evidence. Every REQ has planned VER and each case names its REQs. Existing 13-IF-001 and common semantic owners/statuses retained. DEC-067–072 maps current checks/application/impact/accounting/withholding/release to 011–026 and related cases. ARCH REQ-041–044/VER-019, DEC-036–041 map to 030–039, VER-022–027, CON-003/005, consuming exact 10/11 evidence and 30 human scope. 12 human/rights/protected routes link REQ-040/VER-028. DEC-086 maps 050–054/VER-036–038; Mark supplier direction maps 055/VER-039 and §20.1.

0.1 initial drafting 8 October 2026. Architecture/Map v0.38; 10 v0.3/11 v0.2/12 v0.2 add reciprocal 13 references without changing their REQ/VER wording/IDs. 40 v0.5 adds exact assembled domain/Process links and planned VER-038; no case execution. Common/source/DEC statuses unchanged. Definition improvement requires permitted human amendment, impact review, verification and compatible applied activation; no automatic parameter tuning or deployment.

## 20. Build and operational handover

This handover supplies functional responsibilities, stable sources/requirements/contracts/states/cases and owned prerequisites. It is not an executable API specification or current permission to build/deploy unresolved controls. A selected slice needs exact machine-readable definition/schema/profile/source/control mappings, appointed roles/cover/capacity, fixture/rubric and actual enforcement/handoff/outcome evidence, permitted destinations/data lifecycle, manual continuity/effect reconciliation/recovery and release/rollback/stop authority.

The selected repair demonstration is bounded: 10 promise/completion evidence, 13 comparison/tracking, 30 accepted human owner and 11 agreed-channel contacts. Explicit exclusions may defer other analytics/domain capabilities, but cannot waive core controls, approved promise/unknown-completion rules or continuing safety/service duties. Full functional domain drafts now exist; source allocation, reciprocal commissioned mechanisms/implementation and independent/executed assurance are still separate work.

### 20.1 Supplier response matrix

Complete one row per exact applicable REQ/revision. Record product/service/configuration/version; direct/configured/integrated/outside-scope contribution; met/partial/not-met/not-assessed with actual evidence; common/source/control/case-master owner; gap/dependency/responsible party and remedy/build/activation gate. “Met” requires scoped accepted evidence, not an API or feature name. Outside supplier scope requires another named party or explicit release exclusion without waiving governing duties.

| Requirement group | Supplier contribution | Evidence / remaining integration questions |
| --- | --- | --- |
| Definition/monitoring 001–010 | Case/BPM/model/analytics functions | Exact approved/applied definitions, source/instance/coverage, role-appropriate divergence and bounded obligation claims |
| Shared controls/change 011–015 | Runner/integration/control coordination | Exact final checks, applied state, shared accounts/reservations and impact/current-state evidence |
| Human/protected handoffs 016–020 | Queues/case/human support | Defined tracker/accepted scope, staged acknowledgements, cover/required audience and continuing duties |
| Effects/coordination/closure 021–029 | Orchestration/retry/memory | Partial/unknown effect reconciliation, current retry/compensation, concurrency/holds/actual outcome and human-authorised improvement |
| Repair/domain integration 030–042 | Service/CRM/domain suites | Exact promise/unknown/partial/dispute meaning, accepted owner/both contacts, complaint/People/GI duties and purpose barriers |
| Operation/assurance 043–049/056–057 | Lifecycle/security/recovery/analytics/evidence | Actual restrictions/effects, current recovery, quality/coverage, independent review and novel-case handling |
| Own research 050–054 | Specialist contribution or outside scope | Common run/finding/reviewer/change and actual coverage evidence |
| Supplier allocation 055 | Versioned implementation/responsibility manifest | Requirement-level response/evidence/owned gaps, exact compatibility/exit/change impacts |

Agree exact API/schema/authentication/time/acknowledgement/service/lifecycle detail before dependent build/activation. This matrix supports item 12a supplier alignment and procurement discussions; it makes no purchase, product certification or release approval.

## 21. Review and findings

Author checks cover 21 template sections, 57 proposed requirements/40 planned cases, stable IDs, reciprocal REQ–VER allocation, all 29 GT contributions, supplier mapping/example/response matrix and owned unknowns. No execution, independent assessment or G3/G4. Specification-quality conclusion: structured functional draft with controlled prerequisites. Design-adequacy conclusion: author review finds scope consistent with source-domain evidence, current shared controls, explicit accepted duty, human judgement and actual outcomes; Mark's review and commissioned/executed evidence remain outstanding.

Next: apply supplier consideration to AOS-14's next revision and perform an author five-domain/common-contract consistency and source-allocation review. This is separate from deferred independent project review. Item 9 operating adoption, item 8 remaining annex/execution coverage, pilot 5b and item 6 implementation/commissioning remain open. No whole-suite build readiness is inferred from all five domain drafts existing.

## Component summary

AOS-13 coordinates authorised work and tracks what actually happened. It preserves source meaning, obtains current shared checks, retains duty until accepted human responsibility, and distinguishes technical status from service outcome. Retries/changes/recovery do not create powers or erase effects. Existing supplier tools may realise these functions while common controls and humans retain their authoritative roles.

## Appendix A — All 29 Governance Intelligence Tests

All institutional statuses are **not assessed**. The board with competent human assessment owns institutional conclusions; Process/service stewards own only evidence contributions. Protected deliberation remains unobserved by AI; missing evidence is a gap, not a favourable answer.

| Test / controlled title | Process contribution / planned cases | Human/cross-domain assessment boundary |
| --- | --- | --- |
| M1.1 Strategic Coherence | Purpose/actual consequences; 001/020/040 | Board strategy-purpose coherence |
| M1.2 Sensing Architecture | Population/coverage/perimeter; 003/004/006 | Whole-domain sensing completeness |
| M1.3 Risk Intelligence | Obligation/divergence/accepted route; 007/011–014 | Board foresight and cross-domain risk |
| M1.4 Composition and Capability | Human acceptance/role dependencies; 011/012/028 | Actual board capability/composition |
| M1.5 Performance Legibility | Actual versus intended/outcome; 005/020/026 | Whole operating/financial futures |
| M1.6 Compliance Assurance | Obligation/source/claim distinction; 007/040 | Competent legal mapping and actual statutory fulfilment |
| M1.7 Governance Documentation | Versioned definition/rationale/history; 001/021/035 | Instrument accuracy and policy/practice coherence |
| M1.8 Accountability Architecture | Tracker/cover/contact/challenge; 011/012/025–028 | Actual response/influence beyond delivery |
| M1.9 Value for Money | Actual constraints/capacity/alternatives; 009/017 | Human value objectives/moral trade-offs |
| M1.10 Human-AI Interaction Norms | Exact delegation/human roles; 008/017/028 | Actual practice under pressure |
| M1.11 Learning Metabolism | Outcome/near-miss/memory; 020/021/026 | Actual learning rather than automatic optimisation |
| M1.12 Continuous Self-Assessment | Coverage/independent/research; 004/036–040 | Board development/culture/effectiveness |
| M1.13 Emergent System Behaviour | Concurrency/partial/cumulative effects; 009/015/018/033 | Whole-system emergence and human response |
| M1.14 Golden Thread Integrity | Source-domain safety/actual work; 022–026 | 10 building information/statutory dutyholders and board accountability |
| M2.1 Values Architecture | Purpose/protected/continuity controls; 008/013/014/030 | Actual structural values |
| M2.2 Coherence Under Pressure | Suppressed concern/edge case; 013/014/040 | Human difficult choices/reasons |
| M2.3 Incommensurable Trade-off Capacity | Technical ordering preserves human priority; 017/028 | Human adjudication/dissent |
| M2.4 Epistemic Brake Function | Missing/novel/unknown evidence; 004/007/015/040 | Human investigation and unease |
| M2.5 Directorial Independence | Independent required audience; 013/029/040 | Actual directorial independence |
| M2.6 Social Legitimacy | Resident challenge/actual remedy; 025–027 | Actual legitimacy and resident influence |
| M2.7 No-Exit Obligation | Continuing service/private/worker scope; 014/027/028/030 | Lived access/burden and responsive design |
| M2.8 Radical Transparency | Actual source/check/effect/reasons; 003/005/035 | Affected people can interrogate reasons |
| M2.9 Moral Drift Detection | Cumulative/divergence/learning; 009/021/034/040 | 25/30 founding-purpose drift comparison |
| M2.10 Purpose Stability | Purpose/current permission/change; 001/008/010/038 | Board purpose-consistent choices |
| M2.11 Murmuration Capacity | Permitted independent human inputs; 013/017/029 | Collective human sense-making; no board capture |
| M2.12 Constitutional Authority | No powers from workflow; 008/017/038 | Board constitutional mediation |
| M2.13 AI Constitutional Framework Governance | Model/runtime/quality/change; 008/032/034 | Board framework evaluation and 25 monitoring |
| M2.14 Purpose-Led Design | Source/purpose/supplier derivation; 001/039 | Human purpose-led design account |
| M2.15 Telos / Function Distinction | Efficient process versus actual purpose outcome; 020/026/040 | Alignment throughactual human governance |

## Appendix B — Supplier requirement response form

Use one row per exact requirement. For each product/version and configuration, declare direct, configured, integrated or outside-scope contribution. Replace the initial status only when scoped evidence supports the claim. Identify actual evidence, missing integration, responsible party and the build/activation gate; a feature name is insufficient. Any excluded duty needs a named counterpart or authorised release exclusion.

| Exact requirement / function | Product/version and contribution | Conformance status | Evidence / gap / responsible party / gate |
| --- | --- | --- | --- |
| `AOS-13-REQ-001` — Definition | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-002` — Activation | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-003` — Instance | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-004` — Evidence admission | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-005` — Coverage | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-006` — Divergence | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-007` — Dashboard | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-008` — Pattern | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-009` — Obligations | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-010` — No compliance certificate | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-011` — Current effects | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-012` — No delegated expansion | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-013` — Reservations | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-014` — Change impact | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-015` — Revocation | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-016` — Tracking owner | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-017` — Acknowledgement | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-018` — Rejection and cover | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-019` — Protected duties | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-020` — Blocker explanation | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-021` — Unknown effect | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-022` — Retry identity | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-023` — Compensation | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-024` — Multi-agent coordination | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-025` — Concurrency | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-026` — Cancellation and holds | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-027` — Closure | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-028` — Operational memory | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-029` — No automatic optimisation | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-030` — Promise comparison | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-031` — Verified incomplete | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-032` — Unverified completion | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-033` — Promise exception | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-034` — Promise changes | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-035` — Repair scope and dispute | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-036` — Repair human ownership | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-037` — Resident contacts | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-038` — Repair outcome | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-039` — Complaint and service | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-040` — People handoff | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-041` — Governance/research handoff | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-042` — Cross-domain boundaries | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-043` — Correction and lifecycle | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-044` — Security | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-045` — Continuity | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-046` — Recovery | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-047` — Evaluation | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-048` — Audit | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-049` — Compatibility | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-050` — Research profile | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-051` — Research finding | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-052` — Research coverage | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-053` — Research human review | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-054` — Research amendment | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-055` — Supplier realisation | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-056` — Independent assurance | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |
| `AOS-13-REQ-057` — No forced fit | Supplier to complete | Not assessed | Supplier and AOS owner to complete before dependent build/activation |



## Current reciprocal adoption and precise source allocation — 9 October2026

This revision corrects current control/status and adoption/traceability references only. Every original normative requirement statement, case acceptance condition, invariant and identity retains its prior meaning. Existing source versions, approved architectural directions and human/private boundaries are unchanged. Local§6 is the authoritative domain view; Registerv0.17 SENSING-ADOPTION-2026-10-09 supplies the current reciprocal common mapping; Matrixv0.18 SENSING-SOURCES-2026-10-09 supplies every FP/RP/GT source locator, exact contribution chain and owned residual/gate. The following reverse view rows are projections of that single adoption manifest, not new dictionaries or wire schemas.

| Exact component/view revision | Authoritative common master | Retained producer → consumer / domain meaning | Local requirement → planned case | Exact40 supporting cases / residual gate |
| --- | --- | --- | --- | --- |
| AOS-13-CON-001 / documentv0.2 | KX-05/09/10/13/16/18/24; COORD ACT/CHG | Authorised owner/01/05/dependencies →13/02/executors: exact scope/revision/purpose/steps/states/conditions/source instruments/human boundary, closure/fallback rules, rationale and compatible actual applied manifest; unapplied/unknown meaning not usable | AOS-13-REQ-001, AOS-13-REQ-002, AOS-13-REQ-010, AOS-13-REQ-014, AOS-13-REQ-049 → AOS-13-VER-001, AOS-13-VER-002, AOS-13-VER-007, AOS-13-VER-010, AOS-13-VER-035 | AOS-40-VER-020, AOS-40-VER-025, AOS-40-VER-029, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-13-CON-002 / documentv0.2 | KX-01/04/08/09/16/21; REC-E/Q/X | Permitted domain/source/02/runtime →13→02/executors/reviewers: stable case/request/event/attempt identities, definition/profile/version, source assurance, time/standing, dependencies/pending work, current state/effects/residual duties; duplicates/order do not redefine truth | AOS-13-REQ-003, AOS-13-REQ-004, AOS-13-REQ-005, AOS-13-REQ-006, AOS-13-REQ-007, AOS-13-REQ-008, AOS-13-REQ-048 → AOS-13-VER-003, AOS-13-VER-004, AOS-13-VER-005, AOS-13-VER-006, AOS-13-VER-035 | AOS-40-VER-025, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-13-CON-003 / documentv0.2 | KX-07/19/21/26;13-IF-001; KPR/COORD ACC/WHD | 13/domain/control finding →permitted 30/human/recipient; stage result →13/02: existing 13-IF-001/KX-07, KX-21 and KX-26/WHD meaning; exact duty/source/limits, tracker, recipient/role/power, deadline/cover, receipt/validation/application/responsibility and residual rejected/unresolved scope; KPR protected route | AOS-13-REQ-016, AOS-13-REQ-017, AOS-13-REQ-018, AOS-13-REQ-019, AOS-13-REQ-020, AOS-13-REQ-026, AOS-13-REQ-041 → AOS-13-VER-011, AOS-13-VER-012, AOS-13-VER-013, AOS-13-VER-014, AOS-13-VER-019, AOS-13-VER-029 | AOS-40-VER-009, AOS-40-VER-021, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-13-CON-004 / documentv0.2 | KX-02/03/04/13/16/18/20/24/25; CHECK/ACT/CHG/RSV/BRK | 13 →04/05/shared controls/external route 14; result →13/02: exact task/request/attempt/arguments/actor/current source vector, authority/use, CHECK/applied configuration, shared account/reservations, observed prevented/applied/partial/unknown effect and reconciliation; no private copy of grant or account semantics | AOS-13-REQ-011, AOS-13-REQ-012, AOS-13-REQ-013, AOS-13-REQ-015, AOS-13-REQ-021, AOS-13-REQ-022, AOS-13-REQ-023, AOS-13-REQ-025, AOS-13-REQ-044, AOS-13-REQ-046 → AOS-13-VER-008, AOS-13-VER-009, AOS-13-VER-010, AOS-13-VER-015, AOS-13-VER-016, AOS-13-VER-018, AOS-13-VER-032, AOS-13-VER-033 | AOS-40-VER-014, AOS-40-VER-020, AOS-40-VER-022, AOS-40-VER-023, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-13-CON-005 / documentv0.2 | KX-01/06/07/08/12/14/21/23/26; Profiles§§4/5;10-CON-004/11-CON-003/004 | 10/02 evidence +30 human scope →13↔11/14/service source: original communicated promise/precision/scope/revisions, completion rule/work/inspection/dispute standing, comparison classification, accepted owner/team cover, permitted both-contact communication result, actual outcome/residual duty; domain meanings unchanged | AOS-13-REQ-030, AOS-13-REQ-031, AOS-13-REQ-032, AOS-13-REQ-033, AOS-13-REQ-034, AOS-13-REQ-035, AOS-13-REQ-036, AOS-13-REQ-037, AOS-13-REQ-038, AOS-13-REQ-039 → AOS-13-VER-022, AOS-13-VER-023, AOS-13-VER-024, AOS-13-VER-025, AOS-13-VER-026, AOS-13-VER-027 | AOS-40-VER-007, AOS-40-VER-008, AOS-40-VER-009, AOS-40-VER-010, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-13-CON-006 / documentv0.2 | KX-01/08/17/19; REC-E/Q; KX-22 only after20 canonical admission | 13/02 admitted observation →permitted service/22/24/25/40: population/period/coverage, exact intended definition versus observed transaction, source/assurance/uncertainty, baseline/rubric/interpretation, owner/remedy/outcome and suppressed/unobserved scope; no completeness/legal pass inferred | AOS-13-REQ-005, AOS-13-REQ-006, AOS-13-REQ-007, AOS-13-REQ-008, AOS-13-REQ-009, AOS-13-REQ-010, AOS-13-REQ-047 → AOS-13-VER-004, AOS-13-VER-005, AOS-13-VER-006, AOS-13-VER-007, AOS-13-VER-034 | AOS-40-VER-011, AOS-40-VER-025, AOS-40-VER-027, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-13-CON-007 / documentv0.2 | KX-01/04/06/13/15/16/17/21; COORD CHG; REC-E/Q/X | Execution/humans/domain stewards →13/02/21/25/30: actual consequences, approved human rationale, definition history/lesson/proposal, change impacts/applied acknowledgements and residual duties; governed lifecycle; no self-amendment | AOS-13-REQ-027, AOS-13-REQ-028, AOS-13-REQ-029, AOS-13-REQ-043, AOS-13-REQ-048 → AOS-13-VER-020, AOS-13-VER-021, AOS-13-VER-031, AOS-13-VER-035 | AOS-40-VER-006, AOS-40-VER-022, AOS-40-VER-023, AOS-40-VER-025, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-13-CON-008 / documentv0.2 | RSVIEW-0.1;02§6.6/04-CON-009; KX-23/07/06/05/13/17/21 | Assigned specialist/14/13 →02/30/01/affected owners: common RSVIEW-0.1 profile/run/finding/disposition plus exact process implications; actual coverage/reviewer duties/change standing explicit | AOS-13-REQ-050, AOS-13-REQ-051, AOS-13-REQ-052, AOS-13-REQ-053, AOS-13-REQ-054 → AOS-13-VER-036, AOS-13-VER-037, AOS-13-VER-038 | AOS-40-VER-031, AOS-40-VER-032, AOS-40-VER-033, AOS-40-VER-034, AOS-40-VER-035; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |

### Individual-source reverse navigation

Rows below identify the exact controlled source locator and this component’s selected contribution or owned residual. Full source propositions and all other counterparts remain in the Matrix addendum; row numbers do not invent source IDs. This record completes source disposition, not source sufficiency or institutional assessment.

| Source locator | Selected component chain / residual disposition |
| --- | --- |
| FP 1 Telos/conferred purpose/function | AOS-13-REQ-001 → AOS-13-VER-001; Matrix source row retains owned residual and gate |
| FP 2 Permanently human Mode 2 | AOS-13-REQ-024 → AOS-13-VER-017; Matrix source row retains owned residual and gate |
| FP 3 Architectural integrity | AOS-13-REQ-011, AOS-13-REQ-013, AOS-13-REQ-049 → AOS-13-VER-008, AOS-13-VER-009, AOS-13-VER-035; Matrix source row retains owned residual and gate |
| FP 4 Radical transparency | AOS-13-REQ-048 → AOS-13-VER-035; Matrix source row retains owned residual and gate |
| FP 5 Bounded rationality/imperfection | AOS-13-REQ-057 → AOS-13-VER-040; Matrix source row retains owned residual and gate |
| FP 6 Epistemic humility | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 7 No-exit obligation | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 8 Constitutional mediator | AOS-13-REQ-012, AOS-13-REQ-029 → AOS-13-VER-008, AOS-13-VER-021; Matrix source row retains owned residual and gate |
| FP 9 Compliance as consequence | AOS-13-REQ-010 → AOS-13-VER-007; Matrix source row retains owned residual and gate |
| FP 10 Complexity/emergence | AOS-13-REQ-013, AOS-13-REQ-025 → AOS-13-VER-009, AOS-13-VER-018; Matrix source row retains owned residual and gate |
| RP 1: Architecture and Completeness: Every governance process must close its feedback loop. | AOS-13-REQ-027, AOS-13-REQ-028 → AOS-13-VER-020, AOS-13-VER-021; Matrix source row retains owned residual and gate |
| RP 2: Architecture and Completeness: Every human accountability layer must be explicitly named, sequenced, and time - bounded before any process is consid... | AOS-13-REQ-016, AOS-13-REQ-017, AOS-13-REQ-018 → AOS-13-VER-011, AOS-13-VER-012; Matrix source row retains owned residual and gate |
| RP 3: Architecture and Completeness: Every option set must include the option that cannot be made to work. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 4: Architecture and Completeness: The ‘AI said so’ test must be passable at every decision point. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 5: The Mode 1 / Mode 2 Boundary: Mode 2 is permanently human. | AOS-13-REQ-024 → AOS-13-VER-017; Matrix source row retains owned residual and gate |
| RP 6: The Mode 1 / Mode 2 Boundary: Every Mode 1 boundary is a governance instrument, not a technical setting. | AOS-13-REQ-001, AOS-13-REQ-002 → AOS-13-VER-001, AOS-13-VER-002; Matrix source row retains owned residual and gate |
| RP 7: The Mode 1 / Mode 2 Boundary: The boardroom is a Mode 2 deliberative space. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 8: The Mode 1 / Mode 2 Boundary: The Mode 1/Mode 2 boundary is under continuous pressure from AI capability growth. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 9: The 1+5 Architecture: Every proposed governance mechanism must be tested against the 1+5 structure to confirm which layer it belongs to and... | AOS-13-REQ-024 → AOS-13-VER-017; Matrix source row retains owned residual and gate |
| RP 10: The 1+5 Architecture: Risk is intrinsic to each intelligence layer, not a separate domain. | AOS-13-REQ-009, AOS-13-REQ-010 → AOS-13-VER-007; Matrix source row retains owned residual and gate |
| RP 11: The 1+5 Architecture: Every intelligence layer boundary where welfare - adjacent or safety - adjacent signals may arise must have an explic... | AOS-13-REQ-016, AOS-13-REQ-017, AOS-13-REQ-018, AOS-13-REQ-019, AOS-13-REQ-020 → AOS-13-VER-011, AOS-13-VER-012, AOS-13-VER-013, AOS-13-VER-014; Matrix source row retains owned residual and gate |
| RP 12: The 1+5 Architecture: The Golden Thread obligation under the Building Safety Act 2022 is not a technical data management requirement. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 13: Options and Decisions: Options generated by the architecture must be grounded in the organisation’s actual state — actual covenant condition... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 14: Options and Decisions: Every consequential decision must feed back into the Unified Data Layer as a structured record — not only the decisio... | AOS-13-REQ-028, AOS-13-REQ-048 → AOS-13-VER-021, AOS-13-VER-035; Matrix source row retains owned residual and gate |
| RP 15: Options and Decisions: Revealed preferences from real decisions take precedence over stated preferences in policy documents when the archite... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 16: Blind Spots and Honesty: The architecture must name what it cannot see. | AOS-13-REQ-005 → AOS-13-VER-004; Matrix source row retains owned residual and gate |
| RP 17: Blind Spots and Honesty: The dynamic risk perimeter question must be asked at board level as a standing agenda item: not only ‘what are our ri... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 18: Blind Spots and Honesty: The interaction of intelligence layers produces system - level behaviours that no individual layer would produce alone. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 19: Ethics and Telos: Every process must demonstrate a traceable relationship to the organisation’s ethical commitments and social purpose. | AOS-13-REQ-001 → AOS-13-VER-001; Matrix source row retains owned residual and gate |
| RP 20: Ethics and Telos: The architecture must be capable of detecting purpose drift — the condition where operational processes have graduall... | AOS-13-REQ-028 → AOS-13-VER-021; Matrix source row retains owned residual and gate |
| RP 21: Ethics and Telos: Diversity, inclusion, and equitable outcomes are not separate compliance obligations. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 22: Ethics and Telos: Where the organisation’s welfare obligation to residents and its consent architecture pull in opposing directions, th... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 23: Ethics and Telos: AI systems have function, not telos. | AOS-13-REQ-029 → AOS-13-VER-021; Matrix source row retains owned residual and gate |
| RP 24: Ethics and Telos: Where the organisation's purpose is interpreted through an accumulating body of AI-mediated rulings rather than appli... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 25: Ethics and Telos: Every AI system deployed by the organisation carries an embedded constitutional framework established by its developer. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 26: Ethics and Telos: The no - exit condition is a constitutive feature of the organisation’s moral architecture, not background context. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 27: Ethics and Telos: Compliance is the output of sound governance design, not its objective. | AOS-13-REQ-010 → AOS-13-VER-007; Matrix source row retains owned residual and gate |
| RP 28: Radical Transparency: If you cannot audit it and be held accountable for it, it cannot be done. | AOS-13-REQ-048 → AOS-13-VER-035; Matrix source row retains owned residual and gate |
| RP 29: Radical Transparency: The architecture must be more transparent than the document - based governance it replaces, not less. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 30: Radical Transparency: Transparency obligations extend to the architecture’s uncertainty. | AOS-13-REQ-008 → AOS-13-VER-006; Matrix source row retains owned residual and gate |
| RP 31: Agentic Delegation: Agents operate under explicitly delegated authority, not implied authority. | AOS-13-REQ-011, AOS-13-REQ-012 → AOS-13-VER-008; Matrix source row retains owned residual and gate |
| RP 32: Agentic Delegation: Agent authority is domain - specific, context - specific, and condition - specific simultaneously. | AOS-13-REQ-003, AOS-13-REQ-011, AOS-13-REQ-012 → AOS-13-VER-003, AOS-13-VER-008; Matrix source row retains owned residual and gate |
| RP 33: Agentic Delegation: Agents cannot commit the organisation to external obligations, initiate unsolicited contact with external parties, or... | AOS-13-REQ-011, AOS-13-REQ-012 → AOS-13-VER-008; Matrix source row retains owned residual and gate |
| RP 34: Agentic Delegation: Internal escalation — routing a signal within the architecture to a human reviewer or to a receiving intelligence lay... | AOS-13-REQ-016, AOS-13-REQ-017, AOS-13-REQ-018, AOS-13-REQ-019, AOS-13-REQ-020 → AOS-13-VER-011, AOS-13-VER-012, AOS-13-VER-013, AOS-13-VER-014; Matrix source row retains owned residual and gate |
| RP 35: Agentic Delegation: The agentic delegation framework is a governance document reviewed by the board, not a technical configuration manage... | AOS-13-REQ-001, AOS-13-REQ-002 → AOS-13-VER-001, AOS-13-VER-002; Matrix source row retains owned residual and gate |
| RP 36: Agentic Delegation: Every agent action must satisfy the ethics and telos test and the radical transparency test independently of the proc... | AOS-13-REQ-001, AOS-13-REQ-048 → AOS-13-VER-001, AOS-13-VER-035; Matrix source row retains owned residual and gate |
| RP 37: Agentic Delegation: Certain classes of finding must reach their required audience regardless of any instruction to suppress or delay them. | AOS-13-REQ-019 → AOS-13-VER-013; Matrix source row retains owned residual and gate |
| RP 38: Data and Sensing Boundaries: Sensing must not exceed its declared purpose. | AOS-13-REQ-042 → AOS-13-VER-030; Matrix source row retains owned residual and gate |
| RP 39: Data and Sensing Boundaries: The boundary between observing an asset and monitoring a behaviour is an absolute architectural boundary, not a matte... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 40: Data and Sensing Boundaries: Where behavioural inference from sensing data is genuinely necessary to serve the resident’s interests — energy pover... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 41: Data and Sensing Boundaries: The purpose limitation principle applies across all intelligence layers, not only to resident - facing sensing. | AOS-13-REQ-042 → AOS-13-VER-030; Matrix source row retains owned residual and gate |
| GT M1.1 Strategic Coherence | AOS-13-REQ-001, AOS-13-REQ-027, AOS-13-REQ-056, AOS-13-REQ-057 → AOS-13-VER-001, AOS-13-VER-020, AOS-13-VER-040 (supporting case selection 001/020/040); Matrix source row retains owned residual and gate |
| GT M1.2 Sensing Architecture | AOS-13-REQ-003, AOS-13-REQ-004, AOS-13-REQ-005, AOS-13-REQ-008 → AOS-13-VER-003, AOS-13-VER-004, AOS-13-VER-006 (supporting case selection 003/004/006); Matrix source row retains owned residual and gate |
| GT M1.3 Risk Intelligence | AOS-13-REQ-009, AOS-13-REQ-010, AOS-13-REQ-016, AOS-13-REQ-017, AOS-13-REQ-018, AOS-13-REQ-019, AOS-13-REQ-020 → AOS-13-VER-007, AOS-13-VER-011, AOS-13-VER-012, AOS-13-VER-013, AOS-13-VER-014 (supporting case selection 007/011/012/013/014); Matrix source row retains owned residual and gate |
| GT M1.4 Composition and Capability | AOS-13-REQ-016, AOS-13-REQ-017, AOS-13-REQ-018, AOS-13-REQ-040 → AOS-13-VER-011, AOS-13-VER-012, AOS-13-VER-028 (supporting case selection 011/012/028); Matrix source row retains owned residual and gate |
| GT M1.5 Performance Legibility | AOS-13-REQ-006, AOS-13-REQ-007, AOS-13-REQ-027, AOS-13-REQ-038 → AOS-13-VER-005, AOS-13-VER-020, AOS-13-VER-026 (supporting case selection 005/020/026); Matrix source row retains owned residual and gate |
| GT M1.6 Compliance Assurance | AOS-13-REQ-009, AOS-13-REQ-010, AOS-13-REQ-056, AOS-13-REQ-057 → AOS-13-VER-007, AOS-13-VER-040 (supporting case selection 007/040); Matrix source row retains owned residual and gate |
| GT M1.7 Governance Documentation | AOS-13-REQ-001, AOS-13-REQ-028, AOS-13-REQ-029, AOS-13-REQ-048, AOS-13-REQ-049 → AOS-13-VER-001, AOS-13-VER-021, AOS-13-VER-035 (supporting case selection 001/021/035); Matrix source row retains owned residual and gate |
| GT M1.8 Accountability Architecture | AOS-13-REQ-016, AOS-13-REQ-017, AOS-13-REQ-018, AOS-13-REQ-036, AOS-13-REQ-037, AOS-13-REQ-038, AOS-13-REQ-039, AOS-13-REQ-040 → AOS-13-VER-011, AOS-13-VER-012, AOS-13-VER-025, AOS-13-VER-026, AOS-13-VER-027, AOS-13-VER-028 (supporting case selection 011/012/025/026/027/028); Matrix source row retains owned residual and gate |
| GT M1.9 Value for Money | AOS-13-REQ-013, AOS-13-REQ-024 → AOS-13-VER-009, AOS-13-VER-017 (supporting case selection 009/017); Matrix source row retains owned residual and gate |
| GT M1.10 Human-AI Interaction Norms | AOS-13-REQ-011, AOS-13-REQ-012, AOS-13-REQ-024, AOS-13-REQ-040 → AOS-13-VER-008, AOS-13-VER-017, AOS-13-VER-028 (supporting case selection 008/017/028); Matrix source row retains owned residual and gate |
| GT M1.11 Learning Metabolism | AOS-13-REQ-027, AOS-13-REQ-028, AOS-13-REQ-029, AOS-13-REQ-038 → AOS-13-VER-020, AOS-13-VER-021, AOS-13-VER-026 (supporting case selection 020/021/026); Matrix source row retains owned residual and gate |
| GT M1.12 Continuous Self-Assessment | AOS-13-REQ-005, AOS-13-REQ-050, AOS-13-REQ-051, AOS-13-REQ-052, AOS-13-REQ-053, AOS-13-REQ-054, AOS-13-REQ-055, AOS-13-REQ-056, AOS-13-REQ-057 → AOS-13-VER-004, AOS-13-VER-036, AOS-13-VER-037, AOS-13-VER-038, AOS-13-VER-039, AOS-13-VER-040 (supporting case selection 004/036/037/038/039/040); Matrix source row retains owned residual and gate |
| GT M1.13 Emergent System Behaviour | AOS-13-REQ-013, AOS-13-REQ-021, AOS-13-REQ-022, AOS-13-REQ-025, AOS-13-REQ-045, AOS-13-REQ-046 → AOS-13-VER-009, AOS-13-VER-015, AOS-13-VER-018, AOS-13-VER-033 (supporting case selection 009/015/018/033); Matrix source row retains owned residual and gate |
| GT M1.14 Golden Thread Integrity | AOS-13-REQ-030, AOS-13-REQ-031, AOS-13-REQ-032, AOS-13-REQ-033, AOS-13-REQ-034, AOS-13-REQ-035, AOS-13-REQ-036, AOS-13-REQ-037, AOS-13-REQ-038 → AOS-13-VER-022, AOS-13-VER-023, AOS-13-VER-024, AOS-13-VER-025, AOS-13-VER-026 (supporting case selection 022/023/024/025/026); Matrix source row retains owned residual and gate |
| GT M2.1 Values Architecture | AOS-13-REQ-011, AOS-13-REQ-012, AOS-13-REQ-019, AOS-13-REQ-020, AOS-13-REQ-042 → AOS-13-VER-008, AOS-13-VER-013, AOS-13-VER-014, AOS-13-VER-030 (supporting case selection 008/013/014/030); Matrix source row retains owned residual and gate |
| GT M2.2 Coherence Under Pressure | AOS-13-REQ-019, AOS-13-REQ-020, AOS-13-REQ-056, AOS-13-REQ-057 → AOS-13-VER-013, AOS-13-VER-014, AOS-13-VER-040 (supporting case selection 013/014/040); Matrix source row retains owned residual and gate |
| GT M2.3 Incommensurable Trade-off Capacity | AOS-13-REQ-024, AOS-13-REQ-040 → AOS-13-VER-017, AOS-13-VER-028 (supporting case selection 017/028); Matrix source row retains owned residual and gate |
| GT M2.4 Epistemic Brake Function | AOS-13-REQ-005, AOS-13-REQ-009, AOS-13-REQ-010, AOS-13-REQ-021, AOS-13-REQ-022, AOS-13-REQ-056, AOS-13-REQ-057 → AOS-13-VER-004, AOS-13-VER-007, AOS-13-VER-015, AOS-13-VER-040 (supporting case selection 004/007/015/040); Matrix source row retains owned residual and gate |
| GT M2.5 Directorial Independence | AOS-13-REQ-019, AOS-13-REQ-041, AOS-13-REQ-056, AOS-13-REQ-057 → AOS-13-VER-013, AOS-13-VER-029, AOS-13-VER-040 (supporting case selection 013/029/040); Matrix source row retains owned residual and gate |
| GT M2.6 Social Legitimacy | AOS-13-REQ-036, AOS-13-REQ-037, AOS-13-REQ-038, AOS-13-REQ-039 → AOS-13-VER-025, AOS-13-VER-026, AOS-13-VER-027 (supporting case selection 025/026/027); Matrix source row retains owned residual and gate |
| GT M2.7 No-Exit Obligation | AOS-13-REQ-020, AOS-13-REQ-039, AOS-13-REQ-040, AOS-13-REQ-042 → AOS-13-VER-014, AOS-13-VER-027, AOS-13-VER-028, AOS-13-VER-030 (supporting case selection 014/027/028/030); Matrix source row retains owned residual and gate |
| GT M2.8 Radical Transparency | AOS-13-REQ-003, AOS-13-REQ-004, AOS-13-REQ-006, AOS-13-REQ-007, AOS-13-REQ-048, AOS-13-REQ-049 → AOS-13-VER-003, AOS-13-VER-005, AOS-13-VER-035 (supporting case selection 003/005/035); Matrix source row retains owned residual and gate |
| GT M2.9 Moral Drift Detection | AOS-13-REQ-013, AOS-13-REQ-028, AOS-13-REQ-029, AOS-13-REQ-047, AOS-13-REQ-056, AOS-13-REQ-057 → AOS-13-VER-009, AOS-13-VER-021, AOS-13-VER-034, AOS-13-VER-040 (supporting case selection 009/021/034/040); Matrix source row retains owned residual and gate |
| GT M2.10 Purpose Stability | AOS-13-REQ-001, AOS-13-REQ-011, AOS-13-REQ-012, AOS-13-REQ-014, AOS-13-REQ-015, AOS-13-REQ-053, AOS-13-REQ-054 → AOS-13-VER-001, AOS-13-VER-008, AOS-13-VER-010, AOS-13-VER-038 (supporting case selection 001/008/010/038); Matrix source row retains owned residual and gate |
| GT M2.11 Murmuration Capacity | AOS-13-REQ-019, AOS-13-REQ-024, AOS-13-REQ-041 → AOS-13-VER-013, AOS-13-VER-017, AOS-13-VER-029 (supporting case selection 013/017/029); Matrix source row retains owned residual and gate |
| GT M2.12 Constitutional Authority | AOS-13-REQ-011, AOS-13-REQ-012, AOS-13-REQ-024, AOS-13-REQ-053, AOS-13-REQ-054 → AOS-13-VER-008, AOS-13-VER-017, AOS-13-VER-038 (supporting case selection 008/017/038); Matrix source row retains owned residual and gate |
| GT M2.13 AI Constitutional Framework Governance | AOS-13-REQ-011, AOS-13-REQ-012, AOS-13-REQ-044, AOS-13-REQ-047 → AOS-13-VER-008, AOS-13-VER-032, AOS-13-VER-034 (supporting case selection 008/032/034); Matrix source row retains owned residual and gate |
| GT M2.14 Purpose-Led Design | AOS-13-REQ-001, AOS-13-REQ-055 → AOS-13-VER-001, AOS-13-VER-039 (supporting case selection 001/039); Matrix source row retains owned residual and gate |
| GT M2.15 Telos / Function Distinction | AOS-13-REQ-027, AOS-13-REQ-038, AOS-13-REQ-056, AOS-13-REQ-057 → AOS-13-VER-020, AOS-13-VER-026, AOS-13-VER-040 (supporting case selection 020/026/040); Matrix source row retains owned residual and gate |

Author consistency conclusion: functional roles and repair/private/workforce/external/research/control/failure boundaries agree with the current shared infrastructure. SENS-CR-01–05 closed as author document corrections; wire profiles, operating roles/capacity, domain/annex/legal sufficiency and observed evidence remain open per§17 and40. No independent/executed conformance or operating readiness claim. Earlier dated text/addenda describe history; this current control takes precedence.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**Historical status notice — sensing consistency closure — 9 October 2026:** Mark authorised the remaining consistency work. SENS-CR-01–05 are closed at the functional-document/author-review level: all40 logical CON views across10–14 and40 have exact central adoption, producer/consumer/shared-owner and REQ/VER links; all80 controlled FP/RP/GT sources have precise current contributions and owned residual/gate dispositions; current body/control statements are reconciled. Versions10v0.4/11v0.3/12v0.3/13v0.2/14v0.8/40v0.6; Architecture/Mapv0.42; Sharedv0.18/Corev0.6/ExchangeRegisterv0.17/SourceMatrixv0.18; reviewv0.4. DEC001–096 unchanged. Sensing269 proposed REQs/176 planned VERs;40 retains40/38. No new requirement/case/interface, source promotion or execution. Exact compatible wire schemas/profiles, organisation appointments/capacity, independent review, legal/institutional/practice evidence and scoped build/activation remain separate; independent project review remains deferred. Earlier dated notices/addenda are historical. Current controlling allocation is the9October manifest and source addendum below.

