# AOS — Extension, architectural fit and scoped conformance

Document: aos-extension-and-conformance-specification-v0-1 · Source revision or record: v0.1

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

| Document control | Value |
| --- | --- |
| Identifier / version / date | AOS-EC / 0.1 / 9 October 2026 |
| Status | Functional review draft; proposed obligations and planned assessments; no certification or implementation approval |
| Purpose | To-do item 12: enable a supplier to answer “Where does my product fit?” and declare its contribution, dependencies, evidence and gaps |
| Authority | Mark’s 9 October clarification of items 12/12a; existing AOS-00 DEC-001–097; no new component, power or approved interface identifier |
| Baseline | AOS-00/Map v0.45 reviewed; v0.46 records this document’s allocation. Shared v0.21, Core v0.6, Exchange Register v0.20, Matrix v0.21; current component revisions retained |
| Owner / reviewers | Project custodian Mark Sweeny; author Codex. Organisational semantic owners and competent assessors require appointment; independent project review deferred |
| Quality / release | AOS-QS v0.1; cross-cutting support specification, not a twentieth component. Logical supplier-fit scope; executable profiles/endpoints and build/activation remain items 11/11a/11b |

## 1. The supplier’s question

A supplier should leave with a clear account of the AOS responsibilities its product supports, information it supplies or consumes, controls and decisions that belong elsewhere, and capabilities or integration work still needed. An established product can provide several architectural functions; several products and human procedures can jointly provide one function. The architecture does not require one purchased application per intelligence.

This specification defines the common method and obligations behind that account. Item 12a will turn it into the supplier-facing briefing and submission route. Architectural fit can be assessed before a deployed API exists. A claim about working interoperability needs an implementation and observed evidence.

“Extension” includes a product contribution, adapter, integration, optional module or organisation-specific configuration using existing AOS responsibilities. This does not adopt a sector-independent core, add another intelligence domain or resume CAP-01/02. Those use cases remain in Phase 2 under DEC-097. England/housing scope, separate organisation instances and existing-system integration remain the governing directions.

## 2. Sources and interpretation

| Key | Controlled locator / use |
| --- | --- |
| ARCH | AOS-00 §§3–6/9; DEC-002/005/014–020/028–030/062–078/086/092–097: ownership, existing systems, scoped claims, current controls and Phase 2 boundary |
| COMMON | Shared §§2–5; Core REC-E/Q/A/D/X; Register §§3–7/12–20 and current sensing manifest; Coordination §§3–5; Protected Reporting/Recovery: one meaning, permission, changes, duties and reconciliation |
| DOMAIN | AOS-10–14 §§3/6/10/17/20; supplier allocations, domain interpretation, privacy, external exchange and owned gaps |
| GI/HUMAN | AOS-20–25 and 30 §§3/6/7/10/15/17: evidence, interpretation, presentation, oversight and empowered human judgement |
| ASSURANCE | AOS-40 §§10/12/15/17/20 and acceptance annex §§2–6; QS-14–25: exact scope, observable criteria, methods, evidence and limited claims |
| PRINCIPLES | Controlled FP v4 principles 1/2/3/7/8/10; RP v6 domains 1/2/4/5/6/7/8/9; GT M1.2/3/7/8/10/11/13/14 and M2.3/4/5/8/9/12–15: derivation context, not an institutional pass |
| RESEARCH | DEC-086; AOS-04 common research profile, AOS-02 §6.6 shared research views and AOS-01 change authority: observe/challenge/propose without self-amendment |

These sources constrain the proposed requirements. No new legal conclusion, external standard, API format, performance target or operating permission is asserted. Detailed applicable source/requirement/case bindings are part of the individual contribution dossier.

## 3. Product-to-architecture mapping

