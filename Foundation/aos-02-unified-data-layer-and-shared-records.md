# AOS-02 — Unified Data Layer and shared records

Document: aos-02-unified-data-layer-and-shared-records · Source revision or record: v0.11

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**DEC-104 adopted — 29 October 2026:** Current revision 0.11. Each mandatory protected-finding category requires assessed technical-failure and implicated-person interference arrangements with an appropriately independent authorised alternative and no implicated sole release gatekeeper. [Decision/amendment record](../Supporting-Specifications/aos-dec-104-protected-reporting-and-implicated-recipients-2026-10-29.md). External reporting is conditional on justified lawful authority, not a default. Exact profiles/permissions, protected_finding v0.3 compatibility and actual evidence remain gates; amended wording retains ordinary separate review and cases are planned/unexecuted. Earlier contrary or narrower baselines are history for this scope.

**DEC-103 adopted — 29 October 2026:** Current revision 0.10. Decision validity/effective time, attributable evidence/authentication, minutes approval and permission to execute are separate. DEC-087 is partly superseded; [decision/amendment and legal-source record](../Supporting-Specifications/aos-dec-103-decision-validity-evidence-and-minutes-2026-10-29.md). No universal later-minutes or second decision-record approval gate. Exact instruments/evidence policy, KX-06 v0.3 compatibility and ordinary separate review/readiness gates remain required; cases unexecuted. Earlier contrary wording is historical only where explicitly identified.

**DEC-099 adopted — 29 October 2026:** Mark approved the derived-information restriction rule. Current document revision 0.9; earlier functional/editorial baselines below are retained history. The [decision and controlled amendment record](../Supporting-Specifications/aos-dec-099-derived-information-restrictions-2026-10-29.md) governs this change. Existing requirement/case/IF identities are retained; amended wording remains subject to the normal separate review and readiness gates. No case execution or operating approval is implied.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

| Document control | Value |
| --- | --- |
| Version / date | 0.11 / 29 October 2026 |
| Status | Review draft; component requirements, schemas and HACT mappings proposed |
| Architecture baseline | AOS-00/Map v0.25, DEC-001–089; AOS-30 functional alignment 7 October 2026 |
| Source baseline | Foundational Principles v4; AOS Reasoning Principles v6; Governance Intelligence Tests, controlled supplied set |
| Component owner / custodian | Common-record stewardship required; appointments unresolved |
| Project baseline approver | Mark Sweeny |
| Organisation approvers | Relevant data/governance/privacy/operational authorities under their approved instruments; appointments unresolved |
| Author | Codex, at Mark's request |
| Independent reviewer | Unassigned; independent project review deferred |
| Quality / template | AOS-QS v0.1; component template v0.4 |
| Release scope | Whole-component logical specification; bounded implementation not authorised |
| Readiness | Author-reviewed draft; no formal readiness gate, build or activation approval |
| External standards status | HACT/OSCRE alignment assessed at reference/concept level; exact adopted release and element mappings unverified |
| Change history | 0.1 initial component draft. 0.2 incorporates approved DEC-045–048 and Radical Transparency clarification: assurance provenance, governed reconciliation/history, HACT preferred reference; adds REQ-037–046 and VER-021–024. 0.3 — 6 October: common decision-baseline/status/interface reconciliation (KR-09 label portion), preserves historical approvals and proposed/planned records; register formatting repaired where applicable (KR-10); see §19.1.  0.4 — DEC-062–066 common exchange adoption; five new proposed adoption REQs/six planned cases and an additional full-assurance-chain REQ; AOS-03 REQ-040 sequencing clarified where applicable.  0.5 — DEC-067–072 control coordination/withholding notification; eight proposed REQs/eight planned cases and reciprocal source/field adoption; original records preserved. 0.6 — DEC-073–078 protected reporting/recovery and standards provenance; six proposed REQs/six planned VERs; prior records preserved.  v0.7 — DEC-086 external-research support, reciprocal AOS-04/02/01 allocation and own component profile; previous records preserved. 7 October — authorised AOS-30 functional adoption, Chair/board approval propagation and material-correction alignment; no new identifiers or operating power. |

### Current catalogue inventory — editorial reconciliation, 29 October 2026

The normative tables contain **73 retained numbered requirement records** and **49 planned verification case identities**. These are catalogue counts, not independent obligations, active-scope coverage, executed tests or accepted results. Earlier totals in dated adoption supplements describe those steps only. The [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) records the suite baseline and count method.

## 1. Purpose and scope

### 1.1 Purpose

AOS-02 establishes shared meaning and reconstructable evidence across the AOS. It enables different intelligences, human workflows and existing systems to refer consistently to the same entities, facts, proposals, decisions, actions and outcomes while preserving their differences, provenance and restrictions.

Unified means governed shared semantics and exchange. It does not mean that all information is copied into one database, that every participant may see every record, or that a disputed claim becomes true because it has entered the layer.

### 1.2 Architectural problem

Without this component, a property, person, repair, decision or delegation can acquire incompatible identities or meanings across systems. A later update can erase a resident's account, an inference can become an asserted fact, and technical dispatch can be reported as accountable closure. Integrations can also combine individually accessible records into an unauthorised new inference.

### 1.3 Intended outcome

An authorised consumer can establish what a record means, which exact revision and organisation it belongs to, where it came from, what time it describes, which restrictions apply, what is uncertain, and how correction or later events affect its use. Producers and consumers use one controlled contract definition.

### 1.4 Scope

Common logical structures and vocabulary; entity/source identity mappings; evidence admission; schema/type/unit/reference validation; temporal meaning; provenance and derivation; correction/dispute/version lifecycle; governed retrieval and exchange; accountability/outcome linkage; retention/deletion evidence; semantic ownership and compatibility; sector-standard mappings.

### 1.5 Exclusions

AOS-01 owns authority semantics. AOS-03 owns identity assurance, access/consent/data-use decisions. AOS-04/05 own execution and runtime control. Domain owners determine factual evidence criteria; AOS-13/30 track operational/human responsibility; AOS-14 governs external exchange; AOS-21 owns corpus/precedent admission; AOS-22/23 analytical method; AOS-25 oversight; AOS-40 assurance.

Existing housing, finance, HR and asset systems can remain authoritative for their approved record types. AOS-02 does not replace them by default or independently adjudicate resident disputes, employment decisions, constitutional interpretation or legal obligations.

## 2. Authority and sources

### 2.1 Governing derivation

FP v4 and RP v6 govern; AOS-00 directions retain their recorded approval status. Exact parent REQ wording remains proposed. GT supplies governance assessment criteria, not software pass claims.

Primary architectural anchors: DEC-002 shared ownership; DEC-005 shared controls; DEC-008 human-approved records; DEC-014 separate instances; DEC-015 existing-system integration; DEC-027 explanation; DEC-028–030 current control/material correction/reconciliation; DEC-031–041 repair evidence, human acceptance and resident channels; DEC-042–044 authority lineage/withdrawal/conflict. Parent requirements include AOS-00-REQ-003/004/010/012/021/024/030/033/035/036/040 and the scoped repair/constitutional records REQ-042–048.

Consulted project sources: FP v4, RP v6 and GT supplied texts read during immediately preceding component work; AOS-00 v0.11/Map v0.8; AOS-QS v0.1/template v0.3; AOS-01 v0.2; Shared Contracts, Core Record Contracts and Operational Profiles v0.1 with current dispositions. Source versions are unchanged; original source manifest remains preserved.

### 2.2 HACT and associated primary references

External sources were consulted on 5 October 2026. They inform interoperability assessment; they do not override AOS governing constraints or confer authority to process personal data.