| Product family | Potential contribution | Information or interfaces | Responsibilities retained elsewhere |
| --- | --- | --- | --- |
| Housing management / repairs | Service records, promises, contacts, transactions and workflow; Asset/Resident/Process inputs (10/11/13) | Attributable evidence, exact source IDs/revisions, case events, actual work and outcome records through 02; external contractor exchange through 14 | Source status is not verified completion; 01/03/05 control consequential use; 13 tracks duties; empowered humans accept responsibility |
| Asset management / building information | Asset identities, inspections, condition, coverage, maintenance and information handover (10) | Source/assurance/correction and building-information exchanges via 02 and relevant 10 views | Physical assurance and applicable dutyholder judgement need competent evidence; transport or a populated field does not prove safety |
| HR / workforce systems | Employment records, capability evidence and permitted workforce-service processes (12) | Purpose-bound workforce evidence, scoped referrals and corrections via 02/03/12 | Human employment judgement, rights, representation and approved workforce-use policy; no integration-derived surveillance permission |
| Sensors / IoT | Condition observations, device/source health, timestamps and coverage for Asset/Process (10/13) | Exact asset/source identity, units, time precision, uncertainty, gaps and correction via 02; external service exchanges as applicable via 14 | Observation is not a repair outcome or personal inference permission; 03 use controls and competent domain interpretation remain necessary |
| Workflow / case management | Definitions, accepted assignments, deadlines, cover, exceptions and outcome tracking (13/30) | Process/duty/decision references, acknowledgement stages and change notices | Delivery is not accepted responsibility; assignment is not capacity or fulfilment; 30 and authorised service owners supply actual human standing |
| Governance / document tools | Evidence/corpus custody, assessment inputs, faithful presentation, governance records (21–25/30) | Canonical analysis, permitted projections, exact record/approval status and corrections | No AI boardroom capture, machine moral adjudication or software-only governance certificate; GI/human owners retain governing judgement |
| Integration / identity / platform services | Source adapters, shared data, identity, agents and runtime support (01–05/14) | Existing record/control/view families and exact revision/permission/compatibility evidence | Hosting, authentication, successful transmission or supplier configuration alone does not establish authority, data-use permission or architectural conformance |

These are candidate mappings, not assessments of named suppliers. Each specific product/version/configuration must show its actual contribution. A human or manual service can be part of the declared realisation, with its authority, capacity, evidence and continuity requirements visible.

## 4. Contribution dossier and responsibility boundary

Every dossier records:

- Product, supplier, version/configuration, organisation instance and precise proposed use; assessed architectural and contract baselines.
- Supported AOS functions and exact applicable requirement/CON/view identifiers; producer/consumer direction and boundary to other products or humans.
- Authoritative source of each fact, decision and state; substantive domain owner and common semantic owner; permitted projections and source assurance.
- Existing capability, adaptation needed, external dependency, not provided or unresolved standing for each contribution. These are dossier labels, not new common wire enums.
- Information required/supplied, units/time/identity/status/revision, restrictions, corrections and acknowledgement/effect/fulfilment evidence.
- Authority, lawful purpose/use, human approval, recipient/channel, operational-role and failure/cover dependencies.
- Claim level and scope; evidence references, assessor/review standing, limitations, exclusions and accountable gap owner/next action.

A supplier contact can explain and attest its product. That contact does not acquire the organisation’s semantic ownership or approval powers. Overlapping systems must identify the authoritative source for the particular purpose; arrival order or vendor preference cannot decide it. No adapter silently replaces an AOS semantic definition.

## 5. Contracts and implementation binding

The contribution uses the existing shared record families and component CON views. It identifies required meaning, provenance, status, ordering, corrections, permitted use and required acknowledgements. The owner reviews any translation and its declared losses. Unsupported or unresolved meanings remain rejected/held for dependent use, with an owned exception.

Read-only observations, internal workflow, external disclosure, commitment and execution are classified by actual operation and control/data-use path. Hosting location alone does not classify an external boundary. Monetary and resource impacts remain distinct. Where applicable, current authority/use, exact action binding, runtime validation/accounting and separately observed effects survive every adapter or combined product.

Before implementation-specific reliance, item 11a binds the logical contribution to exact wire schemas, versions, supported operations, protocol/routes, authentication/identity assurance, organisation instruments, confidentiality, clocks, observation methods and acceptance fixtures. This draft does not publish endpoints, an SDK or a test service. It enables a precise fit/dependency discussion and supplies the logical obligations for that later binding.

## 6. Scoped conformance and evidence

| Proposed declaration | What it supports | Required basis / limit |
| --- | --- | --- |
| Architectural contribution mapped | “This product supports these responsibilities, with these dependencies/gaps” | Exact scoped mapping, owner review and truthful capability standing; no implementation-conformance claim |
| Logical contract alignment assessed | “These proposed exchanges preserve the required AOS meanings and boundaries” | Reviewable definitions, translations, applicable requirements and planned assessment; still no observed interoperability |
| Implementation behaviour verified for a scope | “This exact configured contribution demonstrated these requirements under these conditions” | Actual compatible endpoint/control/effect observations, competent assessment, failures/retests and bounded exclusions; not whole-AOS or institutional certification |

The labels are proposed reporting distinctions, not a certification scheme or operating grant. Different aspects of one product can have different evidence standing. A supplier cannot combine favourable partial results into whole-AOS approval. The scope statement names the supported requirements, environment/configuration, tested dependencies and exclusions; required missing evidence withholds the dependent claim.

Testing follows the existing AOS-40 method, independent-assertion results and evidence rules. A model’s refusal narrative cannot prove enforcement; a delivery response cannot prove acceptance or fulfilment. Human participation, practical usability, institutional effectiveness and legal applicability retain their own competent assessment. Every gap has an owner and consequence for the claim. Material changes trigger impact-selected reassessment; old evidence is retained with its original baseline.

## 7. Proposed requirements and traceability

All AOS-EC-REQ rows are proposed support-specification obligations, logical release only. Owner: project contribution/conformance custodian with the authoritative component/domain/control owner; Mark approves project changes, actual organisation authorities approve operating instruments. Origins: v0.1, 9 October. Dependencies: §§4–6/10; rationale in the obligation and source allocation below. No default supplies missing organisation or implementation values.

| ID | Independently assessable obligation | Source / rationale | Planned VER |
| --- | --- | --- | --- |
| AOS-EC-REQ-001 | Bind each contribution declaration to exact product/configuration, entity, intended use and architecture/contract baseline. | ARCH/ASSURANCE; prevent ambiguous scope | 001 |
| AOS-EC-REQ-002 | Map the contribution to exact supported AOS functions/requirements/views and named dependencies without implying whole-suite support. | ARCH/DOMAIN; make fit and limits explicit | 001 |
| AOS-EC-REQ-003 | Identify combined, adapter-supported and manual contributions separately from capabilities provided directly by the product. | ARCH/DOMAIN; truthful realisation | 002 |
| AOS-EC-REQ-004 | Identify authoritative source and substantive/common semantic ownership without delegating reserved AOS or human powers by product selection. | ARCH/COMMON/GI/HUMAN; preserve ownership | 002 |
| AOS-EC-REQ-005 | Reference the single existing contract definition for each declared exchange and identify producer, consumer and permitted direction. | COMMON; prevent competing meanings | 003 |
| AOS-EC-REQ-006 | Describe required identities, units/time basis, source/assurance, revision/status and use restrictions for the intended exchange. | COMMON/DOMAIN; preserve usable evidence | 003 |
| AOS-EC-REQ-007 | Preserve correction, ordering, withdrawal and lifecycle restrictions through every adapter, projection and dependent consumer. | COMMON; prevent stale or unrestricted use | 004 |
| AOS-EC-REQ-008 | Distinguish receipt, validation, application, accepted responsibility, actual effect and fulfilment wherever the exchange purpose requires them. | COMMON/DEC-093/094; no transport-success substitution | 004 |
| AOS-EC-REQ-009 | Declare and preserve independent authority, data-use and runtime/control prerequisites for every consequential contribution. | ARCH/COMMON; no integration-derived power | 005 |
| AOS-EC-REQ-010 | Declare and preserve private Resident, workforce, sensitive-data and organisation-instance boundaries for every included processing route. | DOMAIN/03; no privilege-by-connection | 005 |
| AOS-EC-REQ-011 | Identify supported contract revisions, reviewed translations and declared losses; unresolved incompatibility shall withhold dependent use or favourable claim. | COMMON; compatibility is evidenced | 006 |
| AOS-EC-REQ-012 | Define observable failure, interruption, retry/reconciliation, continuity and supplier-exit responsibilities for the contribution’s scope. | COMMON/05/DOMAIN; ongoing duties survive product failure | 006 |
| AOS-EC-REQ-013 | State each claim’s level and exact assessed scope without implying whole-AOS certification or operating approval. | ASSURANCE/QS; bounded conformance | 007 |
| AOS-EC-REQ-014 | Link any implementation-verification claim to actual observations and competent assessment for the declared configuration and required assertions. | ASSURANCE; documentary mapping is not execution | 007 |
| AOS-EC-REQ-015 | Record unsupported, partial, unresolved or excluded contributions with an accountable gap owner and their effect on dependent claims. | ASSURANCE/COMMON; honest residuals | 008 |
| AOS-EC-REQ-016 | Retain prior evidence and require affected-scope reassessment after material product, contract, permission, configuration or dependency change. | COMMON/ASSURANCE; no stale inheritance | 008 |
| AOS-EC-REQ-017 | Supply a worked boundary-spanning example linking product contribution, common records, retained owners and actual outcome criteria. | DOMAIN/ASSURANCE; make fit concrete | 009 |
| AOS-EC-REQ-018 | Present the mapping so representative suppliers can identify their contribution, dependencies and gaps without guessing architectural ownership. | Mark’s item12 clarification/QS; usable supplier answer | 009 |
| AOS-EC-REQ-019 | Bind external research on this specification to an approved inherited research remit, baseline and source/coverage/limitation record. | RESEARCH; governed adaptation | 010 |
| AOS-EC-REQ-020 | Route supplier feedback/research proposals through controlled human disposition without automatically changing contracts, claims or the specification. | RESEARCH/ARCH; proposal is not amendment | 010 |