| Ref | Primary source / exact locator | Finding and limit |
| --- | --- | --- |
| EXT-H01 | [HACT author on NHF: Help us develop a data model for Awaab’s Law](https://www.housing.org.uk/news-and-blogs/blogs/matthew-grenier/help-us-develop-a-data-model-for-awaabs-law/), Matthew Grenier, 11 August 2025, “A new data model” | Describes modular repairs/damp-and-mould work reusing property/customer/repairs use cases. Published explanation, not the complete current standards dictionary |
| EXT-H02 | [MHCLG Digital: Delivering a data standard to support Awaab’s Law](https://mhclgdigital.blog.gov.uk/2025/08/20/delivering-a-data-standard-to-support-awaabs-law-in-social-housing/), 20 August 2025, “The data model” / “Ownership and next steps” | Government project account identifies the model's components and first-working-version status at publication; does not establish today's final release or endorsement |
| EXT-H03 | [Associated Data Futurists repository](https://github.com/data-futurists/damp-and-mould-standards-concept), README “About this project” / “Disclaimer” | Accessed README still identifies a proof of concept not finalised/assured and advises against live-service adoption at that stage; reviewed as research/reference, not production dependency |
| EXT-H04 | [Introducing the damp and mould data model](https://github.com/data-futurists/damp-and-mould-standards-concept/blob/main/guidance/Introducing%20the%20damp%20and%20mould%20data%20model.md), “What’s included” / “Key features” | Component-level concepts and modularity consulted; SQL/DDL implementation not adopted, exact release/commit not pinned |
| EXT-H05 | [How the damp and mould data model works](https://github.com/data-futurists/damp-and-mould-standards-concept/blob/main/guidance/How%20the%20damp%20and%20mould%20data%20model%20works.md), “How data flows” | Illustrates hazard/investigation/work-order/escalation links; statutory time values in guidance are not imported as verified AOS legal rules |
| EXT-H06 | [OSCRE licensing page](https://www.oscre.org/Industry-Data-Model/Licensing-to-Fit-Your-Needs), HACT UK Housing Data Standards and IDM sections | Describes HACT standards as UK social-housing use cases built on OSCRE IDM; distinguishes standards licensing from IDM access/use terms. Exact applicable artefact terms require verification before reproduction/adoption |
| EXT-H07 | [HACT standards catalogue](https://hact.org.uk/tools-and-services/uk-housing-data-standards/) and [HACT Awaab’s Law use case](https://hact.org.uk/tools-and-services/uk-housing-data-standards/awaabs-law-use-case/) | Direct retrieval returned 403; catalogue/dictionary/latest release not read. OSCRE model browser did not expose readable definitions through this access route |

No “latest version 3.5” assumption is made. The inspected GitHub main-branch guidance is mutable, not a controlled approved standards baseline. Before adopting field-level definitions, obtain and pin the exact applicable HACT release/use-case artefacts, identifier paths, code lists and licence, and assess changes.

### 2.3 Approved alignment direction

Treat HACT UK Housing Data Standards as the preferred reference to assess for housing-domain entity and exchange definitions, reusing compatible meanings rather than inventing competing definitions. Mark approved this preferred-reference direction on 5 October under DEC-048. Reuse verified compatible definitions where they fit; document gaps, extensions and justified departures. Exact release/scope/mapping adoption and conformance remain unverified; whole-model adoption is not implied.

AOS common metadata covers organisation scope, evidence status, provenance, time precision, authority/data-use links, uncertainty, accountable outcomes and governed change. Housing payloads can map to an adopted sector standard beneath that common envelope. Actual gaps and extensions are recorded; labels alone cannot establish semantic equivalence.

### 2.4 Concept-level assessment — not verified field mapping

The five named model components below are confirmed by EXT-H04. Their AOS treatment is our proposed engineering interpretation. No exact HACT element names/cardinalities or one-to-one field equivalences are claimed.

| Source concept | Proposed AOS treatment | Required mapping evidence |
| --- | --- | --- |
| Property | Governed asset/place identity with source mappings and hierarchical relationships | Exact property/address/location identifiers, relationship scope and revision |
| Tenant | Person, household and occupancy/tenancy relationships kept distinguishable | Entity/relationship definitions, effective dates, permissions and sensitive-data restrictions |
| Work order | Repair work instruction/status linked to case and evidence | Distinguish instruction/status from verified completion or resident promise |
| Investigation | Report/investigation/evidence relationships | Preserve assessor, observations, event time and uncertainty; no automatic hazard adjudication |
| Appointment | Scheduled/attempted/fulfilled interaction distinct from repair completion | Timing/status codes and evidence of actual occurrence |
| AOS authority, decision, provenance and execution records | Separate common record families linked to mapped payloads | Coverage assessment required; not asserted absent from the whole HACT catalogue |

EXT-H05's illustrative escalation flow is a useful scenario reference. It does not authorise spending, compensation, external contact, health inference or changes to process scope. Data structure and organisational permission remain different.

### DEC-099 — derived-information restriction rule

Every transformation or combination must preserve the applicable restrictions of its contributing sources. The proposed use of the resulting information must satisfy those restrictions and account for any additional sensitive information the combination reveals. If the system cannot establish the lineage or permitted use sufficiently, it must withhold that use and refer the uncertainty for accountable review.

Applies to summaries, aggregates, embeddings/search indexes, joins, exports and restored derived copies within the declared governed scope. Transformation supplies no wider purpose or permission; conflicting restrictions can prevent the proposed combination. A different treatment requires an evidenced authorised determination under the governing rules, never mere notice or developer discretion. Completed disclosures and unreachable external copies remain explicit limitations with accountable handling; no recall or universal forgetting guarantee is made. AOS-03 REQ-011/012 and the existing necessity, explicit-consent, separate-governance and review-cycle conditions are retained; no new personal-inference exception is created.

AOS-02 owns common lineage/restriction record meaning and the scoped transformation inventory; AOS-03 owns the independent operation/purpose-specific permitted-use assessment. Producers supply attributable source/transformation evidence; receiving components must establish the current permission for their intended use. An unresolved case retains its accountable review duty. Exact profile definitions, evidence sufficiency, source-combination rules, permitted transformations, destination inventory and enforceable withdrawal/recovery behaviour must be fixed and assessed before dependent implementation reliance. This decision adds no default policy, wire schema or automatic override.

### DEC-104 — protected reporting under failure and implicated-person interference

Each mandatory protected-finding category shall have an approved reporting arrangement assessed against both technical failure and interference by implicated people. The profile shall identify the intended recipient, possible conflicts and an appropriately independent authorised alternative; an implicated person shall not be the sole gatekeeper deciding whether the required finding reaches its authorised audience.

Authority/use permissions, minimum report content, recipient verification, custody, route/change dependencies, tracking ownership, acceptance, cover and escalation are established in advance. An external route is included where justified and lawfully authorised; external reporting is not a universal default and a finding creates no extra disclosure power. Planned exercises address failed infrastructure, unavailable/implicated recipients, apparent alternatives controlled by the same implicated gatekeeper and attempted suppression. Missing adequate arrangements remain an explicit owned gap, prevent claims of operational protected-reporting assurance and withhold affected dependent reliance under existing gates; they do not create false delivery, ownership transfer or blanket shutdown of separately authorised service. Original tracking duty persists until actual scoped acceptance.

The organisation’s profile binds each required finding class to normal/alternate authorised audiences, conflict criteria/evidence and accountable assessment, disclosure basis/minimal payload, independently verifiable recipients/permissions, credentials/custody and route/reconfiguration controls, failure/compromise assumptions, tracking/cover/escalation, human fallback, evidence and review triggers. Test both infrastructure/common-dependency independence and organisational release/recipient/custody control; neither implies the other. No administrator, executive sign-off or report-validation step may silently remove a required duty. The declared threat/governance scope and residual limitations must be visible: this is not an unlimited guarantee against every holder of legal/constitutional change powers. Inadequacy returns to an empowered accountable reviewer; the reporting agent cannot invent a recipient or grant itself onward-disclosure authority.

## 3. Responsibilities and boundaries

**Responsibility cross-reference (DEC-094; editorial clarification, 29 October 2026):** AOS-14 recognises an exchange-associated obligation and its source/context; the relevant domain steward determines substantive meaning/applicability. AOS-02 owns the common obligation-record semantics and structure/custody. AOS-13 tracks routing, accepted responsibility, fulfilment and unresolved duties. AOS-30 owns the human-workflow meaning of accepted responsibility and supports empowered human disposition/account. These are distinct responsibilities: recognition, record ownership and dispatch do not constitute human acceptance. The existing tracking owner retains the duty until explicit scoped transfer is accepted; failed delivery or exhausted cover does not create an ownerless success. Actual people, cover and response powers remain organisation-appointed prerequisites. No semantic ownership is transferred by this clarification.

| Responsibility | AOS-02 owns | Semantic or institutional owner |
| --- | --- | --- |
| Common record shapes | Envelope, identifiers, reference/time/value-status conventions | Each family has one accountable semantic owner |
| Authoritative source mapping | Record-type/source identity, revisions, mappings and provenance | Organisation/domain steward approves source authority and factual evidence criteria |
| Evidence admission | Structural/provenance/permission-dependent validation result | Admission is not truth verification or an action grant |
| Correction and dispute | Preservation/linking/status and impact notification evidence | Relevant empowered human/domain owner resolves dispute; AOS-01/03 reassess permission |
| Governed query/exchange | Meaning-preserving projections with permission evidence | AOS-03 use/access, AOS-14 external exchange, AOS-01 action authority |
| Outcome records | Correlation of decision/action/consequence/ownership/disposition | AOS-04/13/30 evidence actual effect and responsibility |
| Standard alignment | Versioned mapping and extension/deviation register | Semantic owners approve compatibility; external publisher controls its standard |

Trust boundaries include external ingestion, producer versus admission service, identity reconciliation, source assertion versus inference/decision, human approval, data-use projection, organisation instances and standard-to-local transformation. Technical integration does not erase these boundaries.

### 3.1 Origin and source of assurance — Radical Transparency

Under DEC-046, source provenance answers two different questions: **where did this assertion originate?** and **what provides assurance for treating it as a fact for this use?** A system-of-record designation answers neither automatically.

Proposed assurance metadata links assertion/fact identity and exact evidence revisions; the fact-type source assignment and its approval basis; supporting inspection, measurement, attestation or other approved evidence; validation method/criteria/version; actual validator identity and accountable assurance role; validation time and applicable scope/currentness; result and known limitations. Methods may be human or automated under approved rules. Automated validation retains the rule/tool version and human accountability; a role label alone is not validation evidence.

Unknown or unperformed validation is explicit. A transformed, summarised or projected record retains a governed reference to this assurance chain and its limitations without granting unrestricted access to protected source content. A corrected assurance basis triggers affected dependency review. Historical assurances retain their applicable time/version and cannot be presented as current without the approved currentness checks.

The record supports scrutiny; it does not prove the adequacy of the inspection, method or human judgement. Those need domain criteria and acceptance evidence. Exact fields/cardinalities, evidence sufficiency and disclosure are shared-schema/AOS-03 work.

### 3.1 Component external-research responsibility

Under DEC-086, AOS-02 has an assigned research agent/capability with a controlled profile inheriting AOS-04 v0.7 §§3.1/6.6. Its remit covers external data standards including HACT, provenance/assurance methods, interoperability, record versioning/lineage and data-lifecycle developments relevant to its own function and specification. The accountable component owner owns relevance and substantive implications. External access/source verification follows AOS-14; common evidence/profile/run/finding/disposition views follow AOS-02 v0.7 §6.6. A shared research service may execute the profile, retaining distinct remit, coverage and accountable review. Sources, jurisdictions, cadence/triggers, rubric, recipients/deadlines/cover and appointments remain profile dependencies; no activation or legal finding is claimed. Internal control/record monitoring remains separately specified.

## 4. Capabilities, functions and requirements

### 4.1 Capabilities

All CAP/FUN/REQ identifiers in this document carry prefix AOS-02.

| CAP | Outcome | FUN |
| --- | --- | --- |
| CAP-001 | Governed shared identities, definitions and source mappings | 001/002 |
| CAP-002 | Admitted evidence with provenance, time and uncertainty | 003/004 |
| CAP-003 | Traceable correction, dispute and derived-data lifecycle | 005/006 |
| CAP-004 | Permitted consistent retrieval/exchange | 007/008 |
| CAP-005 | Reconstructable decisions/actions/outcomes | 009 |
| CAP-006 | Controlled standards/schema change and evidence | 010 |
| CAP-007 | Govern shared research evidence, coverage and disposition views, including AOS-02’s own research profile | 011 |


### 4.2 Functions

| FUN | Trigger / input | Behaviour / output | Permission, uncertainty and failure |
| --- | --- | --- | --- |
| 001 | New/changed contract and semantic owner | Register exact definition, owner, applicable profile and compatibility | No local duplicate silently overrides shared meaning |
| 002 | New source/entity mapping or proposed merge/split | Validate organisation/source identity and approved equivalence; record mapping or unresolved relationship | Similar names/addresses are not proof of same person/entity |
| 003 | Producer submits exact evidence revision | Validate accepted schema, typed values, references, provenance and permitted admission; return result | Missing/conflicting mandatory data unresolved/rejected; no invented payload |
| 004 | Time/source/current-state query | Preserve event/receipt/effective meanings; return revision-specific state and limitations | Latest received does not necessarily govern; unavailable not “none exists” |
| 005 | Correction, dispute or supersession | Link previous assertion and basis, preserve relevant history, notify affected consumers | No silent rewriting of completed effects or adjudication by storage layer |
| 006 | Transformation or retention/delete request | Record lineage/restrictions or approved lifecycle outcome | Derived data does not shed purpose; retention and deletion follow reconciled policies |
| 007 | Authorised consumer query | Evaluate use/access dependencies and produce scoped projection with evidence | Reference resolvability does not imply access; withheld/unknown distinguishable |
| 008 | Delivery/replay/reconciliation event | Record admission/delivery acknowledgements and duplicate/order results | No exactly-once guarantee; uncertain delivery remains uncertain |
| 009 | Approved decision/execution/handoff/outcome | Link exact family records without conflating proposal, grant, dispatch, receipt and closure | Human authority and execution evidence supplied by responsible components |
| 010 | Standards/schema/source-map change | Assess version/meaning/compatibility/impact and controlled activation | No silent coercion or automatic external-version adoption |
| 011 | Research profile/run/finding/disposition record | Validate shared research view; preserve exact evidence/baseline, coverage, impact/review and change links | Domain owns implication; admission is not truth, compliance or amendment approval |


### 4.3 Requirement register

All REQs are **proposed**, origin v0.1, 5 October 2026; whole-component logical scope, implementation unapproved. Owner AOS-02 custodian (unassigned); project approver Mark; operational data/retention/source/authority instruments require empowered organisation owners. Category C/I/D denotes component/interface/design constraint. S/E denotes source-derived translation or engineering derivation. Parent REQs refer to proposed AOS-00 v0.12 wording. REQ-001–036 originated in v0.1; REQ-037–046 originate in v0.2, 5 October, with the same proposed status and shared accountability/release metadata. Dependencies and blocking settings are §§6/16/17. VER IDs have prefix AOS-02. Initial change record applies to every row.

| REQ | Proposed obligation | Category / source and rationale | FUN / dependency | VER |
| --- | --- | --- | --- | --- |
| 001 | A shared record contract shall have one controlled definition referenced by its producers and consumers. | I/S; DEC-002, AOS-00-REQ-021; no incompatible copies | 001; ISS-001 | 001 |
| 002 | Each shared contract shall identify one accountable semantic owner. | I/S; DEC-002, REQ-030; meaning has accountable stewardship | 001; ISS-001 | 001 |
| 003 | A record revision shall identify its organisation instance and exact contract revision. | I/E; REQ-035, REC-R01; scoped interoperability | 003; CON-001 | 002 |
| 004 | Each logical record shall have a stable identity distinct from its revision identity. | I/E; QS-03/13, REC-E envelope; correction without ambiguity | 002/003; ISS-002 | 002/006 |
| 005 | Each source-identity mapping shall retain its source-system namespace and source identifier. | I/S; DEC-015, REQ-036; no global-ID assumption | 002; ISS-002 | 003 |
| 006 | An entity equivalence, merge or split shall require the approved reconciliation evidence for that entity type. | C/E; FP6, QS-13; no identity from similarity alone | 002; ISS-002 | 003 |
| 007 | Each record type exchanged with an existing system shall identify its approved authoritative source assignment. | I/S; DEC-015, REQ-036; preserve source ownership | 002/003; ISS-003 | 004 |
| 008 | An evidence revision shall retain the exact accessible source-revision provenance reference. | I/S; RP7 audit principle, REC-R02; reconstruct origin | 003; CON-001 | 004 |
| 009 | A record shall distinguish source observation/assertion, inference, proposal, approved decision and observed outcome. | I/E; FP6, QS-13/19, REC-R03; no status laundering | 003/009; ISS-004 | 005 |
| 010 | Evidence admission shall not certify the source assertion as verified truth. | C/E; REC-E §3, FP6; validity and truth distinct | 003; CON-001 | 005 |
| 011 | Admission shall require validation of mandatory type, cardinality, unit and vocabulary constraints in the accepted profile. | C/E; QS-12, Core Records §2; no implicit coercion | 003; ISS-004 | 005 |
| 012 | A required unavailable value shall not be replaced with an invented default. | C/S; QS-09, FP6; honest absence | 003/004; ISS-004 | 005 |
| 013 | Shared records shall distinguish unknown, unavailable, not applicable and intentionally withheld values. | I/E; Shared Contracts §3; absence is not false/zero | 003/007; ISS-004 | 005/012 |
| 014 | Time metadata shall distinguish source event time, receipt time and effective time. | I/E; REC-E envelope, QS-12; ordering scope | 004; ISS-005 | 007 |
| 015 | Time values shall preserve source precision and their applicable calendar/timezone context. | I/S; DEC-036, REC-E time value; no invented midnight precision | 004; ISS-005 | 007 |
| 016 | A current-state result shall identify the governing revision rule and known material limitations. | I/E; FP6, REC-E §3.2; latest arrival is not governing truth | 004; ISS-003/005 | 007 |
| 017 | A correction shall identify the superseded evidence revision and correction basis. | I/E; QS-13, REC-R04; reconstruct change | 005; CON-001 | 006 |
| 018 | An unresolved dispute shall preserve the conflicting source accounts as distinct evidence. | C/S; DEC-031; no silent winner | 005; ISS-003 | 006/018 |
| 019 | A material correction notification shall identify the changed scope and affected dependency references, including AOS-30 where its preparation, decision account or outcome review materially depends on the changed evidence. | I/E; DEC-029, REC-R08; support selective reassessment | 005; CON-003 | 008 |
| 020 | Correction shall not rewrite the historical record of an already observed effect. | C/S; DEC-029, QS-19; preserve completed history under lifecycle policy | 005/009; ISS-006 | 008/016 |
| 021 | A derived record shall retain its contributing-source transformation lineage and all applicable source-use restrictions, including when sources are combined. | I/S; RP9 cross-layer purpose, REC-R13; DEC-099 approved direction; no laundering through aggregation | 006; CON-003/004 | 009 |
| 022 | A retrieval or disclosure shall require the current AOS-03 determination for its exact purpose and scope. | C/S; REQ-004/040, REC-D; stored availability is not permission | 007; CON-004 | 010 |
| 023 | A reference to a record shall not itself grant access to that record. | C/E; Core Records §2, QS-13; protected references | 007; CON-004 | 010 |
| 024 | A permitted projection shall preserve the meaning, uncertainty and review status of the content it presents. | I/E; REQ-013, Shared Contracts canonical-analysis brief; no misleading redaction | 007; ISS-006 | 012 |
| 025 | A record lifecycle transition shall follow the approved retention, correction, access and deletion policy for its class. | C/S; QS-13; no unlimited evidence retention | 006; ISS-006 | 011 |
| 026 | A same-identity replay with materially different content shall not overwrite the original as a duplicate. | C/E; REC-R05; integrity conflict | 003/008; CON-001 | 013 |
| 027 | Admission, delivery, human acknowledgement and observed effect shall be recorded as distinct event meanings. | I/S; DEC-033, REC-R17/21; sending is not closure | 008/009; CON-005 | 014 |
| 028 | Each consequential action record shall link its trigger, authority version, observed outcome and accountable human role. | I/S; REQ-012, RP7 audit principle; reconstructability | 009; CON-005 | 015 |
| 029 | An unknown execution outcome shall remain distinguishable from known failure and success. | I/S; DEC-030, REC-R18; timeout not proof | 009; CON-005 | 015 |
| 030 | A decision record shall identify decision validity and effective scope, attributable supporting evidence and authentication status, separate minutes-approval status and decision-authority references without treating later minutes approval as universally creating the decision under DEC-103. | I/S; DEC-008/087, REQ-024; Chair draft is not board-approved decision | 009; CON-005 | 016 |
| 031 | A changed schema or mapping shall require an explicit compatibility and cross-component impact assessment before activation. | C/E; QS-03/12/26; no silent semantic change | 010; ISS-001/007 | 017 |
| 032 | An unsupported contract revision shall return an explicit incompatible or unresolved result. | C/E; REC-E header; no silent coercion | 003/010; CON-001 | 017 |
| 033 | An adopted external-standard mapping shall identify its exact standard artefact/version and element locators. | I/E; QS-10/21, EXT-H01–07 assessment; versioned alignment | 010; ISS-007 | 019 |
| 034 | An external-standard transformation shall declare unmapped or materially lossy content. | I/E; QS-12/19; no false equivalence | 003/010; ISS-007 | 019 |
| 035 | A standard-conformance claim shall be limited to its evidenced artefact, scope and tested mapping. | D/E; QS-24/26; reference is not certification | 010; ISS-007 | 019 |
| 036 | Resident-communication evidence shall link the applicable channel-agreement revision and selected channel(s). | I/S; DEC-041, Operational Profiles §6; separate agreement evidence | 009; AOS-03/11/14 | 018 |
| 037 | Automatic entity linking shall require an unambiguous match under the approved entity-type reconciliation rules. | C/S; DEC-045; no name/address-only identity | 002; ISS-002 | 021 |
| 038 | Uncertain matches or potentially destructive entity merges shall require accountable review under the approved reconciliation profile. | C/S; DEC-045; protect distinct source identities | 002; ISS-002 | 021 |
| 039 | Source authority shall be assigned at the fact or record-type scope rather than inferred for every fact held in a source system. | C/S; DEC-046; explicit bounded assurance | 002/004; ISS-003 | 022 |
| 040 | A fact-assurance record shall identify the supporting evidence revision on which the assurance rests. | C/S; DEC-046; Radical Transparency evidence chain | 003/004; CON-001/003 | 022 |
| 041 | A fact-assurance record shall identify the validation method, criteria and relevant version used. | C/S; DEC-046; assertion is not validation | 003/004; ISS-003/004 | 022 |
| 042 | A fact-assurance record shall identify the accountable assurance role and the actual validator identity where validation occurred. | C/S; DEC-046; trace who or what established assurance | 003/004; ISS-003 | 022 |
| 043 | A fact-assurance record shall state known limitations and absent or incomplete validation explicitly. | C/S; DEC-046, FP6; no origin-to-truth shortcut | 003/004; ISS-003 | 022 |
| 044 | Deletion shall not leave a hidden content copy outside the approved record-class lifecycle policy. | C/S; DEC-047; permitted disposition evidence only | 006; ISS-006 | 023 |
| 045 | Housing-data mapping assessment shall prefer verified compatible HACT definitions and record justified departures, extensions or gaps. | C/S; DEC-048; alignment without blanket adoption | 010; ISS-007 | 024 |
| 046 | An unresolved material fact-source conflict shall be referred for accountable human resolution under the approved source profile. | C/S; DEC-046; no latest-arrival winner | 004/005; ISS-003 | 022 |
| 047 | Each component exchange shall reference the common definition, exact revision and profiles allocated to its CON in the Kernel Exchange Register. | I/S; KXR-01/08; DEC-002/065; QS-12/21 | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 025/029 |
| 048 | A receiving exchange shall reject or hold unresolved an unsupported revision unless an explicitly reviewed translation preserves required meaning and restrictions and declares accepted loss. | I/S; KXR-02/07; DEC-065; FP4/6; RP9 | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 025 |
| 049 | Reliance on a fact for a conclusion or action shall evaluate its linked assurance against the required profile for that exact fact revision and intended use. | I/S; KXR-04; DEC-062/063; FP4/6; RP7 | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 026/030 |
| 050 | An exchange acknowledgement shall identify its actually evidenced stage without implying subsequent application, human responsibility or effect. | I/S; KXR-06; DEC-066; RP1; GT M1.13 | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 028 |
| 051 | A checkpoint or later enforcement/effect record shall link to the exact original permission-evaluation revision without rewriting its original result or presenting a pending evidence link as enforcement proof. | I/S; KXR-05; DEC-064; RP7 auditability | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 027 |
| 052 | A fact-assurance exchange shall retain the complete REC-Q chain for the exact fact revision, preserving competing assessments and explicit incomplete status. | I/S; KXR-03; DEC-046/062/063; FP4; RP7 | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 026/030 |
| 053 | A checkpoint evidence record shall retain the exact request, authoritative source revisions, applied version vector and outcome actually checked. | I/S; DEC-067; KCR-01; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 031/032 |
| 054 | An activation record shall distinguish approved change from per-required-dependency applied compatible state. | I/S; DEC-068; KCR-02; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 032 |
| 055 | The common change register shall retain each dependent consumer’s actual application, evidenced no-material-dependency or owned unresolved result. | I/S; DEC-069; KCR-03; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 033/034 |
| 056 | A cumulative accounting record shall preserve approved linked-work scopes, periods, units and cross-agent effect lineage. | I/S; DEC-070; KCR-04; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 035/036 |
| 057 | A reservation record shall preserve the authoritative admission of its complete scope/demand vector without implying a grant of authority. | I/S; DEC-071; KCR-05; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 035 |
| 058 | Accounting history shall preserve confirmed consumption, uncertain reserved exposure and evidence supporting any capacity release. | I/S; DEC-071; KCR-06; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 036 |
| 059 | A withholding record shall preserve notification ownership, acknowledgement/escalation, linked coalesced operations and unresolved delivery or resident-update duties. | I/S; DEC-071; KCR-07; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 037/038 |
| 060 | A resumption record shall identify reconciled prior effects and fresh checkpoint/account evidence without erasing completed history. | I/S; DEC-072; KCR-08; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 034/038 |
| 061 | Common evidence custody shall preserve protected reporting records under separately governed access and assessed technical-failure and implicated-person interference dependencies, without an implicated sole release/custody gatekeeper. | I/S; DEC-073/104; KPR-01; STD-05 CP-8/CP-8(2)/(3), IR-6/IR-8; STD-01/02/03/04 scope alignment | §6.5/§19.4; Protected Reporting and Recovery v0.2; AOS-02-CON-001/003/004/005/006 | 039 |
| 062 | Protected reporting projections shall carry exact bounded permission, recipient-validation and permitted-content evidence without exposing credentials or excess payload. | I/S; DEC-074; KPR-02; STD-05 AC-6; STD-03/04 scope alignment | §6.5/§19.4; Protected Reporting and Recovery v0.1; AOS-02-CON-001/003/004/005/006 | 040 |
| 063 | Handoff records shall distinguish attempted delivery, receipt, validation, responsibility acceptance, escalation and final duty disposition. | I/S; DEC-075; KPR-03; STD-05 IR-6/IR-8; STD-01 scope alignment; AOS-specific acceptance/continuing duty | §6.5/§19.4; Protected Reporting and Recovery v0.1; AOS-02-CON-001/003/004/005/006 | 041 |
| 064 | Recoverable records shall evidence integrity, scope-specific currentness and completeness of withdrawals, restrictions, deletions, approvals and effects/reservations, with gaps explicit. | I/S; DEC-076; KPR-04; STD-05 CP-9/CP-9(1), AU-9; STD-02/03/04 scope alignment; AOS-specific currentness/completeness | §6.5/§19.4; Protected Reporting and Recovery v0.1; AOS-02-CON-001/003/004/005/006 | 042 |
| 065 | Isolated restoration shall apply current lifecycle dispositions to declared copy scope and preserve effect/reservation lineage without hidden deleted payload or erased uncertainty. | I/S; DEC-077; KPR-05; STD-05 CP-10/CP-10(2)/(4)/(6); STD-01/02 scope alignment; AOS-specific current restriction/effect gate | §6.5/§19.4; Protected Reporting and Recovery v0.1; AOS-02-CON-001/003/004/005/006 | 043 |
| 066 | Recovery evidence shall bind source coverage, validation, outstanding duties and exact scoped acceptance/release without treating restoration as case closure. | I/S; DEC-078; KPR-06; STD-05 CP-4/CP-4(4); STD-01/02 scope alignment; AOS-specific release/duty gate | §6.5/§19.4; Protected Reporting and Recovery v0.1; AOS-02-CON-001/003/004/005/006 | 044 |
| 067 | Research-view producers and consumers shall reference one controlled shared definition with explicitly allocated semantic owners. | I/E; DEC-086/002; interoperable research | 011; §6.6/CON-007; AOS-04/domain owners | 045 |
| 068 | Each admitted research finding shall retain exact component/baseline, source/assurance, inference/uncertainty and affected-element links required by its view. | I/E; DEC-086/046; reconstructable implications | 011; §6.6; REC-E/Q | 046 |
| 069 | Research records shall distinguish run coverage, human review disposition, amendment approval and observed application. | I/E; DEC-086; stages cannot be conflated | 011; §6.6; AOS-01/30 | 047 |
| 070 | A material correction to research evidence or its assessed baseline shall notify affected consumers for owned reassessment without silently rewriting historical findings. | C/E; DEC-086/069; currentness with history | 005/011; existing correction/CHG contract | 048 |
| 071 | Research duplicate handling shall preserve each component’s distinct assessment and outstanding review duties. | I/E; DEC-086; shared retrieval is not shared disposition | 008/011; §6.6; AOS-13/04 | 048 |
| 072 | Research projections shall preserve permitted required provenance, coverage and uncertainty while enforcing applicable source/data restrictions. | C/E; DEC-086; evidence with legitimate access | 007/011; AOS-03/14 | 049 |
| 073 | A bounded no-material-finding result shall remain distinct from incomplete, failed or unperformed coverage in stored and disclosed research records. | I/E; DEC-086; honest absence claims | 011; §6.6 | 047/049 |


## 5. State model

Records have orthogonal dimensions rather than one lifecycle status that erases a still-active restriction. Proposed meanings: admission (submitted/validation pending/admitted/restricted admission/rejected/unresolved); currency (current/superseded/disputed); access (permitted/restricted/withheld); retention (retained/deletion pending/deleted under policy); approval (proposal/reviewed/approved/rejected); outcome (known/partial/indeterminate). Exact vocabularies and valid combinations remain schema work.

| Transition | Entry evidence / required authority | Observable result / failure |
| --- | --- | --- |
| Submit → admitted/restricted/rejected/unresolved | Producer identity, accepted profile, admission data-use checks | Exact revision and limitations; admitted does not mean true |
| Current → superseded/corrected | Approved correction evidence and source relationship | Earlier revision/history governed; consumers notified |
| Current assertion → disputed | Identified contradiction/report under profile | Both accounts retained; disputed state does not erase identity or restrictions |
| Record → derived projection | Permitted operation, exact inputs and transformation | New lineage and inherited restrictions; no expanded purpose |
| Retained → restricted/deleted | Approved applicable lifecycle disposition | Policy-consistent deletion/restriction and permitted evidence of disposition |
| Proposed → approved decision record | Human authority/approval supplied by AOS-30/01 | Exact approval scope; no AI-generated transition |
| Pending delivery → confirmed/indeterminate | Actual admission/delivery evidence | Recipient responsibility remains distinct |

Deletion may constrain retained payload/history; do not prescribe perpetual immutable personal data. A permitted minimal disposition reference must not expose deleted information or itself lack a valid retention basis. Actual policy conflicts remain commissioning blockers.

## 6. Semantic contracts and interfaces

### 6.1 Catalogue

CON identifiers carry prefix AOS-02. CON-001 preserves **AOS-02-IF-001 — Evidence exchange**. Other CONs describe component participation; definitive shared IF allocation remains open where absent. Common schemas are the single proposed definitions in Core Records; this component adds obligations and governance, not competing fields.

| Contract | Semantic owner / producers → consumers | Inputs/outputs and controlled definition |
| --- | --- | --- |
| CON-001 / IF-001 | AOS-02; permitted evidence producers → admission/domain/analysis consumers | Exact REC-E revision, provenance, quality, restrictions and admission result; Core Records §§2–3 |
| CON-002 | AOS-02 common structure, domain semantic owner; source steward/adapters ↔ consumers | Entity/source identities, approved source assignment, mapping and equivalence history; profile definitions pending |
| CON-003 | AOS-02 structure and affected semantic owners; correction/derivation service → materially dependent AOS-01/03/04/05/13/21–25/30 | Correction/lineage/dependency changes and impact evidence; REC-E lifecycle with approved correction profile |
| CON-004 | AOS-03 permission semantics; query/projector ↔ identity/data-use/consumers | Exact data/operation/purpose/audience, current REC-D result and permitted projection; AOS-03 v0.3 §6 CON-002/003; exact reciprocal REC-D/schema adoption remains open |
| CON-005 | AOS-01/04/13/20/30 family meanings; controls/workflows → common records/oversight | Authority, execution, canonical analysis, escalation and approved decision records; parent IFs retained |
| CON-006 | AOS-02 with semantic owner; standards/schema registry → adapters/producers/consumers | Exact external artefact, mapping version, extensions/losses, licence assessment and compatibility evidence |

The parent shared catalogue retains AOS-01-IF-001/002, AOS-13-IF-001, AOS-20-IF-001, AOS-30-IF-001 and AOS-14-IF-001. AOS-02 stores common shapes without taking over each family's meaning, authority or approval rights.

### 6.2 Interface semantics and unresolved settings

Every exchange names organisation, accepted contract revision, producer/acting role, subject/source identity and relevant revision/time/causation. Each family declares required/conditional/optional fields, types/units/code lists, valid and invalid values, resolvable references and profile result for missing data.

Admission acknowledgement names exact revision/restrictions. It is distinct from truth verification, recipient responsibility and actual effect. Replayed identical source-event content is handled under the approved duplicate profile; conflicting content is preserved/rejected as conflict. Retry cannot alter meaning, grants or source currency.

Event/effective ordering applies within declared scope. Late events must not silently replace a governing current revision. No universal total order, exactly-once delivery or global clock precision is promised. Required timing, acknowledgement intervals, dependency-propagation limits and outage/recovery settings remain explicit profile fields.

Unsupported schemas/mappings yield incompatible/unresolved results. A lossy transform can proceed only for an approved use that accepts its recorded limitations; loss must not silently erase authority, purpose or material uncertainty. Revoked authority or withdrawn data-use basis is consumed from AOS-01/03; stored records do not confer continued permission.

### 6.3 Reciprocal common-definition adoption, 6 October 2026

AOS-02 adopts [Kernel Exchange Register v0.1](aos-kernel-exchange-register-v0-1.md) §§3–6 at revision 0.1, Core Record Contracts v0.2 and Shared Contracts v0.2 as its single proposed logical definitions. Each local CON retains its identifier and purpose; the register §6 names every produced/consumed family and reciprocal kernel end. No alternative local fields override them. Producers name exact revisions/profiles; receivers validate matching meaning, authorised access and compatibility. Proposed AOS-03-IF-001/REC-D and AOS-04-IF-001/REC-X are catalogue allocations, not schema approval. Required acknowledgement stages and rejection/partial/unresolved responses follow KX-21; actual effect remains REC-X.

DEC-062–066 are approved detailed directions. Organisation role appointments, vocabulary/threshold/unit profiles, executable wire schemas, current-control/propagation and recovery mechanisms, and non-kernel endpoint adoption remain explicit dependencies. Earlier §6 descriptions of pending schema work are resolved only at this common logical level; commissioning and build evidence remain open.

### 6.4 Action-3 reciprocal coordination adoption

AOS-02 adopts [Kernel Control Coordination v0.1](aos-kernel-control-coordination-v0-1.md) §§2–10, Kernel Exchange Register v0.2 and Core/Shared v0.3 as the single proposed logical checkpoint/activation/change/account/reservation/withholding/resume definitions. Original CON IDs remain stable; Register §10 and Control Coordination §9 extend their common family views. Existing §6.3/§19.2 versions identify action-2 history; current declared definition revisions use Register v0.2 §4/§10, never an inferred version conversion.

AOS-01 supplies current authority/restrictions and powers; AOS-03 supplies identity/use/basis/consent; AOS-04 supplies exact task/effect/grouping/demand; AOS-05 gates actual effects and maintains authoritative account/reservation/applied state; AOS-02 supplies common dependency/assurance/account evidence. KX-24 ACC and KX-25 RSV are produced authoritatively by AOS-05 and consumed by AOS-01/02/03/04/05 only within permitted scope; KX-26 WHD is a continuing-duty view from service/execution workflow with AOS-05 blocker evidence, not an automatic notification exemption. Exact dependent CON allocation is the annex §9 table.

Every relevant change tracks receiving application or a reasoned no-material-dependency/owned unresolved result. Withholding creates an accountable separately authorised notification, human responsibility acknowledgement/cover/escalation, traceable coalescing and appropriate resident workflow update through resident-agreed channels. If delivery fails, the duty remains owned. Acknowledged handoff is not service completion. Independent reporting route/current recovered-state proof remain action 4; no claim of delivery capacity here.

### 6.5 Action-4 protected reporting and recovery adoption

AOS-02 adopts [Protected Reporting and Recovery v0.1](aos-kernel-protected-reporting-and-recovery-v0-1.md) §§2–8 as the single proposed logical specification under approved DEC-073–078. Current baseline: AOS-00/Map v0.18; AOS-01–05 v0.6; Core/Shared v0.4; Exchange Register v0.3; Control Coordination v0.2. Existing CON/IF identifiers remain; AOS-02-CON-001/003/004/005/006 consume/produce the annex §5 views. KX-19 protected finding, KX-20 recovery and KX-26 continuing duty use their newly declared revisions in Register v0.3. Older action-2/3 declarations remain historical and require explicit reviewed compatibility, never automatic conversion.

The common envelope, REC-E/A/D/X/Q and CHECK/ACT/CHG/ACC/RSV/WHD remain distinct. Protected reporting adds separately approved route/permission/recipient/custody and human responsibility evidence; recovery adds authoritative currentness/completeness, isolation/reconciliation and scoped empowered release. Custody, technical receipt, system availability and accepted responsibility are different results. Operational role appointments, deadlines, accepted source mechanisms and actual fallbacks remain commissioning dependencies with no invented default.

Annex §7 records dated primary standards references and per-rule provenance. STD-05 control principles are design sources; ISO references are verified edition/scope alignments pending licensed clause verification. AOS approval is not ISO conformance or certification. AOS-specific no-revival, uncertainty retention, agreed resident channels and acknowledged continuing duty are expressly distinguished from standard-derived principles.

### 6.6 Common external-research supporting views

**AOS-02-CON-007**: component research/profile/run/finding/disposition views. AOS-02 owns shared structure; AOS-04 owns common research behaviour/profile semantics, the affected component owns substantive finding meaning and source relevance, AOS-14 owns external exchange/source-verification evidence, AOS-13 owns coordinated handoff and AOS-30 owns empowered human disposition. AOS-01 owns amendment/activation powers. These are local supporting views bound to existing evidence/assurance/execution/analysis/decision/change families, not new approved REC/IF identifiers. This section is the single proposed cross-component logical view definition; AOS-20 v0.1’s GI candidate fields must be reconciled as a domain specialisation, not a competing common schema. Exact wire format, schema revision, catalogue allocation, types/units/cardinalities beyond the logical constraints and reciprocal consumer adoption require reviewed baseline before dependent build. Presence of fields never proves truth or permission.

All views inherit existing organisation/identity/exact revision/provenance, permission, time, lifecycle and staged acknowledgement rules. R = required; C = required when condition applies. References bind exact identities/revisions; unavailable required references leave validation/reliance unresolved. Source access does not imply unrestricted onward disclosure.

| View | Required logical meaning | Ownership / validation |
| --- | --- | --- |
| research_profile | R: component ID and exact assessed specification manifest; remit/questions/topics/jurisdiction; source admission/authority criteria; cadence/triggers; assigned agent/service and accountable component/review/tracking owners; permitted retrieval/tools/use/control references; coverage/currentness/evaluation/materiality/urgency rules; permitted audiences/routes, acknowledgement/deadline/cover/escalation; approval/version/effective/lifecycle references | AOS-04 common meaning, component remit, AOS-01 powers. Required numerical/time/source settings have declared types/units and approval basis; no inferred defaults. Shared agents identify every assigned profile separately. |
| research_run | R: exact profile/baseline/configuration and task/attempt refs; planned/actual execution period; declared coverage scope and actual sources/retrieval results with evidence; complete/partial/failed/cancelled/not-performed condition; finding/no-material-finding-within-coverage/coverage-unresolved result; limitations and owner/follow-up. C: nonperformance/failure reason and missing coverage | AOS-04 run semantics, 14 retrieval evidence. Run completion is not global external completeness or legal compliance. Cancelled/not-performed runs cannot claim complete research. |
| research_finding | R: finding identity/revision, run/profile/component/baseline links; exact source/evidence/assurance refs and publication/event/access/effective dates where known, with explicit unknown/not-applicable reasons; evidence versus inference, relevance/applicability/status, affected CAP/FUN/REQ/CON/source/decision references, materiality/urgency uncertainty, cross-component impacts/owners, recommendation/alternatives or explicit unresolved basis; review/tracking/audience/route and disposition links. C: jurisdiction/proposal/enactment/adoption/effective distinctions for legal/regulatory/standards claims; linked urgent operational response | Component owns substantive meaning, not storage or gateway. Source verification/admission is not organisational adoption. Source and specification version changes link later reassessment, retaining original assessment under governed lifecycle. |
| research_disposition | R: exact finding/proposal revision, empowered reviewer/decision record/powers, observed decision time, accepted-for-further-work/rejected/deferred/unresolved state, rationale/conditions, follow-up owner/deadline or approved no-follow-up basis. C: separate controlled change proposal, amendment approval, verification/release/application/outcome refs when present | AOS-30 decision semantics; AOS-01 powers. Responsibility acceptance and completed follow-up remain distinct. Acceptance for work cannot be rendered as an approved/applied amendment. |

Producers are component research agents and authorised profile/review workflows; consumers are assigned component owners, AOS-13/30, relevant controls and GI where governance implications justify permitted access. Shared retrieval references one source revision with separate component finding/disposition links. Duplicate/coalesced records retain all affected owners/deadlines; conflicting same-identity content is not silently overwritten. Correction/revocation follows existing CHG notifications and governed data lifecycle; storage does not adjudicate substantive validity. Late acknowledgement cannot revive old approval. Privacy/source licensing and retention/delete duties apply to raw documents, summaries and derived records; an unavailable permitted projection exposes the limitation rather than granting more access.


### 6.7 AOS-30 decision-record participation — 7 October 2026

Under DEC-103 and current AOS-30 §§5/6.2/10.3, decision validity/effective time, record authentication/evidence, minutes approval and permission to execute are distinct. Reliance uses sufficient attributable evidence assessed under the actual organisation’s legal form, instruments and approved evidence policy; a valid decision may precede minutes approval. A Chair-authenticated record or extract may be evidence through an authorised route, but no signature, draft or extract alone creates decision authority or resolves conflicting evidence. No universal second approval of exact decision wording is imposed where applicable arrangements do not require it. Minute-taker drafting and Company Secretary stewardship remain distinct; non-board decisions use their applicable empowered route. Current authority/data-use/conditions and observed effects remain separate. Missing or disputed sufficient evidence blocks affected automated reliance for accountable resolution, not a declaration of legal invalidity.

CON-005 stores and projects this approval meaning without upgrading a draft through admission. CON-003 conditionally notifies AOS-30 of material evidence corrections; the shared notification does not itself alter a governing decision. No executable schema change is made; the existing logical KX-06 v0.3 meaning is explicitly adopted. Existing REQ/VER identifiers and proposed/planned statuses are preserved.

## 7. Authority and decision boundaries

AOS-02 can validate and store records only within current permissions. It cannot create an authority grant, resolve an incommensurable-values question or turn an AI proposal into an approved human decision. Source stewardship, semantic ownership, record custody and operational authority are separate powers.

Merge/split, source precedence, evidence resolution, schema change and retention/deletion need named empowered owners and approved rules. Technical administrators cannot silently rewrite governance meaning or remove protected obligations through a data migration.

The boardroom remains outside AI observation/live capture. Only permitted human-authored or human-approved post-meeting records enter. Historical powers and approved revisions are evidenced through AOS-01/30 rather than inferred from a current job title.

A sector standard's vulnerability/contact/occupancy fields are available modelling concepts, not permission to collect, infer or disclose them. HACT alignment does not replace AOS-03 purpose/consent/access controls or determine a welfare exception.

## 8. Reasoning principles applied

### 8.1 FP v4 applicability

| FP | Application / limitation |
| --- | --- |
| 1 Telos/function | Record organisational purpose and software function distinctly; AOS-01/21 govern authoritative purpose |
| 2 Permanent human Mode 2 | Approval/proposal differences and empowered human references; no automated dispute/value adjudication |
| 3 Architectural integrity | Governed meaning, purpose inheritance and auditable interfaces; data convenience cannot remove controls |
| 4 Radical transparency | Provenance/revision/uncertainty/explanation records, with governed disclosure |
| 5 Structural imperfection | Missing, late, duplicate, conflicting and lost events explicitly modelled |
| 6 Epistemic humility | Unknown/unavailable/withheld distinctions; admission is not truth; entity matches require evidence |
| 7 No-exit obligation | Preserve resident accounts and agreement, not silence as approval; AOS-11/30 own contestability |
| 8 Constitutional mediator | Human-approved decision/purpose records, no grant from storage or AI inference |
| 9 Purpose-led design | Shared records derived from governance needs; legal mapping separate, not assumed from data-standard alignment |
| 10 Complexity/emergence | Trace cross-layer derivation and aggregate effects; AOS-25/40 assess system-level behaviour |

### 8.2 RP v6 applicability

| Controlled domain / locator | AOS-02 application and other owners |
| --- | --- |
| 1 “Every governance process must close…” / accountability / “‘AI said so’ test” | REQ-027–030 and causation/accountability records; AOS-13/30 perform tracked handoffs and disposition |
| 1 impossible-option principle | Preserve rejected/impossible option references in canonical analysis records; preparation/rubric owned by AOS-22, not an AOS-02 claim to generate options |
| 2 all Mode 1/2 commitments | Approved parameter/decision provenance; no live boardroom input; AOS-01/25/30 govern review and boundary defence |
| 3 1+5/risk/cross-layer handoff | Shared governed exchange instead of untracked cross-domain copies; domain meaning retained |
| 3 Golden Thread | Versioned building-safety evidence/source accountability supports AOS-10; completeness and verified legal mapping not certified here |
| 4 real-state options/decision feedback/revealed preferences | Evidence currency and structured approved outcomes; revealed preferences remain analytical evidence, not constitutional amendment |
| 5 blind spots/perimeter/emergent behaviour | Limitations and coverage references retained; AOS-14/25 assess perimeter and interactions |
| 6 purpose/ethics/equity/no-exit/compliance | Purpose metadata and disputable evidence; no generic vulnerability or welfare/consent default; professional/board determinations with AOS-03/30 |
| 6 telos/function and accumulated precedent | Founding statements, interpretations and approved amendments distinguished; AOS-21/25 own curation/independent review |
| 6 developer frameworks | Provider/model/configuration lineage permits later divergence assessment; does not itself establish value alignment |
| 7 all three transparency principles | Evidence-backed traceability, explicit uncertainty, approved projections and retention policy |
| 8 all delegation commitments | REC-A/current restriction/delegation trail linked; AOS-01 grants no power from a task; protected audience obligations survive record migration |
| 9 all four purpose/sensing commitments | REQ-021–025; separate asset facts and behavioural inference; no new purpose from cross-layer aggregation |

This assessment covers source applicability and complementary ownership. Exact individual source-item allocations in the controlled traceability matrix remain to be extended; unsupported obligations are not marked complete.

### 8.3 GT applicability

| Tests | Contribution / limit |
| --- | --- |
| M1.1/2/3/5/6/7/8/9/10/11/13/14 | Consistent source/evidence/currentness/outcome records support governance assessment; domain performance, legal compliance and Golden Thread adequacy require their own evidence |
| M1.4/12 | Board capability and self-assessment are institutional matters; AOS-02 can retain permitted evidence but cannot certify conduct |
| M2.1/3/4/7/8/9/10/12/13/14/15 | Purpose/approval/provenance/uncertainty and resident contestability support human assessment; no automated adjudication or value-alignment claim |
| M2.2/5/6/11 | Coherence under pressure, independence, legitimacy and collective judgement require human/longitudinal assessment |

All 29 tests are accounted for at applicability level. No GT pass is claimed, and none justifies observing live board deliberation.

## 9. Data, privacy and disclosure

AOS-02 processes the data necessary for governed admission, identity reconciliation, evidence linkage, permitted query/exchange and accountable outcomes. AOS-03 specifies valid purposes/bases, consent dependencies, access, permitted inference, recipient/role constraints and withdrawal. These decisions govern operation, storage, derivation and projection separately.

Proposed logical families include asset/place, person/household/occupancy relationships, process/case/work item, source/evidence, authority/delegation, data-use determination, analysis, approved human decision, execution/attempt/effect, handoff/disposition and channel agreement. The exact domain models are owned jointly with their relevant semantic owners; this catalogue is not an approved instruction to collect all such data.

Health, vulnerability, person-alert, behavioural or workforce records have specific scope and access requirements. Domain integration cannot turn asset condition into occupancy surveillance, staff-development data into unapproved employment assessment, or resident assistance into enterprise profiling. Standardised fields can remain unpopulated where collection is not approved.

Projection and disclosure minimise exposed content while preserving accurate meaning. Restrictions attach to derived and aggregate data as applicable; access to an aggregate is not automatically safe from identification. Identity maps, provenance and audit records can themselves contain personal data and need approved retention/access controls.

Consent withdrawal invalidates dependent future use under the applicable policy. It does not automatically erase every independently governed retention duty, authorise welfare override or reverse completed disclosure. Deletion/restriction decisions preserve only evidence that their approved policies permit. Under DEC-047, retain only permitted disposition evidence after authorised deletion, not a hidden content copy. Conflicts between accountability and deletion go to the empowered governance/privacy owners. No universal retention duration, blanket UK-only location rule or legal processing basis is adopted.

## 10. Behaviour and workflows

### 10.1 Governed admission and query

Source event → authenticating/permission dependencies → exact contract/version validation → approved source/entity mapping → provenance/time/value-status assessment → admitted/restricted/rejected/unresolved revision → acknowledgement → permitted projection/query → consumer assessment/action → linked outcome.

A receipt error or unknown source identity cannot be repaired by fabricated data. A producer's authority to submit does not give every consumer permission to retrieve. A data-use change before retrieval/disclosure is reassessed at its enforceable control boundary.

### 10.2 Correction, dispute and dependent work

Correction/dispute → exact earlier revision and basis → preserve distinct accounts/history under lifecycle policy → determine affected dependencies → notify consumers → AOS-01/03/04/05/13/21–25/30 reassess materially affected pending work within their responsibilities → accountable review of significant completed consequences → permitted updated evidence/disposition.

No blanket freeze of unrelated work. No storage-layer selection of a convenient winner. An approved source assignment is specific to a fact/record type. It retains the source of assurance and cannot by itself dispose of a material dispute. Under DEC-046, unresolved material conflicts are referred for accountable human resolution; later arrival does not automatically govern.

### 10.3 Standard mapping and change

Proposed external artefact/version → verify access/terms and source status → compare entity/field/code-list/time meanings → record direct/conditional/lossy/unmapped relationships → semantic owner/consumer impact review → approved mapping/profile → controlled deployment → round-trip/loss/effect tests → preserved previous mapping/version and review evidence.

HACT use cases are assessed individually; a supplier's broad “HACT compatible” statement is not mapping evidence. Migrating a database or accepting a new code list does not activate organisational authority or new processing purposes.

### 10.4 Decision and action feedback

Human-approved decision or execution event → exact approval/instrument reference → capture trigger/context/output/limitations → retain attempt/effect/handoff evidence → link disposition → make permitted evidence available to AOS-21/25/30 review.

Do not generate missing human rationale after the event and present it as contemporaneous evidence. Human approval, recipient acknowledgement and actual effect remain separate.

### 10.6 Combined control coordination

For effects, activation, material changes, concurrent reservations, withholding and resumption, apply the common protocol in Control Coordination v0.1 §§3–8. Denial or missing current controls/accounting withholds dependent work; actual application and responsibility are separately evidenced. Timeouts/cancellations do not establish no prior effect or release uncertain capacity. Numeric/profile/role selections remain commissioning dependencies.

### 10.7 Protected reporting and controlled recovery

Apply Protected Reporting and Recovery v0.1 §§3–4: withhold dependent effects, attempt only permitted reporting, retain original tracking owner until accepted handoff and preserve unresolved failure duties. Restore in isolation; prove required authoritative current state and complete material changes, apply current dispositions and reconcile effects/reservations. Only scoped accepted release can restore operation, followed by fresh current CHECK and capacity admission; no automatic queue replay. Unaffected release requires evidence of no material dependency, not mere absence of a known incident.

### 10.8 External research evidence and review

Approved component research profile and exact baseline → permitted external retrieval through AOS-14 → source/provenance/date/applicability evidence → component assessment of relevance and affected requirements/functions/contracts → finding or bounded no-material-finding/coverage-gap result → authorised recipient and accountable handoff → recorded human disposition → controlled change candidate if accepted → required approval, verification, compatible activation and outcome follow-up. Urgent operational/legal/safety implications use their separately authorised response route while specification change remains pending; a research finding supplies no emergency power. One retrieved source may feed several permitted component assessments; each preserves its own implications, review duties and disposition.

## 11. Failure, escalation and recovery

| Failure | Behaviour / accountable dependency |
| --- | --- |
| Unsupported or invalid schema/code/unit | Reject or return unresolved/incompatible under profile; preserve permitted diagnostic and source reference |
| Missing/stale source or ambiguous entity match | Surface limitation; hold dependent matching/use; steward/human route |
| Conflicting account or changed payload under duplicate identity | Preserve distinct contradiction; no overwrite; accountable source/domain resolution |
| Late/out-of-order event | Recompute governing revision under approved time/source rules; do not equate arrival with effectiveness |
| AOS-03 or authority dependency unavailable | Withhold dependent operation/disclosure; separately authorised fallback only |
| Partial delivery or missing acknowledgement | Indeterminate delivery/admission distinguished; query/reconcile before repeat where effect matters |
| Missing required audit/pre-effect record | Dependent action remains blocked at responsible executor boundary unless valid approved fallback exists |
| Migration drops restrictions/provenance | Incompatible/failed migration; do not activate affected consumers; preserve authorised rollback evidence |
| Retention and required evidence conflict | Refer to empowered data/privacy/governance owners; no implicit perpetual retention or erasure priority |
| Compromised/unauthorised source or namespace | Quarantine/reject only under approved incident/admission rights; no unrestricted incident repository |
| Store/index/cache outage | Declare unavailable/stale boundary and dependent capability; no false empty result |
| Recovery restores older state | Reconcile current revisions/restrictions/decisions before dependent operation; no permission resurrection |

Exact recovery, replication, reconciliation and manual operating capacity belong with AOS-05 and the approved profiles. No universal exactly-once, zero-loss, always-current or unbreakable-store claim is made.

## 12. Evidence, provenance and audit

Each relevant record chain exposes trigger → source revision → actor/producer → permitted purpose/authority → transformation/rule/model/configuration where applicable → record/admission result → downstream request/action → actual effect/uncertainty → human intervention → disposition.

Capture actual input/rule/output and approved human rationale. Do not demand private model chain-of-thought. Record changes, failed admission, deliberate withholding, migration/mapping versions, loss limitations and unresolved references. Audit projections are governed, not a bypass around AOS-03.

AOS-02 owns common evidence identity/shape and storage lifecycle, while the event's semantic owner owns what it proves. A delivery log proves attempted/confirmed delivery only to its evidenced extent, not substantive receipt, judgement or repair completion.

## 13. Security and operational requirements

Instance scope, data classification and current operation-specific permissions apply to record payload, indexes, search, provenance, exports, backups and derived views. Identifier leakage and relationship traversal are assessed as disclosures. Credentials/secrets are not copied into common envelopes.

AOS-05 must define tamper-detection/protection, backup, recovery, migration/rollback, availability, query freshness and capacity boundaries. Evidence versioning does not mandate one storage architecture or indefinite append-only personal data. Replicas and caches must expose their actual currentness constraints.

Admission/type/time validation must be distinguishable from probabilistic entity matching or evidence interpretation. Where matching/model transformation is used, define allowed task/output, uncertain result, human review, test data/rubric/thresholds and model-change impact. No self-reported confidence or fuzzy score is treated as proven identity.

Profiles require approved values for permitted operations, entity reconciliation, quality/currency limits, admission/query timing, duplicate windows, clock uncertainty, mapping compatibility, retention and recovery. Missing required settings block the dependent capability; there are no numerical defaults in this draft.

Human data stewardship, explanation access and correction/challenge processes need accessible formats and feasible operating cover with AOS-30/05. Technical performance cannot substitute for accountable correction handling.

## 14. Invariants

INV identifiers have prefix AOS-02. They restate listed proposed requirements rather than add unrecorded obligations.

| INV | Meaning | REQ / VER |
| --- | --- | --- |
| INV-001 | Shared meaning has one controlled definition and semantic owner | 001/002; 001 |
| INV-002 | Admission is not truth, permission or human approval | 009/010/022/030; 005/010/016 |
| INV-003 | Correction preserves accountable historical meaning within approved lifecycle | 017–020/025; 006/008/011 |
| INV-004 | Derived data does not shed applicable purpose restrictions | 021/022; 009/010 |
| INV-005 | Latest arrival is not necessarily current governing fact | 014–016; 007 |
| INV-006 | Delivery, responsibility and effect are distinct | 027–029; 014/015 |
| INV-007 | Standard alignment is versioned and evidenced, not inferred from a label | 031–035; 017/019 |
| INV-008 | Agreed resident-channel evidence is distinct from organisational permission | 036/022; 010/018 |
| INV-009 | Research coverage/disposition cannot be represented as compliance or amendment approval | 068/069/073; 046/047 |


## 15. Conformance and acceptance

### 15.1 Criteria

CR identifiers have prefix AOS-02; all criteria are proposed.

| CR | Claim requiring evidence | REQ / verification |
| --- | --- | --- |
| CR-001 | Controlled shared semantics, identity and sources | 001–008/037–043/046; VER-001–004/021/022 |
| CR-002 | Honest evidence, time and correction meaning | 009–020/026; VER-005–008/013 |
| CR-003 | Governed derivation, privacy and lifecycle | 021–025/036/044; VER-009–012/018/023 |
| CR-004 | Reconstructable approval/delivery/effect | 027–030; VER-014–016 |
| CR-005 | Controlled schema/standards compatibility | 031–035/045; VER-017/019/024 |
| CR-006 | Adequate behaviour across contexts and recovery | Relevant whole allocation; VER-020 and scenario matrix |

### Explicit conformance navigation — 29 October 2026

This index completes the documentary navigation from every retained kernel requirement to its proposed conformance criterion and its existing planned case(s). It neither adds a requirement nor claims that a case was executed or that its coverage is adequate. CR-EXCHANGE, CR-COORDINATION, CR-CONTINUITY and CR-RESEARCH below are derived grouping labels local to this component, not new system obligations. Original numbered CR claims remain applicable with their stated scope and limitations. Exact requirement text in §4.3 and case definitions in §15 remain authoritative.

| Derived criterion | Existing obligation family / derivation |
| --- | --- |
| CR-EXCHANGE | Common definition/revision, compatibility, assurance and staged evidence adoption; existing §19.2 allocation. |
| CR-COORDINATION | Current checkpoint, compatible activation, change propagation, cumulative accounting and owned withholding/resumption; existing §19.3 allocation. |
| CR-CONTINUITY | Protected reporting, accepted human duty and current-state recovery/release; existing §19.4 allocation. |
| CR-RESEARCH | Controlled research, evidence/coverage, human review and separate amendment authority; existing research requirements and their allocation. |

| Requirement | Proposed criterion (AOS-02 prefix) | Existing planned case(s) | Derivation / applicability |
| --- | --- | --- | --- |
| AOS-02-REQ-001 | CR-001 | AOS-02-VER-001 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-002 | CR-001 | AOS-02-VER-001 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-003 | CR-001 | AOS-02-VER-002 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-004 | CR-001 | AOS-02-VER-002, AOS-02-VER-006 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-005 | CR-001 | AOS-02-VER-003 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-006 | CR-001 | AOS-02-VER-003 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-007 | CR-001 | AOS-02-VER-004 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-008 | CR-001 | AOS-02-VER-004 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-009 | CR-002 | AOS-02-VER-005 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-010 | CR-002 | AOS-02-VER-005 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-011 | CR-002 | AOS-02-VER-005 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-012 | CR-002 | AOS-02-VER-005 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-013 | CR-002 | AOS-02-VER-005, AOS-02-VER-012 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-014 | CR-002 | AOS-02-VER-007 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-015 | CR-002 | AOS-02-VER-007 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-016 | CR-002 | AOS-02-VER-007 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-017 | CR-002 | AOS-02-VER-006 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-018 | CR-002 | AOS-02-VER-006, AOS-02-VER-018 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-019 | CR-002 | AOS-02-VER-008 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-020 | CR-002 | AOS-02-VER-008, AOS-02-VER-016 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-021 | CR-003 | AOS-02-VER-009 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-022 | CR-003 | AOS-02-VER-010 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-023 | CR-003 | AOS-02-VER-010 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-024 | CR-003 | AOS-02-VER-012 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-025 | CR-003 | AOS-02-VER-011 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-026 | CR-002 | AOS-02-VER-013 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-027 | CR-004 | AOS-02-VER-014 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-028 | CR-004 | AOS-02-VER-015 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-029 | CR-004 | AOS-02-VER-015 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-030 | CR-004 | AOS-02-VER-016 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-031 | CR-005 | AOS-02-VER-017 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-032 | CR-005 | AOS-02-VER-017 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-033 | CR-005 | AOS-02-VER-019 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-034 | CR-005 | AOS-02-VER-019 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-035 | CR-005 | AOS-02-VER-019 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-036 | CR-003 | AOS-02-VER-018 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-037 | CR-001 | AOS-02-VER-021 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-038 | CR-001 | AOS-02-VER-021 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-039 | CR-001 | AOS-02-VER-022 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-040 | CR-001 | AOS-02-VER-022 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-041 | CR-001 | AOS-02-VER-022 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-042 | CR-001 | AOS-02-VER-022 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-043 | CR-001 | AOS-02-VER-022 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-044 | CR-003 | AOS-02-VER-023 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-045 | CR-005 | AOS-02-VER-024 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-046 | CR-001 | AOS-02-VER-022 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-02-REQ-047 | CR-EXCHANGE | AOS-02-VER-025, AOS-02-VER-029 | Existing common exchange and assurance/evidence obligation. |
| AOS-02-REQ-048 | CR-EXCHANGE | AOS-02-VER-025 | Existing common exchange and assurance/evidence obligation. |
| AOS-02-REQ-049 | CR-EXCHANGE | AOS-02-VER-026, AOS-02-VER-030 | Existing common exchange and assurance/evidence obligation. |
| AOS-02-REQ-050 | CR-EXCHANGE | AOS-02-VER-028 | Existing common exchange and assurance/evidence obligation. |
| AOS-02-REQ-051 | CR-EXCHANGE | AOS-02-VER-027 | Existing common exchange and assurance/evidence obligation. |
| AOS-02-REQ-052 | CR-EXCHANGE | AOS-02-VER-026, AOS-02-VER-030 | Existing common exchange and assurance/evidence obligation. |
| AOS-02-REQ-053 | CR-COORDINATION | AOS-02-VER-031, AOS-02-VER-032 | Existing coordinated current-control/effect/duty obligation. |
| AOS-02-REQ-054 | CR-COORDINATION | AOS-02-VER-032 | Existing coordinated current-control/effect/duty obligation. |
| AOS-02-REQ-055 | CR-COORDINATION | AOS-02-VER-033, AOS-02-VER-034 | Existing coordinated current-control/effect/duty obligation. |
| AOS-02-REQ-056 | CR-COORDINATION | AOS-02-VER-035, AOS-02-VER-036 | Existing coordinated current-control/effect/duty obligation. |
| AOS-02-REQ-057 | CR-COORDINATION | AOS-02-VER-035 | Existing coordinated current-control/effect/duty obligation. |
| AOS-02-REQ-058 | CR-COORDINATION | AOS-02-VER-036 | Existing coordinated current-control/effect/duty obligation. |
| AOS-02-REQ-059 | CR-COORDINATION | AOS-02-VER-037, AOS-02-VER-038 | Existing coordinated current-control/effect/duty obligation. |
| AOS-02-REQ-060 | CR-COORDINATION | AOS-02-VER-034, AOS-02-VER-038 | Existing coordinated current-control/effect/duty obligation. |
| AOS-02-REQ-061 | CR-CONTINUITY | AOS-02-VER-039 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-02-REQ-062 | CR-CONTINUITY | AOS-02-VER-040 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-02-REQ-063 | CR-CONTINUITY | AOS-02-VER-041 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-02-REQ-064 | CR-CONTINUITY | AOS-02-VER-042 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-02-REQ-065 | CR-CONTINUITY | AOS-02-VER-043 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-02-REQ-066 | CR-CONTINUITY | AOS-02-VER-044 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-02-REQ-067 | CR-RESEARCH | AOS-02-VER-045 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-02-REQ-068 | CR-RESEARCH | AOS-02-VER-046 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-02-REQ-069 | CR-RESEARCH | AOS-02-VER-047 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-02-REQ-070 | CR-RESEARCH | AOS-02-VER-048 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-02-REQ-071 | CR-RESEARCH | AOS-02-VER-048 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-02-REQ-072 | CR-RESEARCH | AOS-02-VER-049 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-02-REQ-073 | CR-RESEARCH | AOS-02-VER-047, AOS-02-VER-049 | Existing research obligation; assessment remains distinct from amendment/activation. |

### 15.2 Planned verification register

All cases have prefix AOS-02-VER and status **planned, not executed**. Shared preconditions: fixed source/specification/contract/profile manifest; isolated synthetic environment; approved fixtures and test identities; no live personal data or external effects. Required unavailable configuration yields not assessed. Inspect every relevant in-scope record/mapping/path; no undisclosed sample.

Method: structured inspection plus test/demonstration when implemented. Assessor roles: AOS-40 data/integration reviewer; semantic/source steward for factual definitions; AOS-03 privacy reviewer; governance reviewer for approvals. Appointments unresolved. Preserve exact tested revisions, inputs, outputs, limitations and assessment evidence. Institutional quality needs separately defined human review; software results cannot establish it alone.

| VER | REQ | Procedure / challenge | Expected result and retained evidence |
| --- | --- | --- | --- |
| 001 | 001/002 | Producer/consumer use competing definitions or missing owner | Incompatibility/vacancy exposed; one controlled reference and owner required before dependent adoption |
| 002 | 003/004 | Same record identity across instances or materially revised payload | Instance/revision distinction enforced; no silent cross-instance join or overwritten revision |
| 003 | 005/006 | Similar person names/address; namespace collision; merge then split | Source namespace retained; similarity alone not equivalence; approved relationship evidence/history required |
| 004 | 007/008 | Source substitution, absent source assignment and missing provenance revision | Source authority/reference gaps explicit; no unsupported current-fact claim |
| 005 | 009–013 | Inference labelled fact; malformed unit; unknown/withheld value; invented default | Meaning/status/validation distinctions preserved; missing required value not invented; admission not truth |
| 006 | 017/018/004 | Contractor update contradicts resident account; approved correction | Both assertions and correction links retained under policy; no silent overwrite |
| 007 | 014–016 | Date-only/precise times, late effective record, stale view/query outage | Source precision and time roles preserved; governing revision rule/limitations surfaced; outage not false absence |
| 008 | 019/020 | Correct material input affecting pending and completed actions | Dependent references notified, including AOS-30 for affected preparation/account/outcome review; GI revises canonical analysis and AOS-30 obtains human review; affected work reassessed by responsible controls; completed effects remain historical |
| 009 | 021 | Transform restricted sources into a summary, aggregate, embedding/search index, joined view, export and restored copy; try a wider purpose, incompatible source restrictions, missing lineage and a combination revealing additional sensitive information. | All applicable contributing-source restrictions and attributable lineage retained; transformation grants no wider use. Additional sensitive disclosure is identified for AOS-03 assessment; incompatible or insufficiently evidenced use withheld and referred with an owner. Exercise an evidenced authorised different treatment under existing rules and reject an unsupported override. Completed disclosures/unreachable copies retain explicit limitations and accountable handling. Planned, not executed. |
| 010 | 022/023 | Retrieve via known ID or authority allow without valid data use | Operation-scoped access required; reference/action permission alone insufficient; denied content not leaked |
| 011 | 025 | Conflicting retention/deletion needs and authorised lifecycle disposition | Unresolved conflict referred; approved restriction/deletion follows exact policy; only permitted residual evidence retained |
| 012 | 013/024 | Redact source/uncertainty/approval state in an otherwise permitted projection | Withheld versus absent distinguished; projection does not falsely imply certainty or approval |
| 013 | 026 | Same event/content replay; same identity with changed material content | Approved deduplication for first; conflict preserved for second; no destructive overwrite |
| 014 | 027 | Admitted record, dispatched notification, delivered message and human acceptance | Distinct evidence/states; dispatch/delivery do not close accountable handoff |
| 015 | 028/029 | Partial/unknown effect and consequential repeat | Trigger/authority/accountable role/outcome linked; indeterminate not converted to failure; responsible executor reconciles repeat |
| 016 | 030/020 | Valid decision with minutes pending; authorised authenticated record/extract; signature without a real decision; contradicted signed minutes; later correction or changed decision. | Four axes and actual times retained. Valid decision plus sufficient policy-assessed evidence may support reliance before minutes approval; unsupported/contradicted evidence withholds affected reliance for human resolution. Required governing conditions and current controls still apply; later correction cannot silently backdate, erase or fabricate decision/effect. Planned, not executed. |
| 017 | 031/032 | Unsupported schema and materially changed mapping/code meaning | Explicit incompatibility; approved impact/compatibility assessment before affected activation |
| 018 | 036/018 | Changed resident-channel agreement, unavailable channel and disputed completion | Exact agreement/selected channel evidence linked; relevant sends reassessed; no unagreed substitution or deletion of dispute |
| 019 | 033–035 | Candidate HACT mapping with pinned artefacts, missing fields, lossy statuses and unsupported conformance claim | Exact mapping/version/limitations recorded; no claim beyond tested scope; unsupported semantics not silently coerced |
| 020 | relevant whole allocation | Execute contrasting scenario review and restore/migrate stale/restricted records | Meaning/permissions/currentness/history preserved to approved scope; gaps recorded as source-grounded issues; no universal rule inferred from one process |
| 021 | 037/038/005/006 | Ambiguous names/address, approved unambiguous identifier rules, potentially destructive merge and split | No similarity-only identity; automatic link only within approved rule; uncertain/destructive operation requires accountable review; source identities/history retained |
| 022 | 039–043/046/007/008/016/018 | One system authoritative for different fact types; missing supporting evidence; validation contradicted or stale; unresolved material conflict | Fact-type assignment explicit; origin separate from assurance evidence/method/version/validator/accountability/limitations; missing validation visible; conflict routed to authorised human without latest-arrival shortcut |
| 023 | 044/025 | Approved deletion; attempt hidden archive/shadow content copy; independently permitted disposition metadata | No unauthorised retained content; only policy-permitted disposition evidence remains; unresolved policy conflict referred to empowered owners |
| 024 | 045/033–035 | Compatible verified HACT definition; unsuitable/missing definition; candidate extension/version change | Compatible meaning preferred; gaps/extensions/departures justified; exact release/scope/elements/losses/tests recorded; no blanket adoption or unsupported conformance |
| 025 | 047/048 | Definition/version compatibility; inspect/test exact approved synthetic fixture and definition revisions | KXV-01: supported, unsupported and accepted translated records; original and translation retained, restricted meaning preserved, declared loss suitable for use. Planned, not executed. |
| 026 | 049/052 | Assurance status and exact fact binding; inspect/test exact approved synthetic fixture and definition revisions | KXV-02: multiple incomplete/disputed/purpose-bounded assessments; preserve all chains and disagreements; no admission-to-truth or new-revision validation shortcut. Planned, not executed. |
| 027 | 051 | Original evaluation and later effects; inspect/test exact approved synthetic fixture and definition revisions | KXV-03: permit/deny before effect, later checkpoint/withheld/effect links; original decision reconstructable, absent evidence never proof of enforcement. Planned, not executed. |
| 028 | 050 | Acknowledgement stages; inspect/test exact approved synthetic fixture and definition revisions | KXV-04: delivery without application/responsibility; no false completion; pure information requires no invented human acknowledgement. Planned, not executed. |
| 029 | 047 | Reciprocal CON walkthrough; inspect/test exact approved synthetic fixture and definition revisions | KXV-05: inspect every component CON against the same producer/consumer definitions, field/status/units/ack manifest; retain mismatches and non-kernel dependencies. Planned, not executed. |
| 030 | 049/052 | Restricted assurance projection; inspect/test exact approved synthetic fixture and definition revisions | KXV-06: permitted projection preserves required assurance substance; unavailable material evidence leaves reliance unresolved; no privacy bypass. Planned, not executed. |
| 031 | 053 | KCV-01: Exact checkpoint and restriction race; inspect/test exact authorised synthetic fixture and versions | Substitute arguments/current evidence and restrict before/after last enforceable point; affected pre-boundary effect blocked, irreversible crossing and uncertainty/follow-up evidenced. Planned, not executed. |
| 032 | 053/054 | KCV-02: Partial compatible activation; inspect/test exact authorised synthetic fixture and versions | Wrong/old/missing required applied member and restriction during rollout; affected path withheld, compatible unaffected scope evidenced, no approval-to-activation shortcut. Planned, not executed. |
| 033 | 055 | KCV-03: Change receipt versus application; inspect/test exact authorised synthetic fixture and versions | Duplicate/conflicting/out-of-order notices and missing consumer; actual applied/no-material-dependency basis or owned unresolved cover/escalation; old permission not revived. Planned, not executed. |
| 034 | 055/060 | KCV-04: Selective impact and restart; inspect/test exact authorised synthetic fixture and versions | Correct pending input and significant completed consequence; reassess affected work, preserve history and owner review, no replay on restart. Planned, not executed. |
| 035 | 056/057 | KCV-05: Concurrent overlapping capacity; inspect/test exact authorised synthetic fixture and versions | Parallel workers request same remaining allowance across multiple scopes and provider switch; no partial grant, double spend or account reset evasion; exact authoritative evidence. Planned, not executed. |
| 036 | 056/058 | KCV-06: Partial/unknown reservation; inspect/test exact authorised synthetic fixture and versions | Expire/cancel/failover after possible effect and cross period boundary; confirmed quantity consumed, uncertain remainder held, release only evidenced unused quantity. Planned, not executed. |
| 037 | 059 | KCV-07: Withheld duty notification; inspect/test exact authorised synthetic fixture and versions | Accounting/control unavailable, missing acknowledgement, failed route and coalesced repeats; dependent work blocked, separate permitted notification and accountable delivery exception/cover; every operation traceable. Planned, not executed. |
| 038 | 059/060 | KCV-08: Resident update and controlled resume; inspect/test exact authorised synthetic fixture and versions | Service affected with acknowledgement but unresolved task, unagreed channel and sensitive content, then premature resume; only permitted agreed-channel update, contact duty visible, no replay without current reconciled evidence/approval. Planned, not executed. |
| 039 | 061 | KPV-01 / DEC-104: approved finding-class profile; primary controls/reporting failure plus implicated or suppressing normal recipient/release controller; false alternative sharing technical dependency or implicated sole gatekeeper; valid authorised independent alternative. | The component supplies its assigned authority/record/use/task/runtime evidence for both technical and organisational independence. No implicated sole release gate; no assumed independence from an alternate address alone. Use only pre-authorised verified minimal-content routes; inadequate arrangements remain owned, block protected-reporting assurance/affected dependent reliance and preserve tracking/service duties. Inspect actual alternate attempt, custody/control, recipient and acceptance evidence; no external-disclosure default. Planned, not executed. |
| 040 | 062 | KPV-02: Reporting permission and recipient invalid; authorised synthetic fixture, exact profile and source revisions | Expired/wrong-scope advance permission, unverified recipient or excessive content; refuse unauthorised payload, retain minimal permitted fallback if valid, otherwise owned unresolved duty; no emergency grant. Planned, not executed. |
| 041 | 063 | KPV-03: No human accepts and fallback also fails; authorised synthetic fixture, exact profile and source revisions | Receipt without responsibility acceptance, absent cover, escalation failure and repeated linked reports; original tracking owner persists, all affected work traceable, approved human fallback/owned exception and resident-channel duty remain visible. Planned, not executed. |
| 042 | 064 | KPV-04: Protected backup is stale or incomplete; authorised synthetic fixture, exact profile and source revisions | Valid integrity check but omitted withdrawal/consent/deletion/change or uncertain source coverage; dependent release blocked until scope-specific currentness and completeness are established from authoritative evidence. Planned, not executed. |
| 043 | 065 | KPV-05: Restore contains old permission and uncertain effects; authorised synthetic fixture, exact profile and source revisions | Isolated old snapshot with deleted/restricted payload, completed/partial/unknown effects, uncertain reservation and incompatible config; no normal effects, apply dispositions and reconcile exposure, no repeated known effect or hidden retained payload. Planned, not executed. |
| 044 | 066 | KPV-06: Premature selective release under compound failure; authorised synthetic fixture, exact profile and source revisions | Combine compromise, incomplete current-state evidence, outstanding handoff and provider failover; reject unsupported automatic/human release, accept only evidenced approved unaffected scope, preserve unresolved duties and require fresh CHECK/reservation for continuation. Planned, not executed. |
| 045 | 067 | Producer/consumer walkthrough of four research views using exact synthetic schema/profile revisions | Same authoritative structure and semantic owners; unsupported fields/versions and absent mandatory references rejected/unresolved. Planned, not executed. |
| 046 | 068 | Evidence-backed versus unsupported finding, disputed assurance, future rule and stale component baseline | Source/assurance/date/status/applicability, evidence/inference and affected element links retained with uncertainty; admission is not validation. Planned, not executed. |
| 047 | 069/073 | Complete no-finding, partial/failed/skipped research; candidate accepted but amendment not approved | Coverage and review/change/application states remain distinct in queries and presentation; no false completion. Planned, not executed. |
| 048 | 070/071 | Correct source and change baseline after two component findings; replay/coalesce with different deadlines | Historical findings preserved; each affected consumer/owner receives tracked reassessment and duties survive deduplication. Planned, not executed. |
| 049 | 072/073 | Restricted source/assurance projection with missing material evidence and failed coverage | Only permitted payload disclosed; required uncertainty/coverage survives projection or reliance remains unresolved; no access bypass. Planned, not executed. |



### 15.3 Contrasting scenario matrix

| Scenario | General model tested | Local/profile dependency |
| --- | --- | --- |
| Overdue repair | Resident promise versus internal target; disputed/partial/unverified completion; exact evidence and agreed channels | DEC-031–041 scoped rules; factual evidence/time/channel profiles |
| Property inspection and hazard case | Asset/place/investigation/work-order links; uncertain evidence and approved restrictions | HACT-related concept mapping; verified sector release and independent legal/process assessment |
| Procurement commitment | Supplier/source identity, quantity/currency/time meaning, approval and actual commitment outcome | Finance source/approval profiles; no spending right created by records |
| People development/employment | Person/role/context relationships, purpose inheritance and sensitive correction | AOS-03/12 approved purposes and employment authority; no generic staff profiling |
| Constitutional amendment | Draft/review/approved/effective versions and board-body powers | AOS-01/30 exact-version/sequence evidence; interpretations not authority |
| External exchange and cross-domain insight | Recipient/principal/source provenance, data-use projection, duplicate/unknown outcomes | AOS-03/14 trust/use controls; no assumed federation or aggregate safety |

## 16. Dependencies

| Stage | Required dependencies |
| --- | --- |
| Drafting | Governed sources/architecture, common contracts, AOS-01 and researched HACT references |
| Component baseline | Exact shared envelope/family schemas, type/unit/status/reference rules, appointed semantic stewardship, source allocation and resolved material design questions |
| Build | AOS-03/04/05 contracts; fixed domain source/maps/profiles; approved fixtures; control/retention/evidence boundaries; accepted cases and bounded release |
| Standards adoption | Exact HACT/other artefacts/releases/code lists/terms, controlled field-level mapping, domain approval and conformance evidence |
| Activation | Valid organisation permissions, source ownership, steward/operational cover, approved data lifecycle/location/identity rules and compatible deployed consumers |
| Operation | Current restrictions/revisions, source/quality monitoring, accessible correction/query routes, recovery and ongoing assurance |

No draft interoperability mapping supplies a lawful data-sharing arrangement or an institutional appointment.

## 17. Issues and decisions required

ISS IDs have prefix AOS-02. Detailed dependencies remain open; the four submitted general-data directions are resolved under DEC-045–048. Shared owner appointments remain unresolved. “Decision required” denotes a material design choice to refer, not permission for a builder to invent an answer.

| ISS | Type / question and source | Affected / owner | Required evidence / gate |
| --- | --- | --- | --- |
| 001 | Dependency: contract ownership appointments, change procedure and compatibility; DEC-002/P01 | FUN-001/010; AOS-02 and semantic owners | Controlled registry/review process; component baseline/build |
| 002 | Design choice: entity namespace/equivalence/merge-split implementation and role settings; DEC-045 settles matching/review direction, FP6 | FUN-002; AOS-02/domain/privacy owners | Approved matching/relationship rules and disputed-identity handling; build |
| 003 | Design choice: fact-type source/assurance assignments and current-fact profile implementation; DEC-046 settles conflict/assurance direction, DEC-015/031 | FUN-002/004/005; source/domain stewards | Record-type source profiles and human resolution powers; activation |
| 004 | Design gap: final common envelope/family schemas, value-status, type/unit/cardinality/vocabulary | CON-001–005; AOS-02 with semantic owners | Executable logical definitions and producer/consumer agreement; component baseline |
| 005 | Dependency: calendar/time precision/order/currentness/clock/query boundaries | FUN-004; AOS-02/05/domain owners | Approved comparison/currentness profiles and acceptance fixtures; build |
| 006 | Decision/dependency: approved record-class correction/history/deletion settings, projection/access and permitted disposition evidence; DEC-047 settles direction | FUN-005–007; AOS-02/03/privacy/governance owners | Valid reconciled class policies; activation |
| 007 | Decision/dependency: HACT exact release/terms/field mapping; preferred-reference direction settled by DEC-048 | FUN-010/CON-006; AOS-02/domain stewards for mapping, Mark for newly discovered material departures | Accessible versioned artefacts, precise definitions/losses and approved scope; standards adoption |
| 008 | Design gap: delivery/duplicate/retry/reconciliation semantics and operational limits | FUN-008/009; AOS-04/05/13/14 | Approved profiles/test evidence; build |
| 009 | Dependency: human decision, channel-agreement and outcome common schemas | CON-005; AOS-01/03/11/30/04 | Exact family definitions and approval/effect evidence; component baseline |
| 010 | Assurance gap: threat model, migration/recovery and probabilistic matching evaluations | §§11/13/15; AOS-05/40/domain reviewers | Executable tests, qualified assessment and operating capacity; readiness |
| 011 | Dependency: exact source-matrix allocation and complementary component adoption | §8/19; AOS-02/40 and all semantic owners | Source-to-REQ/VER links and residual findings; component baseline |
| 012 | Review: adequacy across non-repair scenarios and emergent derived uses | §15; Mark/AOS-25/40 | Scenario review with explicit source-grounded scope; component baseline |

Research confidence: high that HACT is a relevant sector interoperability reference; insufficient evidence to claim an exact latest release, comprehensive mapping, formal endorsement or conformance. Direct catalogue access was blocked; the accessible associated model is explicitly provisional.

**AOS-02-ISS-013 — research view exact schema/adoption (open design gap):** §6.6 logical views need exact schema/units/cardinalities/version/catalogue adoption with 04/14/13/30 and all components; reconcile AOS-20 candidate view and shared/core/register/source matrix. Owners: AOS-02 and semantic owners. Evidence: reviewed definitions, reciprocal producers/consumers and executed fixtures; gate: dependent contract baseline/build. AOS-02’s own research profile/sources/cadence/appointments remain activation dependencies.

## 18. Implementation guidance — non-normative

A governed logical layer may use adapters, separate authoritative stores, indexed projections, versioned schemas, evidence journals and permissions-aware retrieval. A central database is one implementation option, not an architectural requirement. A graph or vector index cannot replace exact source/revision/permission evidence.

HACT-compatible payload definitions can sit beneath the common AOS envelope where their verified meaning fits. Mapping should reuse rather than rename equivalent concepts unnecessarily, while retaining separate AOS evidence/authority/outcome metadata. The preferred-reference direction is approved under DEC-048; exact sector schema adoption remains unverified.

No database, API style, message broker, identity format or model is prescribed. Associated reference SQL/DDL illustrates a research model; it is not AOS code or a mandated implementation. External artefact rights and accepted scope must be checked before copying or publishing definitions.

## 19. Traceability and change

Requirement rows link source/decision/engineering derivation to function/dependency and planned VER. CAP/CON/INV/CR tables provide complementary reverse paths. AOS-02-IF-001 remains stable. Core Records retains the single proposed detailed family/envelope definitions; definitive component/schema adoption must resolve gaps without competing copies.

HACT is recorded through EXT-H01–07 and ISS-007. Concept-level assessment is distinguished from field-level mapping. Any adopted mapping records exact source artefact/revision/element, AOS target, relationship/cardinality/type/unit/time/code semantics, transformation/loss, reviewer, approval, tests and permitted use. Later releases require impact review, not automatic replacement.

Extend the controlled source traceability matrix with exact component REQ/VER allocations during adoption. This draft does not close source findings or assert all-domain adoption. Material changes identify affected sources, records, mappings, requirements, consumers, permissions and cases, with rationale and approval evidence.

The agreed sequence is governing principles → architecture → specification → contrasting process tests → justified change where needed. Repair-specific profiles remain scoped. Research agents observe/analyse/challenge/propose without amending the baseline themselves.

### 19.1 Common decision-baseline reconciliation, 6 October 2026

Author review against AOS-00 v0.15 (DEC-001–061) and Specification Map v0.15. Earlier dated source/approval references identify historical derivation, not a competing current baseline. Decisions DEC-001–044 remain applicable as scoped in §§2–8: logical ownership, human reserved powers, common contracts, separate organisation instances, controlled locations, technology neutrality and bounded repair profiles. Repair-specific choices do not become universal rules. DEC-018 remains deferred; independent review remains unassigned. No new decision, permission, numerical setting or requirement approval is inferred.

The table records later-decision applicability and existing document anchors. It is a decision/status reconciliation, not the completed source-to-field-to-producer/consumer traceability required by KR-09.

| Decision set | Applicable direction / responsibility boundary | Existing component anchors | Remaining work / status |
| --- | --- | --- | --- |
| DEC-045–048 | Existing v0.2 approval disposition retained: entity reconciliation, fact-specific source/assurance, governed history/deletion and HACT preferred reference. | REQ-037–046; VER-021–024; ISS-002/003/006/007 | Exact source/matching/lifecycle settings, verified HACT release/mappings and assurance-chain field adoption remain open. |
| DEC-049–053 | Identity assurance is not entity matching; governed private-content, welfare, refusal and disclosure boundaries constrain record exchange. | REQ-022–025/036/040–043; CON-004; VER-010/011/018/022 | AOS-03 v0.3 supplies the logical permission specification; exact family adoption remains ISS-004/006/011. |
| DEC-054–057 | Task memory and worker records retain lineage/restrictions; aggregate and change evidence use common structures without transferring semantic ownership. | REQ-016/018/025/028; CON-003/005/006; VER-007/011/013 | Task/execution field definitions and aggregate accounting remain KR-01/06; no new IF allocated. |
| DEC-058–061 | Incident evidence, selective continuity and restoration preserve current lifecycle restrictions; platform privilege is not record-use permission. | REQ-022/025/028/033/044; CON-004/005; VER-010/011/013/016/023 | Correction consumer map and authoritative recovery inputs remain KR-03/05; they are not repaired by this label pass. |

Stable REQ/VER/CON/IF identifiers, requirement wording and planned-case status are preserved. The five current component revisions are v0.3; their historical v0.1/v0.2 records remain intact. KR-09 decision/status/interface-label work is complete; full reciprocal source/REQ/contract/field/VER allocation remains open with the shared-contract work. Author checks are document checks, not executed verification or independent readiness evidence.

### 19.2 Action-2 source/field/consumer/verification allocation

New REQ-047–052 originate in v0.4, 6 October 2026; status proposed, owner inherited from document control, logical scope only. VER-025–030 are planned cases. Earlier records retain their origins; AOS-03 REQ-040 is clarified under DEC-064, not retired. Totals at this historical adoption step: 52 proposed REQs and 30 planned VERs.

| Source / decision | Register obligation / common field | Component REQ → planned VER | Reciprocal adoption |
| --- | --- | --- | --- |
| DEC-002/065; QS-12/21; GT M1.13 | KXR-01/02/07/08; definition_revision/profile_manifest; KX-10 field_map/losses | REQ-047/048 → VER-025/029 | Every local CON ↔ declared producer/consumer ends in register §6 |
| FP4/6; RP7 audit/uncertainty; DEC-046/062/063 | KXR-03/04; REC-E assurance_refs/status, complete REC-Q and use suitability | REQ-049/052 → VER-026/030 | Evidence producer/AOS-02 ↔ this consumer under independently permitted use |
| RP7 auditability; DEC-064 | KXR-05; original REC-A/D evaluation, REC-X exact-result/checkpoint/effect links | REQ-051 → VER-027 | AOS-01/03 evaluator ↔ AOS-04 execution/AOS-05 runtime ↔ AOS-02 custody |
| RP1 accountability; GT M1.13; DEC-066 | KXR-06; KX-21 stage/result/evidence | REQ-050 → VER-028 | Actual receiver/applier/empowered human ↔ sender/tracker; no assumed non-kernel adoption |

Shared fields and reciprocal logical definitions are now adopted at kernel document level. Old local source-matrix/schema issue descriptions remain residual commissioning/full-suite tasks, not a reason to duplicate definitions. Full-suite source allocation and non-kernel adoption remain open; no implemented conformance or independent readiness evidence.

### 19.3 Action-3 exact obligation/field/consumer/verification allocation

REQ-053–060 originate in v0.5, 6 October; proposed logical scope, custodian/approver inherited, no implementation approval. VER-031–038 are planned. Totals at this historical adoption step: 60 proposed REQs/38 planned VERs. Original record wording and IDs remain unchanged.

| Source / approved decision | Common obligation / field / reciprocal ends | Proposed REQ → planned VER |
| --- | --- | --- |
| DEC-067; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-01; CHECK.request/current sources/version/outcome; 01/03 controls → 04/05 effect gate, 02 custody | REQ-053 → VER-031/032 |
| DEC-068; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-02; ACT.required members/applied vector/restriction fence; 01/03/04/05 application → coordinator/02 | REQ-054 → VER-032 |
| DEC-069; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-03; CHG.consumer application/impact owner; semantic source/02 → all material consumers | REQ-055 → VER-033/034 |
| DEC-070; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-04; ACC.linked scope/period/units; 04 semantics → 05 accounting, 01/03 constraints, 02 custody | REQ-056 → VER-035/036 |
| DEC-071; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-05; RSV.complete demand/admission vector; 04 request → 05 authoritative admission → exact executor | REQ-057 → VER-035 |
| DEC-071; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-06; RSV.confirmed/residual/release evidence; observed effects → 05 account and 02/04 evidence | REQ-058 → VER-036 |
| DEC-071; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-07; WHD.owner/ack/cover/resident duty; service/05 blockers → permitted operational recipient, 13/30/resident workflow | REQ-059 → VER-037/038 |
| DEC-072; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-08; BRK.resume evidence/current check; authorised owner/controls/account → 04/05 executor | REQ-060 → VER-034/038 |

Record types and source locators are the annex §§9–10, using unchanged FP/RP/GT versions. Non-kernel adoption and wire/profile/role implementation remain explicit gaps. This source/field/case allocation does not supply executed or independent assurance.

### 19.4 Action-4 sources and reciprocal verification

REQ-061–066 link DEC-073–078/KPR-01–06 to planned VER-039–044/KPV-01–06 one-to-one; all cases include cross-component failure/acceptance evidence. Source references and derivation boundaries are Protected Reporting and Recovery §7; exact fields, ownership and CON reciprocity are §§2/5. Current authoritative source mechanisms, human capacity, numerical profiles and commissioned independence need explicit owners/evidence before release. These cases have not been executed.

### 19.5 External-research traceability

DEC-086 → CAP-007/FUN-011/CON-007/§6.6 → REQ-067–073 → VER-045–049. Origin v0.7, 6 October 2026; proposed logical wording, project approver Mark, operational semantic owners/appointments open. AOS-04-CON-009 references this single supporting view; AOS-01 v0.7 §6.6 retains existing authority/change/decision contracts. Source matrix/catalogue and remaining consumer specialisations are explicit downstream obligations.

## 20. Build and handover

No build is authorised. A future bounded release requires exact schema/contract/profile/source/mapping manifest, resolved relevant issues, validated permissions/lifecycle/location arrangements, approved synthetic fixtures, accepted cases, platform/recovery implementation and separate readiness assessment.

Builder discretion covers technology behind approved semantics. Stop for unresolved identity/source equivalence, missing data-use permission, unapproved required schema/units, ambiguous timing/currentness, unaccountable correction/deletion, absent recording or unknown effect, incompatible mapping, unverified required standard artefact or newly proposed inference/authority scope.

An HACT reference alone is not a release dependency; if the build depends on an adopted mapping its exact verified artefacts become prerequisites. Author checks cannot satisfy G3's separate reviewer walkthrough. Independent project review remains deferred; organisational independent governance reviews remain required.

## 21. Review and control

| Quality area | Author assessment / residual limitation |
| --- | --- |
| QS-01–03 structure/identity/history | 21 template sections, common stable IDs and explicit control; no earlier AOS-02 found in the current reference-architecture inventory |
| QS-04–10 requirement records | 66 proposed obligations with derivation/category/shared accountability/release/history and planned cases; schemas/values remain unresolved |
| QS-11–14 context/contracts/lifecycle/failure | Shared meaning, source/identity/projection boundaries, preserved IF-001, six CONs, states and failure paths; cross-component implementation pending |
| QS-15–20 qualities/authority/source fidelity | Purpose/restriction/lifecycle/provenance/uncertainty explicit; no numeric default, legal determination or AI truth certificate |
| QS-21–23 traceability/testing | 38 planned cases and six contrasting scenarios; source-matrix allocation/executable assurance not complete |
| QS-24–28 review/handover/readiness | Author review only; no independent assurance, formal gate, build or live activation claim |
| HACT reference adequacy | Primary explanations/associated guidance read and linked; catalogue access/current release/field mapping unresolved; no standards-conformance claim |

Author checks: section/identifier uniqueness, REQ-to-VER linkage and Markdown table structure. No tailoring claimed. Specification-quality conclusion: structured review draft with explicit dependencies. Design-adequacy conclusion: principle-derived common-data model with relevant HACT reference assessment, requiring material-choice review, exact mapping/schema adoption and technical/organisation assurance.

**Next:** action-4 logical protected reporting/recovery adopted with standards provenance. Read existing GI/human-handoff material before further drafting; non-kernel adoption, commissioning and independent/executed evidence remain open.

**v0.7 research amendment author checks:** stable original requirement/verification rows and approval histories preserved; new REQ/VER sequences and references checked; common profile/view/powers ownership reconciled against AOS-00/Map v0.21 and template v0.4. New cases remain planned; no actual research, runtime, independent review or readiness evidence claimed.

## Component summary

**Purpose:** shared meaning and reconstructable evidence without treating storage as truth or permission.  
**Owns:** common structures, source/entity mappings, provenance, time/version/correction and governed exchange.  
**Receives:** permitted source evidence and exact authority/data-use/analysis/decision/execution records.  
**Produces:** validated revision-scoped records, permitted projections, correction/lineage and compatibility evidence.  
**Does not own:** institutional judgement, source truth adjudication, action authority, data-use permission or domain process design.  
**HACT:** approved preferred reference for compatible housing-data definitions; concept assessment included, exact release/mapping adoption and conformance unverified.  
**Conformant when:** accepted requirements and fixed dependency/mapping scope are evidenced across contrasting cases.  
**Open:** semantic/schema choices, source/reconciliation rules, AOS-03 lifecycle/access, exact HACT artefacts/mappings and independent readiness assurance.

**5 October approval disposition:** Mark agreed all four recommendations and emphasised fact-assurance provenance as Radical Transparency. DEC-045–048 in AOS-00 v0.12 / Map v0.9 record these directions. AOS-02 v0.2 incorporates them; exact requirement wording remains proposed and cases planned. No further general-data question is currently submitted to Mark. Detailed schemas, factual assurance criteria, actual source/role/lifecycle settings, HACT artefacts/mappings and readiness evidence remain open.

**Action-2 current disposition, 6 October:** v0.4 uses AOS-00/Map v0.16 and approved DEC-062–066. §6.3/§19.2 record common logical adoption and traceability. Current totals 52 proposed REQs/30 planned VERs; earlier counts/versions in approval histories remain historical. No requirement-wording, executed-case or readiness promotion.

**Action-3 current disposition, 6 October:** DEC-067–072 approved, including revised recommendation 5 notification/acknowledged duty and appropriate resident update. AOS-02 v0.5 adopts Register v0.2, Core/Shared v0.3 and Control Coordination v0.1 against AOS-00/Map v0.17. Current totals 60/38 proposed REQs/planned VERs; no executed assurance or readiness promotion. KR-02/03/06 logically reconciled; actual commissioned implementation remains open.

**Action-4 current disposition, 6 October:** all six directions approved; DEC-073–078 and standards-reference instruction recorded. AOS-02 v0.6; 66 proposed REQs/44 planned VERs. KR-04/05 logically reconciled through the common annex and reciprocal adoption. No executed recovery/report delivery, clause-level ISO conformity, independent assurance or readiness promotion.


**External-research current disposition, 6 October:** AOS-02 v0.7; 73 proposed REQs/49 planned VERs against AOS-00/Map v0.21/template v0.4. Direction DEC-086 approved, logical supporting views proposed; exact schema/adoption/evaluation open, no research activation or readiness claim.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**Historical status notice — AOS-30 alignment — 7 October 2026:** functional drafting and consistency alignment complete under Mark’s instruction. AOS-00/Map v0.25, DEC-001–089; AOS-01–05 v0.8, AOS-14 v0.4, AOS-20 v0.3 and AOS-30 v0.3; Shared v0.9/Core v0.6/Exchange Register v0.8; source matrix v0.9 and template v0.4 unchanged; Control Coordination v0.2/Protected Reporting and Recovery v0.1 unchanged. Earlier dated baseline/adoption/next-step entries are history. CR30-01–03 are closed at the functional-document level; implementation/commissioning evidence remains separate. No new DEC/REQ/VER/IF identifier or operating power is introduced.