## 8. Planned assessments

All cases are unexecuted. Common method: controlled document inspection/walkthrough; when implementation is claimed, separately authorised integration/failure tests and actual observations. Assessor: appointed contribution reviewer with competent semantic/control/domain/service reviewers; supplier usability additionally requires representative supplier assessment. Missing mandatory fixture, authority, assessor, endpoint or rubric blocks the dependent assessment. Each contrast/assertion records its own result under AOS-40 rules.

Evidence for each case: exact requirement/fixture/baselines, ordered steps, expected versus observed outcomes, method and assessor, permitted source/access, actual sink/effect where applicable, findings/accepted owner/cover/retest, limitations and retained lifecycle. A document exercise can judge logic only.

| Case / requirements | Fixture and procedure | Observable acceptance / evidence criterion |
| --- | --- | --- |
| AOS-EC-VER-001 / REQ-001–002 | Compare a bounded sensor contribution with an unspecified “AOS compliant” offer; trace supported functions and exact baseline | Specific fit/dependencies readable; ambiguous or inflated declaration returned with owner; no whole-suite claim |
| AOS-EC-VER-002 / REQ-003–004 | Combined product/adapter/manual workflow; vendor asserts record ownership and human approval by configuration | Actual delivery boundary visible; authoritative owners and required human powers unchanged; missing manual capacity remains a gap |
| AOS-EC-VER-003 / REQ-005–006 | Producer/consumer use one common definition versus altered units/status or undeclared source assurance | Exact common meanings and endpoint roles retained; unsupported value/meaning held; no connectivity-as-truth shortcut |
| AOS-EC-VER-004 / REQ-007–008 | Corrected/withdrawn record arrives out of order; contractor transport receipt offered as completed repair | Current lineage/restrictions retained at consumers; receipt, duty acceptance and actual completion remain separate; no blind retry |
| AOS-EC-VER-005 / REQ-009–010 | Valid permitted service exchange; same connection attempts private transcript, workforce profiling, cross-instance or stale-authority use | Permitted scope can proceed; forbidden dependent use/effect prevented at actual boundary if implemented; documentary logic alone supplies no enforcement pass |
| AOS-EC-VER-006 / REQ-011–012 | Supported translation, lossy/incompatible version, outage, unknown effect and supplier exit | Reviewed losses/suitability visible; dependent incompatible use withheld; reconciliation and continuing service/duties owned; no unknown-as-success |
| AOS-EC-VER-007 / REQ-013–014 | Marketing claim relies on architecture diagram, simulation, model refusal or test evidence for another configuration | Claim limited to actual evidence standing; implementation claim withheld where required observation is absent; qualified human assessment retained |
| AOS-EC-VER-008 / REQ-015–016 | Partial support/exclusion plus changed adapter or permission; previous pass offered unchanged | Exact gap owner/dependency consequence; affected reassessment required; original evidence/history preserved; exclusion gives no coverage |
| AOS-EC-VER-009 / REQ-017–018 | Give representative housing/asset/HR/sensor suppliers the dossier and worked example; ask them to identify contribution, exchanges, retained owners and gaps | Each required answer traceable to the document under approved usability rubric; misunderstandings become owned findings, not inferred supplier acceptance |
| AOS-EC-VER-010 / REQ-019–020 | Supplier/research source proposes new requirement during partial/failed coverage or hostile retrieval | Source/status/coverage limits visible; controlled proposal/disposition retained; no source instruction, publication date or supplier request self-amends the baseline |

## 9. Worked fit example — contractor repair evidence

A repairs platform holds an original resident promise and a contractor work event. Its declared contribution supplies attributable service evidence and transaction status to 02 and10/13;14 governs any external exchange. The dossier identifies exact source IDs, revisions, permitted purposes and the product’s missing assurance or control dependencies.

A contractor response saying “complete” arrives. Transport receipt proves only receipt. Asset/domain assessment preserves whether actual completion is evidenced, disputed, partial or unverified; Process retains the original communicated promise and remaining service duty. A later internal target does not erase that promise. Separately current-checked authority/use/runtime controls govern any consequential follow-up.

An empowered human accepts the escalation scope, with capacity, deadline and cover. The resident is contacted through the currently agreed permitted channel with the required owner/team details. Contact, accepted responsibility, actual repair and service outcome have separate evidence. Resident silence supplies neither satisfaction nor closure. Private assistant content, where such an assistant exists, is not an enterprise feed by default.

The supplier can now state: “We supply these records and workflow events; these architectural controls and domain/human judgements are supplied elsewhere; these translations and evidence gaps need work.” That is architectural fit. Demonstrating the full interaction requires a selected implementation and approved scoped tests under11a/11b.

## 10. Open dependencies and research remit

| Issue | Owner / resolution gate |
| --- | --- |
| EC-ISS-001 — Proposed wording and scope disposition | Mark/project custodian; substantive review before treating the draft as an approved project baseline |
| EC-ISS-002 — Product-specific mapping, sources, rights and accountability | Supplier plus domain/common semantic owners; before favourable contribution assessment or dependent reliance |
| EC-ISS-003 — Exact technical bindings and environment | Implementer/control/semantic owners under11a; before affected build/compatibility or execution claim |
| EC-ISS-004 — Assessor, rubric, representative supplier and evidence lifecycle | Contribution/AOS-40/service owners; before assessment; no usability or conformance result asserted now |
| EC-ISS-005 — Public claim wording, licensing, participation and governance | Mark under12a/13/13a; before publishing an endorsement or contribution scheme |
| EC-ISS-006 — External research profile and continuing review | Project custodian via approved04 research profile,02 shared views and14 access; before commissioning research; no schedule/default agent activation |

Research remit: changes relevant to architectural product mapping, contract compatibility, evidence-supported conformance claims, supplier dependence/exit and integration failures. Bind source/jurisdiction/date/status, exact baseline, method/coverage, limitations and affected requirements. The custodian owns relevance; authorised research may observe, analyse, challenge and propose through existing02/04/14 mechanisms. Accepted findings have an empowered review owner, permitted audience, deadline/cover and controlled disposition. No new intelligence component, universal research owner, autonomous calibration or amendment power is created.

## 11. Author review and programme disposition

Specification quality: source locators, responsibilities,20 individually assessable proposed requirements and10 reverse-linked planned cases, worked example, evidence/claim limits and owned dependencies are present. Author identifier/link and reciprocal primary-coverage checks performed. Design adequacy: the proposed fit method preserves existing owners, human/data/control boundaries and supplier-specific evidence limits. Actual supplier usability, adapter feasibility and implemented enforcement remain unassessed.

No new DEC/IF/REC family, canonical wire enum, technology selection, deployment, legal conclusion or certification authority is introduced. Source statuses/manifest and the previously closed component/acceptance work remain unchanged. This draft completes item12’s functional drafting at author level; Mark review remains5d, supplier briefing12a next, technical binding/verification11a/11b later. Independent project review remains deferred. No G3/G4 or operating approval.

