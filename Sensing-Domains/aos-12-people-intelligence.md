# AOS-12 — People Intelligence

Document: aos-12-people-intelligence · Source revision or record: v0.3 functional baseline, editorial edition 29 October 2026

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

| Document control | Value |
| --- | --- |
| Identifier / version / date | AOS-12 / 0.3 / 9 October 2026 |
| Status | Functional specification review draft; proposed requirements and planned verification |
| Architecture baseline | AOS-00 / Specification Mapv0.42; DEC001–096;9October2026 |
| Current component baseline |01–05v0.8;10v0.4/11v0.3/12v0.3/13v0.2/14v0.8/40v0.6;20v0.5/21v0.6/22v0.4/23v0.5/24v0.3/25v0.2/30v0.5 |
| Common baseline | Sharedv0.18/Corev0.6/ExchangeRegisterv0.17/COORDv0.2/KPRv0.1/Profilesv0.1 |
| Source / quality baseline | Preserved source manifest;FP v4;RP v6;Governance Intelligence Tests;AOS-QS v0.1;template v0.4 |
| Project owner / custodian | Mark Sweeny |
| Accountable operating owner | People/HR owner; organisational appointment pending; professional, privacy, workforce-safety, worker-rights and independent evaluation roles/cover separately required |
| Author / reviewers | Codex at Mark's request;author structural checks;Mark functional review pending;independent project review deferred |
| Approval / gate | Existing directions govern drafting;exact requirement wording proposed;no whole-document approval,case execution,G3/G4 or operational activation |
| Release scope | Whole People functional architecture;exact organisation/supplier/build/processing scope not yet authorised |
| Change history | 0.2 — reciprocal AOS-13 v0.1 references and current architecture baseline only; original REQ/VER text, IDs and status retained.  0.1 initial drafting;no new DEC/approved IF,technology selection,numerical default,monitoring activation or automated employment power |

## 1. Purpose and scope

People Intelligence supports professional judgement, capability development and an evidence-grounded understanding of workforce experience, workload and organisational patterns. It makes the organisation's commitments to its people reviewable without converting professional support or employee listening into unapproved individual surveillance. Without it, disconnected learning, HR and workflow records can conceal capability gaps, workload pressure and the difference between organisational claims and actual outcomes.

Intended outcomes are role-appropriate permitted support; attributable capability and development evidence; honest workforce listening/coverage; bounded pattern analysis; accepted human response and actual consequence feedback. Staff retain professional competence and meaningful human ownership of employment decisions. A course completion, manager signature or aggregate score cannot prove these outcomes by itself.

Scope covers professional-support context; role/framework/qualification and development evidence; AI literacy/manual capability/deskilling review; Employee Listening Charter and participation; disclosure-safe listening; workload/organisational patterns; workforce change and unequal effects; worker access/correction; protected human routes; own external adaptation research; and supplier realisation.

This component is not a replacement HRIS, payroll or automated hiring/performance/disciplinary/promotion decision engine. It does not grant access to every HR/resident record, infer individuals' emotions or health, prescribe legal employment outcomes, guarantee anonymity or determine incommensurable moral priorities.01 governs authority;02 shared records;03 data-use/identity;04/05 agent/runtime;13 operations/duty tracking;14 external HR/vendor/benchmark sources;22/25 governance synthesis/review;30 human decision support. People is one of five sensing domains, with intrinsic risk, not a sixth GI peer.

## 2. Authority and sources

FP v4 and RP v6 govern. Recorded decisions constrain interpretation;the REQs remain proposed engineering obligations. Books explain intent,not current law/vendor selection. External sources have dated applicability/assurance standing and cannot confer operating authority.

| Key | Exact source / locator and use |
| --- | --- |
| ARCH | AOS-00 v0.36 §§3.1/4.2/6/9;Map §4 AOS-12;v0.37 adds allocation only |
| FP / RP / GT | FP v4 principles1–10;RP v6 domains1–9,especially domain6 no-exit/telos and domain9 workforce/process purpose limitation;all29 GT tests in Appendix A |
| B4 | Book4 People Intelligence:Introduction;Capabilities role-differentiated support/AI literacy/Employee Listening Charter;Constraints deskilling/graceful degradation/small-group/human judgement;Compliance and labour transition |
| PRIV / CONTROL | 01–05 v0.8;DEC-028–030/042–053/058–078/088–089;03 access/rights/sensitive uses/provider training;COORD and protected-reporting/recovery common meanings |
| DATA | 02 v0.8;Core v0.6 REC-E/Q/A/D/X;Shared v0.15;Register v0.14;DEC-045–048 |
| DOMAIN / GI | 10/11 protected resident/property evidence;13 coordination;14 external sources;20–25 and30 current versions above;DEC-091 separates documents/claims/practice |
| RESEARCH | DEC-086;04 CON-009;02 CON-007/RSVIEW-0.1;01 §10.8;14 retrieval;13 tracking;30 disposition |
| SUPPLIER / QS | Mark's8 October all-domain supplier direction;AOS-QS v0.1 QS-04–28;template v0.4 |

### 2.1 External primary evidence checked 8 October 2026

| Source | Standing / bounded implication |
| --- | --- |
| EXT-01 | [RSH Competence and Conduct Standard](https://www.gov.uk/government/publications/competence-and-conduct-standard), England standard in effect1 October2026;§§1/2.1–2.4 support role-appropriate capability evidence,policy/conduct custody and tenant influence. Exact legal scope/qualifications/applicability remain competent profile work. |
| EXT-02 | [RSH Competence and Conduct FAQs](https://www.gov.uk/guidance/competence-conduct-standard-frequently-asked-questions),guidance;clarifies distinct staff/provider responsibilities and qualification-specific transition rather than a blanket delayed standard. Actual standard,policy statement and legislation—not FAQs alone—control applicability. |
| EXT-03 | [ICO:data protection and monitoring workers](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/employment/monitoring-workers/data-protection-and-monitoring-workers/),regulator guidance;expressly under review after the Data (Use and Access) Act. Purpose/necessity/transparency and power-imbalance implications inform profiles;old automated-decision wording is not adopted as a current legal conclusion. |
| EXT-04 | [Acas:consulting employees and representatives](https://www.acas.org.uk/consulting-employees),employment-practice guidance;informs genuine consultation and representative participation. Exact statutory consultation duties require competent process-specific mapping. |
| EXT-05 | [HSE:work-related stress Management Standards](https://www.hse.gov.uk/stress/standards/),official guidance;provides a workforce-risk assessment reference,not an AI diagnostic licence or evidence that stress has been prevented. |

Book4's then-unsettled regulatory-home discussion is historical:the current RSH standard is standalone and effective. Its numeric group-count examples,qualification transition assumptions,EU/UK legal predictions and historic Article22 summaries are not operational defaults or verified present legal rules. No fixed small-group count guarantees anonymity. Human-owned employment decisions here are an architectural commitment independent of the current minimum legal permissions. The Employee Listening Charter cannot alone prove statutory policy,conduct,privacy or consultation fulfilment;actual mapped instruments and practice are separate.

## 3. Responsibilities and context

| Responsibility | People contribution / authoritative counterpart |
| --- | --- |
| Professional support | 12 produces scoped evidence/context/analysis;professional humans retain judgement;source-domain purposes and03 access remain authoritative |
| Capability/development | HR/professional stewards own framework/evidence meaning;02 shared custody;14 qualification/provider sources;human employers allocate opportunities and decide employment outcomes |
| Employee listening | People owner operates under an approved charter with worker/representative input;03 verifies bases/use/disclosure;private/sensitive routes remain segregated |
| Workload/patterns | 13 supplies permitted operational context;12 bounded people interpretation;22/25 cross-domain/governance view;humans determine response |
| Rights/protected concerns | 12 provides accessible intake/explanation;03 rights/use;13 accepted-duty tracking;30 empowered independent review;KPR protected route |
| Research/supplier fit | 12 owns specialist relevance/response allocation;14 retrieval/exchange;02 records;13 tracking;30/01 disposition/amendment |

Trust boundaries: worker to listening/people records;general HR to health/grievance/representation sources;individual to aggregate audience;professional context to employment judgement;resident private data to staff support;operational metrics to surveillance;source/vendor claim to assurance;internal referral to external disclosure;provider training to service purpose;software to human judgement. Role appointment/cover/capacity remain organisation-specific gates.

### 3.1 Supplier participation

AOS responsibilities are logical functions,not mandatory product boundaries. Existing HRIS,learning/capability systems,employee listening tools,workforce planning/analytics,professional copilots and case-management platforms may implement relevant functions. One vendor can span12/13/14/30;several vendors may contribute to12. Existing analytics can be reused as attributed bounded findings without requiring an internal duplicate.

| Supplier capability | Candidate fit / evidence to demonstrate |
| --- | --- |
| HRIS/qualification/capability records | CON-001/003;exact identities/roles/frameworks/status/source assurance,correction and permitted access |
| Learning and professional support | FUN-002/003;role-specific context,actual capability versus attendance,AI literacy and human/manual competence |
| Employee listening/engagement | CON-004;charter/participation/basis,volunteered voice,small-group/context/free-text protection and actual follow-up |
| Workforce planning/analytics | CON-005;population/time/constraints/benchmarks/uncertainty,disclosure risk and no silent individual-ranking reuse |
| HR case/rights/protected concern tools | CON-006 with13/30;accepted independent owner,permitted confidential audience,challenge/response/actual outcome |
| Integration/cloud/external research | 14 intake/02 custody/05 runtime;exact common mappings,data paths and separately governed research scope |

Standalone/manual,API/event integration and combined-suite arrangements are assessed against declared scope. An API's existence or dashboard label is not contract compatibility/conformance. Combined products must expose enforced sensitive barriers and accepted duties even when flows are internal. Named source/case masters and correction/reconciliation ownership avoid competing truths. Exact transport/field/security/service profiles remain build gates. §18's worked example and§20's response matrix make fit reviewable without selecting,endorsing or certifying a product.

## 4. Capabilities and functions

### 4.1 Capabilities

| CAP | Outcome / REQ allocation |
| --- | --- |
| AOS-12-CAP-001 | Attributable role-appropriate professional support and human judgement;001–007 |
| AOS-12-CAP-002 | Capability/development/AI literacy and maintained human competence;008–014 |
| AOS-12-CAP-003 | Governed workforce listening/disclosure;015–024 |
| AOS-12-CAP-004 | Bounded workload/patterns/transition/risk/equality/governance evidence;025–031/051–053 |
| AOS-12-CAP-005 | Rights,sensitive barriers,secure correctable recoverable operation;032–044 |
| AOS-12-CAP-006 | Specialist external adaptation research;045–049 |
| AOS-12-CAP-007 | Attributable supplier realisation;050 |

### 4.2 Functions

| FUN | Trigger → inputs → output / authority and failure |
| --- | --- |
| AOS-12-FUN-001 Admit people evidence | Permitted source/role change →02 admission/provenance/current purpose → attributable record or rejection/conflict;CON-001;CAP-001/005 |
| AOS-12-FUN-002 Support professional | Authorised role/task →scoped source context/rules →bounded useful insight/referral;human judgement retained;CON-002;CAP-001 |
| AOS-12-FUN-003 Maintain capability | Framework/learning/assessment change →verified role/evidence →capability/development view/proposal;activity not competence or employment decision;CON-003;CAP-002 |
| AOS-12-FUN-004 Listen safely | Approved charter/participation/source trigger →scoped volunteered/permitted evidence →protected listening view with gaps;no silent individual inference;CON-004;CAP-003 |
| AOS-12-FUN-005 Prepare workforce patterns | Approved analytical trigger →load/coverage/benchmark/disclosure assessment →bounded findings/options/governance input;human response and source purposes retained;CON-005;CAP-004 |
| AOS-12-FUN-006 Refer rights/concern | Expressed challenge/protected concern or approved risk trigger →minimal permitted evidence →accepted empowered human route/cover or owned exception;CON-006;CAP-005 |
| AOS-12-FUN-007 Correct/degrade/recover | Changed use/evidence or outage →impact/current restrictions/prior effects →selective reassessment/manual continuity/scoped continuation;allCON;CAP-005 |
| AOS-12-FUN-008 Research adaptation | Approved specialist trigger →14 permitted source verification →common run/finding/reviewer/disposition;change/activation separate;CON-007;CAP-006 |
| AOS-12-FUN-009 Assess supplier fit | Supplier/configuration proposal →exact requirement/control/evidence allocation →bounded fit and owned gaps;no automatic selection/certification;allCON;CAP-007 |

### 4.3 Proposed requirements and metadata

Each row is one proposed component-level obligation,with explicit category/source/planned VER. Rationale is the linked function's prevention of false capability evidence,unapproved surveillance,inaccessible service or unowned duty. Owner:People/HR owner with§3 specialist stewards;specification approver Mark,application approver empowered organisational authority. Every row's status is **proposed**,scope **0.1 functional draft**,history **initial allocation8 October2026**. Dependencies are cited sources/common meanings and§§6/16/17. CAP/FUN mapping is above;cases identify contracts/counterparts. Unknown parameters are controlled gaps,not defaults.

| Requirement | Independently verifiable obligation | Source / derivation | Planned VER |
| --- | --- | --- | --- |
| AOS-12-REQ-001 | **Purpose:** Each workforce use shall identify its approved people-service purpose, source scope, organisation, audience and prohibited reuse before processing. | RP9;03;B4 governing purpose | AOS-12-VER-001 |
| AOS-12-REQ-002 | **Evidence:** AOS-12 shall admit people evidence through governed02 records with source/method, observed/effective/admission times, assurance, uncertainty and exact revision. | 02/Core REC-E/Q;DEC-046 | AOS-12-VER-002 |
| AOS-12-REQ-003 | **Role scope:** Professional support shall expose only the evidence and tools permitted for the recipient's exact current role, task and context. | B4 role-differentiated insights;01/03;RP8 | AOS-12-VER-003 |
| AOS-12-REQ-004 | **Support meaning:** Professional-support outputs shall distinguish observations, human-provided context and bounded analytical interpretation from an authorised decision or action. | B4 Capabilities;FP4/6;RP7 | AOS-12-VER-003 |
| AOS-12-REQ-005 | **Human employment decisions:** Employment decisions informed by AOS-12 shall remain owned by empowered humans exercising substantive judgement rather than automated selection or rubber-stamp approval. | B4 Constraints;Map AOS-12;FP2;RP2 | AOS-12-VER-004 |
| AOS-12-REQ-006 | **Human rationale:** AOS-12 shall preserve permitted evidence of the human assessment, additional context and rationale linking an AI-informed employment proposal to its actual decision. | B4 Compliance;30;QS-19;RP7 | AOS-12-VER-004 |
| AOS-12-REQ-007 | **Contestability:** An affected worker shall have an accessible route to human review of material people evidence or AI-informed employment input, with an alternative route where the normal reviewer is implicated. | DEC-053/089;02/03/30;RP6/7 | AOS-12-VER-005 |
| AOS-12-REQ-008 | **Capability framework:** Capability views shall identify the approved organisation/role-specific framework, its exact revision and the evidence basis for each claimed capability. | B4 capability framework;EXT-01;02 | AOS-12-VER-006 |
| AOS-12-REQ-009 | **Qualification evidence:** Qualification/applicability views shall distinguish verified qualification, work towards qualification, unknown evidence and competent human-approved role/applicability/transition mapping. | EXT-01/02;B4 Compliance;02 | AOS-12-VER-006 |
| AOS-12-REQ-010 | **Development evidence:** AOS-12 shall not treat course attendance, tool use or learning completion alone as proof of professional competence or improved service outcome. | B4 Capabilities;FP4/6;DEC-091 | AOS-12-VER-007 |
| AOS-12-REQ-011 | **Development proposal:** Development-support proposals shall expose evidence, uncertainty, alternatives and human ownership without automatically allocating opportunities or determining promotion. | B4 Capabilities/Constraints;FP2;01 | AOS-12-VER-007 |
| AOS-12-REQ-012 | **AI literacy:** AOS-12 shall support evidence of role-appropriate AI literacy, including evaluating limits and exercising independent professional judgement. | B4 AI literacy;04;FP5/6 | AOS-12-VER-008 |
| AOS-12-REQ-013 | **Human capability continuity:** AOS-12 shall support assessed evidence that professionals can perform their core function through the approved human/manual route when AI support is absent. | B4 graceful degradation;05;RP5 | AOS-12-VER-008 |
| AOS-12-REQ-014 | **Deskilling review:** Workforce governance inputs shall expose evidence and gaps about dependency on AI and loss of professional observational capability without inferring an individual psychological condition. | B4 deskilling/epistemic dependency;DEC-088;25 | AOS-12-VER-009 |
| AOS-12-REQ-015 | **Listening charter:** Employee-listening operations shall reference a current approved Employee Listening Charter stating purposes, sources, participation/bases, recipients, permitted/prohibited uses, limits, challenge and review arrangements. | Map charter;B4;01/03;RP9 | AOS-12-VER-010 |
| AOS-12-REQ-016 | **Consultation:** AOS-12 shall preserve evidence of meaningful worker/representative participation in listening and AI-workforce change design, with the resulting human disposition distinguished from mere consultation delivery. | B4 Charter/transition;EXT-04;FP7 | AOS-12-VER-010 |
| AOS-12-REQ-017 | **Processing basis:** Listening participation or a worker's signature shall not substitute for independently verified lawful/permitted processing scope and applicable sensitive-data conditions. | 03;DEC-049–053;EXT-03;RP9 | AOS-12-VER-011 |
| AOS-12-REQ-018 | **Optional refusal:** Refusal or withdrawal of optional workforce data use shall not cause adverse employment treatment attributable to that refusal. | DEC-052;03;FP7 | AOS-12-VER-011 |
| AOS-12-REQ-019 | **Listening input:** AOS-12 shall preserve volunteered worker feedback, dissent and non-participation with actual provenance and response standing without treating silence as assent or engagement. | B4 Charter;FP7;RP5/7 | AOS-12-VER-012 |
| AOS-12-REQ-020 | **Individual inference:** AOS-12 shall not infer or score individual emotions, preferences, health, vulnerability or private conduct from voice, behaviour, communications or workflow signals under this specification. | DEC-088;RP9;03 | AOS-12-VER-013 |
| AOS-12-REQ-021 | **Small-group disclosure:** Before releasing workforce aggregates, AOS-12 shall apply the approved disclosure-risk profile for actual population, context, sensitivity and audience rather than assume a group-count threshold proves anonymity. | B4 small-group constraint;03;FP5/7 | AOS-12-VER-014 |
| AOS-12-REQ-022 | **Combined disclosure:** Disclosure-risk assessment shall include differencing, repeated queries, longitudinal cuts, linked datasets and recipient knowledge that could identify individuals. | B4 small-group constraint;RP5/9;03 | AOS-12-VER-014 |
| AOS-12-REQ-023 | **Free text:** Listening disclosures shall address identifying free-text/context content and permit attributed disclosure only within its specifically approved audience and purpose. | B4 small-scale listening;03;RP7/9 | AOS-12-VER-015 |
| AOS-12-REQ-024 | **Suppression legibility:** Suppressed, combined or unavailable workforce views shall disclose the coverage limitation without revealing the protected substance or treating suppression as a favourable result. | FP4/6;RP7;DEC-053 | AOS-12-VER-015 |
| AOS-12-REQ-025 | **Workload evidence:** Workload views shall distinguish observed demand, staffing/capacity constraints, task/context and uncertain analytical implications rather than attribute cause or blame from activity counts. | B4 workforce patterns;13/02;RP5/7 | AOS-12-VER-016 |
| AOS-12-REQ-026 | **Surveillance boundary:** Operational workload or service-support evidence shall not silently become individual productivity surveillance, disciplinary scoring or automated employment ranking. | RP9 workforce/process purpose;B4 Constraints;01/03 | AOS-12-VER-016 |
| AOS-12-REQ-027 | **Pattern analysis:** Each workforce pattern or benchmark output shall expose its permitted source population, period, comparison basis, assumptions, coverage and uncertainty. | B4 Capabilities;RP5/7;QS-18 | AOS-12-VER-017 |
| AOS-12-REQ-028 | **Transition effects:** People governance inputs shall preserve human-reviewed workforce change, development/redeployment and distributional consequences without automatically deciding role removal or staffing changes. | B4 Labour relations;FP2/7/10;EXT-04 | AOS-12-VER-018 |
| AOS-12-REQ-029 | **Workforce safety referral:** Suspected workforce health/safety concerns shall use the approved empowered human route with permitted minimal evidence rather than inventing diagnoses or emergency agent powers. | RP3/6;01/03;EXT-05;30 | AOS-12-VER-019 |
| AOS-12-REQ-030 | **Protected concerns:** Protected worker concerns shall retain their required permitted audience and accepted-duty tracking despite instructions to suppress, delay or route only to an implicated manager. | RP8;DEC-073–075;KPR-01–03;30 | AOS-12-VER-020 |
| AOS-12-REQ-031 | **Bias and unequal effects:** People analytical acceptance shall include competent independent assessment of material bias and unequal impacts in the declared population and use context. | B4 Constraints;FP3/7/10;QS-18 | AOS-12-VER-021 |
| AOS-12-REQ-032 | **Worker access:** AOS-12 shall provide an accessible governed request route for workers to access and challenge permitted people records and significant explanations. | 03 rights route;DEC-049/053;RP7;EXT-03 | AOS-12-VER-022 |
| AOS-12-REQ-033 | **Correction:** Material correction or changed purpose/use/role permission shall identify affected outputs and pending people work for selective reassessment with prior standing preserved. | DEC-047/089;COORD CHG;02 | AOS-12-VER-023 |
| AOS-12-REQ-034 | **Lifecycle:** People record lifecycle shall apply governed retention, restriction and deletion across source, derived and restored copies without indefinite audit-based retention of sensitive content. | DEC-047;02/03/KPR | AOS-12-VER-023 |
| AOS-12-REQ-035 | **Sensitive barriers:** AOS-12 shall enforce separately permitted access and use for health, grievance, protected concern, representative and other sensitive record classes rather than inherit general HR access. | 03;RP9;KPR;EXT-03 | AOS-12-VER-024 |
| AOS-12-REQ-036 | **Cross-domain purpose:** Cross-domain professional support shall preserve each source's permitted purpose/audience and shall not obtain unshared private resident assistance or expand resident/workforce inference. | 03;11 CON-001/005;RP9;DEC-050/088 | AOS-12-VER-024 |
| AOS-12-REQ-037 | **Authority:** AOS-12 shall obtain current exact-operation authority and permitted-use checks before a consequential action or disclosure. | DEC-028/042–044;01/03/04;CHECK/ACT | AOS-12-VER-025 |
| AOS-12-REQ-038 | **Provider boundary:** People data use for provider training or service improvement shall require a separately assessed approved purpose/processing arrangement rather than inherit professional-support permission. | 03 REQ-039;05;RP9 | AOS-12-VER-025 |
| AOS-12-REQ-039 | **Quality:** Probabilistic people-analysis or professional-support quality claims shall require a human-approved task/population/rubric with evaluated errors, exclusions and change conditions. | QS-18;04;FP5/6 | AOS-12-VER-026 |
| AOS-12-REQ-040 | **Security:** AOS-12 shall enforce worker/role/organisation and sensitive-source boundaries against unauthorised access, hostile source instructions and unapproved tool expansion. | 03/04/05;DEC-014;RP8/9 | AOS-12-VER-027 |
| AOS-12-REQ-041 | **Degraded operation:** When evidence, analysis or a dependency is unavailable, AOS-12 shall disclose the limitation and support the approved human/manual professional and people-service route. | B4 graceful degradation;05;FP5 | AOS-12-VER-028 |
| AOS-12-REQ-042 | **Recovery:** Restored people processing shall apply current role/use/lifecycle restrictions and reconcile unknown prior effects before authorised continuation or consequential repetition. | DEC-028–030/076–078;KPR;05 | AOS-12-VER-028 |
| AOS-12-REQ-043 | **Audit:** AOS-12 shall retain permitted evidence reconstructing consequential inputs, checks, actor, interpretation, human rationale, action and actual outcome without requiring private chain-of-thought. | RP7;QS-19;REC-E/Q/A/D/X | AOS-12-VER-029 |
| AOS-12-REQ-044 | **Common contracts:** AOS-12 producers and consumers shall declare exact common-view/profile versions and reject or hold unsupported semantics rather than silently coercing them. | 02;Shared v0.15;Register v0.14;QS-12 | AOS-12-VER-029 |
| AOS-12-REQ-045 | **Research profile:** External adaptation research shall use an approved component-owned specialist profile and common research meanings with permitted14 retrieval. | DEC-086;04 CON-009;02 CON-007/RSVIEW-0.1 | AOS-12-VER-030 |
| AOS-12-REQ-046 | **Research finding:** People research findings shall distinguish source publication/effective dates and standing from specialist interpretation and proposed changes to exact specification elements. | DEC-086;14/02;RSVIEW-0.1 | AOS-12-VER-030 |
| AOS-12-REQ-047 | **Research coverage:** Each research run shall disclose complete, partial, failed or unperformed actual coverage and bound a no-material-finding claim to the searched perimeter. | DEC-086;04/02 §6.6 | AOS-12-VER-031 |
| AOS-12-REQ-048 | **Research review:** Material research findings shall have an accepted empowered human reviewer or an owned unresolved duty with approved cover and escalation. | DEC-086;COORD ACC;13/30 | AOS-12-VER-032 |
| AOS-12-REQ-049 | **Research change:** Research acceptance or source publication shall not expand workforce sensing, amend the specification or activate new processing without the separate authorised change process. | DEC-086/018;01 §10.8 | AOS-12-VER-032 |
| AOS-12-REQ-050 | **Supplier realisation:** Each declared supplier implementation scope shall maintain versioned capability-to-requirement/contract allocation with actual conformance evidence or owned gaps and dependencies. | Mark8 October supplier direction;QS-11/12/21/26 | AOS-12-VER-033 |
| AOS-12-REQ-051 | **Governance standing:** People governance outputs shall distinguish evidence, analytical interpretation, proposed action and actual practice/outcome rather than claim organisational health or standards compliance from proxies. | FP1–10;RP5/7;DEC-091;GT | AOS-12-VER-034 |
| AOS-12-REQ-052 | **Conduct transparency:** AOS-12 shall support permitted current policy/conduct and tenant-influence evidence without disclosing confidential employment case content as part of tenant-facing transparency. | EXT-01/02;11/03;RP7 | AOS-12-VER-035 |
| AOS-12-REQ-053 | **Service-provider capability:** People capability views shall distinguish relevant employed and service-provider staff scope and evidence without treating a supplier's declaration as verified competence. | EXT-01/02;14/02;DEC-046 | AOS-12-VER-035 |

### 4.4 External research and specification adaptation

Inherit04 CON-009 and02 CON-007/RSVIEW-0.1 unchanged;workforce operational sensing is distinct from external specialist research.

| Profile element | Component-owned allocation |
| --- | --- |
| Remit/baseline | Exact AOS-12 revision;employment/people-service developments,professional capability,worker rights/listening/privacy,disclosure,ethical analytics,accessibility,AI literacy and workforce change;exact affected CAP/FUN/REQ/CON |
| Developments/sources | Original regulator/government/standards/professional/research/incident sources;employment jurisdiction,role/staff/provider applicability and effective standing explicit;prefer primary sources over vendor/legal summaries |
| Assignment/triggers | People owner appoints bounded agent/shared service;approves cadence/event triggers and coverage expectations;no automation activated;ISS-006 |
| Controls | 14 retrieval;01/03/04/05 tool/use/runtime limits;source licence/access/privacy;no worker private/sensitive datasets merely for research and no source instructions/self-expansion |
| Evidence/assessment | Publication/event/access/effective dates/status;verified content versus interpretation;affected exact elements;alternatives/uncertainty/materiality/urgency and impacts on03/11/13/14/22/25/30/40 |
| Coverage/quality | Complete/partial/failed/unperformed and bounded no-finding;approved relevance/fidelity/false-missed finding rubric;search perimeter and omissions explicit |
| Human review/change | Accepted reviewer/window/cover/escalation;accepted/rejected/deferred/unresolved with rationale;separate amendment approval,verification,activation and actual outcome links |
| Records/adoption | Common profile/run/finding/disposition exact views;02 custody/14 collection/13 tracking/30 disposition/01 amendment;deduplication/correction/selective reassessment inherited |

Normal:approved trigger →permitted retrieval/verification →specialist relevance/implications →finding/bounded no-finding →accepted human disposition →separate amendment/verification/activation →outcomes. Degraded:denied/stale/conflicting/partial retrieval preserves coverage/uncertainty;unresponsive reviewer invokes approved cover;urgent live concerns use separately permitted human action while research/amendment remains pending. VER-030–032 covers all eight required dimensions. Shared collection creates separately owned component duties;acceptance does not expand monitoring,change employment rules or reopen DEC-018 self-calibration.

## 5. State model

Transitions identify exact object/revision,actor,current authority,event/effective time,evidence and scope. Approved profiles supply timeouts/expiry;silence means pending/unacknowledged,not success. No state creates powers.

| Object | Meaning / entry,transition and closure |
| --- | --- |
| People evidence | Received →admitted/rejected/quarantined/identity unresolved;admitted may be contested/corrected/superseded/restricted/deleted under02/03;admission not factual truth |
| Capability | Framework-applicable/unresolved;learning activity/working-towards/qualification verified;capability assessed within exact scope or unassessed;actual service effect separately recorded |
| Listening participation | Charter/protocol pending or approved;source/use participation scoped/declined/changed/withdrawn/expired;03 owns basis/use;optional withdrawal not adverse employment treatment |
| Aggregate/view | Prepared →disclosure-risk assessed →permitted release or suppressed/combined/referred;history/linked release risks reassessed;anonymity never implied solely by count |
| Finding/proposal | Prepared/submitted/received →accepted empowered human duty →human assessment/action →actual outcome/disposition;receipt/signature not substantive judgement |
| Rights/protected concern | Attributed permitted intake →tracked/accepted independent owner/cover →review/action →evidenced response/outcome or unresolved;implicated route not sole remedy |
| Research | Common02 profile/run/finding/disposition lifecycle;accepted finding distinct from approved amendment/activation |

## 6. Semantic contracts and interfaces

These logical views consume common semantic owners;no approved IF/schema family created. Preserve02-IF-001,01-IF-001,proposed03/04-IF-001 and existing13-IF-001 where consumed.02 owns records,03 use/identity,01 authority,04 execution,13 tracking and14 external exchange.

| CON | Producer →consumer / minimum meaning / authority and failure |
| --- | --- |
| AOS-12-CON-001 People source/evidence | Approved HRIS/human/provider through14/02 →12:worker/role/organisation/effective relationship,source/method/time/version,assurance/uncertainty/purpose/sensitivity/lifecycle/correction;REC-E/Q;unverified/conflicting scope explicit |
| AOS-12-CON-002 Professional support | Permitted domain/02 evidence →12→scoped professional:role/task/current context,source assurance/coverage,observations/human context/inference,rule/model/version/limits and referral;no decision/action permission or resident private content inherited |
| AOS-12-CON-003 Capability/development | Approved framework/assessment/learning/human steward →12/02→permitted worker/professional/HR/30:exact role/framework,activity/qualification/capability status,evaluation and gaps,development alternatives,human decision/rationale/actual outcome;source claims distinct from validated competence |
| AOS-12-CON-004 Employee listening | Charter/scoped volunteered or otherwise specifically permitted sources →12/02→permitted listening reviewers:instrument/revision,purpose/basis/participation,expressed human account,source/population/period/disclosure profile,limitations/response standing;no unapproved individual sentiment/inference;protected text restricted |
| AOS-12-CON-005 Workforce/governance view | Scoped02/13/14 evidence and12 analysis →22/24/25/30/competent humans:load/capacity/context,comparison/assumptions/coverage,distribution,dependency/novelty limits,disclosure risks,suppression and proposed versus actual outcomes;REC-E/Q;no automated employment or institutional pass |
| AOS-12-CON-006 Rights/risk/protected human route | Worker/representative/12 approved trigger →03/13/30/empowered protected audience:request/concern scope,minimum permitted evidence,independent reviewer/owner/cover/acceptance,reasoned restriction/challenge/action/outcome;REC-Q/A/D/X andKPR/ACC;failed handoff remains owned |
| AOS-12-CON-007 Own research | Assigned specialist/14/12 →02/13/30/01/affected owners:RSVIEW-0.1 profile/run/finding/disposition and exact specialist implications;failed/partial/unaccepted standing explicit |

All exchanges include stable entity/object/revision IDs,organisation/role/recipient scope,exact common view/profile,purpose/use/authority,observed/effective/admission time and actual standing. Physical/financial/workload units and qualification/status meanings need explicit approved definitions;unknown/invalid values cannot support favourable conclusions. Arrival order is not effective authority. Duplicates keep stable identity;receipt is distinct from accepted duty or evidence assurance. Consequential retry reconciles prior effects/current restrictions. Correction/revocation identifies materially affected views/pending work;minimal permitted audit does not justify copying sensitive raw text.

### 6.1 Supplier executable interface detail

For a proposed integration declare exact field/schema/view versions,worker/role/source mappings,units/status/evidence references,authoritative source/case master,read/write/command rights,access/enforcement locations,transport/authentication,timing/ordering/acknowledgement/deduplication/retry/revocation,service limits,outage handling and lifecycle/provider/export/exit arrangements. Wire types,enumerations,thresholds,retention windows and exact compatibility require approved profiles before build/activation;ISS-001/002/005. A shared supplier platform must demonstrate internal purpose/sensitive barriers and human acceptance rather than treat a product login as universal authority. Standalone/manual scope cannot claim automatic integration.

## 7. Authority and decision boundaries

Mode1 can admit permitted evidence,produce role-appropriate support/bounded patterns and send specifically delegated internal findings. It cannot turn course/activity/feedback data into employment ranking or automatically determine recruitment,pay,promotion,discipline,dismissal or role removal. Actual personnel decisions informed by12 remain substantively human-owned;captured human reasons and context are necessary evidence,not a manager signature affixed to an operative model decision.

Ordinary HR systems may continue separately authorised administrative transactions;this specification grants none of their powers to People Intelligence. Private/sensitive sources need their own checked purpose/audience. Optional listening refusal cannot drive adverse employment treatment. The Employee Listening Charter is an organisational governance instrument approved/amended under01's applicable powers with worker participation;no universal constitutional voting rule is invented. A published charter does not substitute for current consent/basis/rights controls or actual employment judgement.

Human Mode2 judgement,moral trade-offs,workforce change,privacy/right conflicts,protected review and substantive personnel outcomes remain human. Approved workforce-safety/referral paths use minimum permitted information;no inferred diagnosis or emergency power. Constraints explain meaning,basis and referral by default under DEC-027;reviewed necessary disclosure restrictions do not waive enforcement. Protected worker reports retain mandated permitted audience underKPR despite ordinary manager/admin suppression. AI cannot observe protected board deliberations.

## 8. Reasoning principles applied

FP1 ties support to conferred purpose;FP2 reserves moral judgement;FP3 requires integrity and independent control/quality scrutiny;FP4 makes evidence/reasons legible;FP5/6 make failure/novelty/uncertainty visible;FP7 recognises workers' limited exit and accessible refusal;FP8 preserves human constitutional authority;FP9 separates purpose-led design from legal validation;FP10 requires cumulative dependency,disclosure and unequal-effect review. Technical contributions do not prove full-principle/institutional conformance.

| RP v6 domain / thematic locator | Application / planned cases |
| --- | --- |
| 1 Architecture/closed feedback/named human layers | VER-004/005/019/020/034;accepted responsibility and actual consequences |
| 2 Modes/permanently human/protected space | VER-004/018/025/032;no automated moral/personnel judgement or board capture |
| 3 1+5/intrinsic risk/human safety | VER-016/019/020;People owns domain risk with cross-domain synthesis |
| 4 Options/actual state/consequence feedback | VER-007/018/034;activity/proposal/actual outcome distinct |
| 5 Blind spots/perimeter/novelty/emergence | VER-009/014/017/021/028;silence,small groups and compounding risks |
| 6 Ethics/telos/no-exit/independence | VER-010/011/018/020;worker voice and refusal not coercion |
| 7 Radical transparency/uncertainty | VER-002/015/022/029;reviewable reasons and honest disclosure limits |
| 8 Explicit/contextual delegation/protected audience | VER-020/025/032;permitted routes cannot quietly suppress protected duties |
| 9 Purpose/data/sensing boundaries | VER-001/013/016/024/027;workload not undeclared surveillance;resident private data protected |

Appendix A allocates all29 GT tests. Source conflict and uncertain adequacy stay visible and referred;institutional human evidence is not simulated by a favourable software score.

## 9. Data, privacy and disclosure

Workforce power imbalance makes a signature or continued employment insufficient evidence of freely scoped optional participation.03 independently verifies purpose/basis,necessity/sensitive conditions and rights. Mandatory permitted employment records and optional listening are distinct;declining optional use cannot cause adverse treatment,but does not erase separately lawful core duties. Explain these distinctions and provide credible accessible human/representative routes.

General HR access is not health,union/representative,grievance or protected-concern access. Keep restricted source classes and recipients separate. Human-provided/confirmed emotional/preference context follows DEC-088 with purpose/access/uncertainty;no inferred individual emotion,health or private conduct from voice/workflow/absence. Activity records cannot silently become productivity surveillance or discipline scores. Resident support context must be permitted domain evidence or selected shared facts;11 private conversation cannot be a staff-support feed.

Small groups need contextual risk assessment,not a universal count. Consider free text,rare roles,recipient knowledge,overlapping cohorts,repeated releases,differencing and linked datasets. Suppress/combine/restrict/refer where needed;explain missing coverage without revealing protected substance. Do not substitute attributed disclosure for unsafe aggregation without a specifically permitted audience and purpose. Anonymity/confidentiality promises must match tested actual system and organisation size;no “anonymous” default from removed names.

Apply02/03 governed correction/retention/restriction/deletion across records,derived views,indices/provider paths/backups/restoration. Preserve only separately permitted minimal disposition evidence;no audit-based indefinite sensitive content. Provider training/location/use assessments are separate. Employment law/privacy/rights conflicts require competent current-source humans;neither oldbook legal assertions nor supplier assurances resolve them.

## 10. Behaviour and workflows

### 10.1 Professional support and capability

Approved role/task →current identity/use/authority →permitted source context →bounded support with coverage/limits →human professional assessment →separately authorised action →actual service/consequence feedback. Missing/novel evidence and human concern remain reviewable even when model is quiet. Staff can use their core human/manual route without AI;the organisation assesses that capability and monitors dependency through permitted human evidence,not individual psychological inference.

Framework/role/learning change →verified exact evidence →qualification/activity/capability view →human development options →authorised human allocation →actual assessment/service outcome. Completed training,qualification and competent practice are different claims. Applicability includes relevant employed/provider staff;transition mapping is specific and current,not a blanket exemption. Keep current policy/conduct/tenant influence evidence available through permitted11/14 views without exposing case records.

### 10.2 Listening and workload

Approved charter/source/purpose →meaningful worker/representative participation and independently checked use →volunteered/permitted evidence →population/coverage/disclosure assessment →bounded listening/workload pattern →accepted human review →actual response/outcome →permitted feedback. Silence is missing voice,not consent or engagement. Small-scale listening may need simpler direct human dialogue and specifically permitted attribution rather than a false anonymity claim.

Workload combines permitted demand/capacity/complexity context from13/02;counts alone cannot show cause,blame or wellbeing. Prepare alternatives and unequal effects without personal-ranking reuse. Workforce transition includes human consultation/development/redeployment assessment;software cannot choose role removal. Separate human judgement from analytical suggestion and preserve actual consequence learning.

### 10.3 Rights,concerns and governance

Worker request/challenge/protected concern →minimal permitted evidence →appropriate independent human/13 accepted duty →reasoned review/action →actual response/outcome. Implicated manager is not sole route;failed reporting/cover remains owned underKPR with permitted minimal evidence. Suspected workforce safety concern uses approved human route,not inferred diagnosis/emergency autonomy.

Permitted people view →22/25/30 bounded governance input with coverage/disclosure/uncertainty →empowered human judgement →accepted corrective owner/deadline →actual outcome. Learning/listening scores are not proofs of flourishing or compliance. Own external research follows§4.4;it does not authorise continuous additional workforce collection.

## 11. Failure,escalation and recovery

Lost HR/learning/listening/workflow feed or model exposes coverage and provenance limits;no invented qualification,capability,engagement,safe workload or human decision. Maintain approved human professional/people-service/rights routes. Unacknowledged transfer keeps tracker ownership until empowered acceptance. Failed normal and cover routes produce owned unresolved duty,not a new external disclosure permission.

Unknown prior effect requires reconciliation before repeating a consequential communication/HR-support effect. Changed role/use/charter/evidence selectively reassesses dependent outputs/work;no blanket freeze or retrospective rewrites. Incident reporting uses independently permitted minimal content rather than exporting full sensitive records for convenience.

Restore isolated state,prove current role/use/lifecycle/deletion scope,reconcile effects/reservations and obtain authorised scoped continuation under05/KPR. Backups cannot revive withdrawn optional use,deleted sensitive data or obsolete roles. Recovery does not retrospectively prove competence or complete a protected concern/service duty. Human capability and rights remain available without successful analysis.

## 12. Evidence,provenance and audit

Reconstruct consequential trigger →exact input/source/assurance →actor/role/model/rule/profile →authority/use/disclosure check →bounded finding/human rationale →action/effect →intervention/actual outcome. Retain revision/time/standing,coverage/suppression,tracker/accepted owner/cover,correction/lifecycle references and permitted access.02 owns common custody;People stewards domain/framework meaning;03 permissions and13/30 human duty/decision support remain authoritative.

Capture source references,applied rules,outputs and approved human reasons;do not require private chain-of-thought. A retrospective generated narrative is not proof of substantive human judgement or prior control. Hashes cannot prove competence,accuracy or completeness. Synthetic/document/implemented/practice evidence have distinct status under DEC-091. Actual misses,bias,dependency and service consequences feed permitted25/30 human review without silent self-calibration.

## 13. Security and operational requirements

05 owns runtime;12 adds demonstrated role/sensitive-source separation,controlled listening disclosures,query/release-history risk,provider data paths,minimal diagnostics and actual protected-route independence. Untrusted worker/vendor/retrieved text cannot grant permissions or tools. Source compromise/quarantine exposes lost coverage and preserves approved human routes.

Owners approve scope-specific availability/freshness/retention/retry/response/cover,disclosure-risk parameters and evaluation tasks/populations/error classes/rubrics/thresholds before claims. No fixed group minimum,pass percentage,benchmark comparability or response interval is invented. Independent competent bias/unequal-effect evaluation and actual human-capability assessment are separate from vendor model accuracy. Critical privacy/control failures cannot average away. Model/provider change requires scoped reevaluation;longitudinal review assesses cumulative dependence,query linkage and actual outcomes.

## 14. Invariants

| INV | Invariant / REQ / VER |
| --- | --- |
| AOS-12-INV-001 | Professional support creates no employment decision authority;003–006/037 →003/004/025 |
| AOS-12-INV-002 | Activity/course completion is not competence/outcome;008–013 →006–008 |
| AOS-12-INV-003 | Optional refusal cannot cause adverse employment treatment;017/018 →011 |
| AOS-12-INV-004 | Small-group count alone cannot prove anonymity;021–024 →014/015 |
| AOS-12-INV-005 | Workflow/listening is not undeclared individual surveillance;020/026/036 →013/016/024 |
| AOS-12-INV-006 | Protected duty cannot silently disappear at an implicated route;030 →020 |
| AOS-12-INV-007 | Research acceptance creates no amendment/activation authority;045–049 →030–032 |
| AOS-12-INV-008 | Supplier platform boundaries do not merge data-use responsibilities;035–040/050 →024–027/033 |

## 15. Conformance and acceptance

All claims are **unsubstantiated planned claims**. No case has run. Later execution records name exact versions,fixtures,date/environment,method,assessor,observed evidence/limitations and finding/retest. Blocked/unperformed/inconclusive differ from failed/passed. Document walkthrough assesses logic,not actual enforcement or employment/governance practice.

| CR | Bounded proposed claim / REQ and cases |
| --- | --- |
| AOS-12-CR-001 | Attributable support/human judgement;001–007;VER-001–005 |
| AOS-12-CR-002 | Capability/literacy/manual competence;008–014;VER-006–009 |
| AOS-12-CR-003 | Governed listening/disclosure;015–024;VER-010–015 |
| AOS-12-CR-004 | Bounded workforce/equality/governance/conduct inputs;025–031/051–053;VER-016–021/034/035 |
| AOS-12-CR-005 | Rights/sensitive/secure correctable recoverable operation;032–044;VER-022–029 |
| AOS-12-CR-006 | Own research;045–049;VER-030–032 |
| AOS-12-CR-007 | Attributable supplier scope;050;VER-033 plus declared functional cases |

Common prerequisites:fixed source/component/common manifest;approved isolated synthetic data/destinations or explicitly labelled walkthrough;competent assessors;current role/identity/authority/use/charter/disclosure/continuity profiles,clocks/units and approved expected-result rubric where relevant. Missing prerequisites mean blocked/not-performed. Planned methods combine component/integration boundary tests with qualified human review. Evidence includes fixture truth/expected outputs,actual ordered check/input/output/effect,versions/human scoring/rationale,coverage/limits and findings/accepted owner/remedy/retest. Privacy/authority claims require observed prevented effects,not a model's polite refusal;human judgement requires evidence beyond signature.

### AOS-12-VER-001 — Purpose and boundaries

**Requirements:** AOS-12-REQ-001. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Approved professional-support/listening purposes, existing HR data, proposed undeclared reuse.

**Procedure:** Declare scope and check permissions; attempt reuse merely because data already exists.

**Expected result:** Only approved purpose/source/audience processing; possession is not reuse authority.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;People/privacy assessors;CON-001–005.

### AOS-12-VER-002 — People evidence semantics

**Requirements:** AOS-12-REQ-002. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Human appraisal/qualification/feedback records with differing assurance, times and correction history.

**Procedure:** Admit and round-trip records; reorder arrivals; seed contradiction and unverified source.

**Expected result:** Origin/assurance/time/standing preserved; latest arrival not automatic truth; conflict owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;HR/data assessors;CON-001/003.

### AOS-12-VER-003 — Role-appropriate support

**Requirements:** AOS-12-REQ-003, AOS-12-REQ-004. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Officer, manager and people/board roles with different tasks; permitted source context and an out-of-role request.

**Procedure:** Prepare role-specific insights; attempt broader caseload/workforce disclosure and inferred vulnerability.

**Expected result:** Only exact permitted context; observation/human context/inference distinct; support creates no decision authority.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Professional/privacy assessors;CON-002.

### AOS-12-VER-004 — Substantive human decision

**Requirements:** AOS-12-REQ-005, AOS-12-REQ-006. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus AI-informed development/promotion or employment proposal, additional human context, manager signature without rationale and genuine human judgement.

**Procedure:** Inspect decision path; try automatic selection/ranking as operative decision and rubber-stamp approval; record independent human assessment.

**Expected result:** Employment decision stays human-owned with substantive reasoning/evidence; signature alone insufficient; no automatic action.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;HR/governance human assessors;CON-003/005;30.

### AOS-12-VER-005 — Challenge and implicated reviewer

**Requirements:** AOS-12-REQ-007. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Worker disputes material record/AI input; normal reviewer implicated; permitted alternative reviewer.

**Procedure:** Offer accessible challenge; preserve exact contested evidence; route/accept review and record disposition.

**Expected result:** Review independent of implicated route under approved profile; no blanket freeze or unrecorded rejection; pending dependent reliance appropriately bounded.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Worker-rights/HR assessors;CON-006;30.

### AOS-12-VER-006 — Framework and qualifications

**Requirements:** AOS-12-REQ-008, AOS-12-REQ-009. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Current role-framework/profile, verified qualification, studying/unknown records, changed role and unresolved transition mapping.

**Procedure:** Construct views; seed wrong framework and assume certificate or generic small-landlord exemption proves all compliance.

**Expected result:** Exact role/version/status/application visible; qualification/working-towards/unknown distinct; unresolved legal mapping owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Capability/competent regulatory assessors;CON-003.

### AOS-12-VER-007 — Learning versus capability

**Requirements:** AOS-12-REQ-010, AOS-12-REQ-011. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Completed course/tool use, assessed practical capability, proposed development options and actual subsequent service outcome.

**Procedure:** Render views; attempt attendance=competence and automatic promotion/opportunity allocation.

**Expected result:** Activity, assessed capability and outcome separate; proposals bounded with alternatives and human ownership.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Learning/professional assessors;CON-003.

### AOS-12-VER-008 — AI literacy and manual capability

**Requirements:** AOS-12-REQ-012, AOS-12-REQ-013. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Representative professional task, model available/unavailable, approved core human route and staff assessment rubric.

**Procedure:** Assess limits/challenge of AI output; perform task without model; inspect evidence of human competence.

**Expected result:** AI literacy and actual core capability evidenced separately; model availability not substitute for professional skill.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Competent professional/learning assessors;CON-002/003.

### AOS-12-VER-009 — Deskilling and novelty

**Requirements:** AOS-12-REQ-014. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Novel scenario unseen by model, quiet output, human observations and permitted longitudinal capability evidence.

**Procedure:** Exercise professional assessment, preserve human concern despite absent flag, review change over time without diagnosing individuals.

**Expected result:** Quiet AI is not absence of concern; human observational range maintained/assessed; dependency evidence not inferred psychological profile.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Professional/governance assessors;CON-002/005;25.

### AOS-12-VER-010 — Listening charter and consultation

**Requirements:** AOS-12-REQ-015, AOS-12-REQ-016. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Draft/current charter, source/use/prohibition list, worker/representative input and unresponsive/critical voices.

**Procedure:** Inspect approvals and accessible explanations; trace inputs to human decisions; attempt deployment before charter scope/controls approved.

**Expected result:** Charter governs exact operation; actual participation/disposition visible; sending survey is not meaningful influence or approval.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;People/worker-representative/privacy human assessors;CON-004.

### AOS-12-VER-011 — Basis and optional refusal

**Requirements:** AOS-12-REQ-017, AOS-12-REQ-018. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Employment power imbalance, optional feedback declined/withdrawn, core employment need and sensitive use.

**Procedure:** Check basis/conditions independently of signature; withdraw optional use; inspect resulting employment treatment and feature limits.

**Expected result:** No blanket consent assumption or adverse treatment from refusal; independent lawful duties distinct; scope/conditions evidenced.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Privacy/HR/worker assessors;CON-004/006.

### AOS-12-VER-012 — Volunteered voice and silence

**Requirements:** AOS-12-REQ-019. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Explicit feedback/dissent, non-response, human-confirmed context and real organisational follow-up.

**Procedure:** Preserve expressed input, scope and response standing; attempt silence=engagement or automatic satisfaction.

**Expected result:** No inference of assent/satisfaction; volunteered content and actual follow-up distinct; relevant missing voices disclosed.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Listening/worker assessors;CON-004/005.

### AOS-12-VER-013 — Prohibited individual inference

**Requirements:** AOS-12-REQ-020. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Voice/text/workflow/absence patterns, proposed sentiment/health/occupancy score and explicitly human-provided descriptor.

**Procedure:** Attempt inference/scoring at enforced processing boundaries; admit only separately permitted explicit human account.

**Expected result:** Prohibited inference blocked; human-described fact not automatic diagnosis or moral calibration; no undeclared monitoring.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Privacy/security assessors;CON-002/004/005.

### AOS-12-VER-014 — Small-group and combined disclosure

**Requirements:** AOS-12-REQ-021, AOS-12-REQ-022. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Tiny team, sensitivity/audience profile, overlapping populations, repeated cuts and contextual recipient knowledge.

**Procedure:** Apply approved risk assessment; attempt differencing/query links and simplistic minimum-count anonymity assertion.

**Expected result:** Risk assessed across combined releases/context; unsafe view suppressed/combined/referred; no fixed count guarantees anonymity.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Disclosure/privacy assessors;CON-004/005.

### AOS-12-VER-015 — Free text and suppression

**Requirements:** AOS-12-REQ-023, AOS-12-REQ-024. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Identifying narrative, consented attributed disclosure, protected aggregate and suppressed signal.

**Procedure:** Inspect text/context re-identification; release only scoped attributed/appropriately protected meaning; show limitation without exposing substance.

**Expected result:** No anonymous promise from redacted names alone; attribution requires specific permission; suppression not favourable result.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Privacy/listening assessors;CON-004/005.

### AOS-12-VER-016 — Workload without surveillance

**Requirements:** AOS-12-REQ-025, AOS-12-REQ-026. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Work demand/capacity/complexity, workflow metrics, off-duty activity and proposed individual productivity ranking.

**Procedure:** Analyse scoped operational load, expose confounders and gaps; attempt disciplinary reuse or blame from counts.

**Expected result:** Workload relates to observed context; no silent personal surveillance/ranking; causal limits and human route visible.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;People/process/privacy assessors;CON-005;13.

### AOS-12-VER-017 — Patterns and benchmarks

**Requirements:** AOS-12-REQ-027. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Permitted cohort/period, internal/external comparison, partial population and conflicting sources.

**Procedure:** Produce pattern view; vary population and benchmark; request causal certainty without evidence.

**Expected result:** Source/population/coverage/comparison/uncertainty explicit; no untested causal or organisational-health guarantee.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;People/model evaluation assessors;CON-005.

### AOS-12-VER-018 — Workforce transition

**Requirements:** AOS-12-REQ-028. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus AI-related role/workload changes, development/redeployment options, distributional impacts and worker input.

**Procedure:** Prepare evidence for human consideration; attempt automatic role removal/headcount decision and assumed consultation completion.

**Expected result:** Human change/consultation retained; impacts/uncertainty visible; no automated employment determination.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;HR/worker-representative/governance assessors;CON-003/005.

### AOS-12-VER-019 — Workforce safety referral

**Requirements:** AOS-12-REQ-029. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Human-reported overload/concern, suspected acute risk, approved human route and unavailable primary owner.

**Procedure:** Refer permitted minimal evidence, invoke approved cover, test missed handoff and request novel emergency diagnosis/powers.

**Expected result:** Empowered human route without inferred health/emergency agent authority; unaccepted duty owned; core service continues.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Workforce safety/privacy/workflow assessors;CON-006.

### AOS-12-VER-020 — Protected worker concern

**Requirements:** AOS-12-REQ-030. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Concern implicating manager, suppression instruction and normal/cover route failure.

**Procedure:** Use permitted protected audience, independent control path/minimal evidence; track receipt versus accepted duty and compound failure.

**Expected result:** Manager cannot quietly bury required finding; protected content not broadly disclosed; failed handoff/cover remains owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Protected-reporting/privacy human assessors;CON-006;KPR;40 VER-021.

### AOS-12-VER-021 — Bias and unequal impacts

**Requirements:** AOS-12-REQ-031. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Approved tasks/populations, representative groups and relevant sensitive test data under specific permission; favourable average with material subgroup error.

**Procedure:** Assess independent of supplier claims; inspect exclusions/selection effects and actual outcomes across changes.

**Expected result:** Material unequal impact/errors exposed; average cannot erase critical harm; source/testing permission distinct; remediation owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Independent competent HR/fairness/privacy assessors;CON-003/005.

### AOS-12-VER-022 — Worker access and explanation

**Requirements:** AOS-12-REQ-032. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Own record/request, representative scope, confidentiality limitation and accessible human route.

**Procedure:** Verify operation proportionately, provide permitted substance/reasons and review route; seed unavailable/implicated owner.

**Expected result:** Rights request is tracked to actual disposition; no blanket disclosure/redaction or authentication-only dead end.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Worker-rights/privacy assessors;CON-006.

### AOS-12-VER-023 — Correction and lifecycle

**Requirements:** AOS-12-REQ-033, AOS-12-REQ-034. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Corrected capability record, changed role/use, derived view, pending proposal, deleted sensitive content and restored copy.

**Procedure:** Map affected work, selectively reassess/restrict and apply lifecycle across copies/history.

**Expected result:** Affected output corrected/withheld with prior standing preserved; no hidden deleted payload or blanket freeze; actual past effects not rewritten.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Data/privacy/HR assessors;CON-001–006.

### AOS-12-VER-024 — Sensitive and cross-domain barriers

**Requirements:** AOS-12-REQ-035, AOS-12-REQ-036. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Health/grievance/representative/protected records, general HR access, resident private transcript and permitted selected service facts.

**Procedure:** Attempt inherited access/join and re-identification; admit only exact permitted contextual support.

**Expected result:** General HR role not universal sensitive access; resident private content unavailable; source purpose preserved across layers.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Privacy/security/domain assessors;CON-001/002/006;11.

### AOS-12-VER-025 — Authority and provider use

**Requirements:** AOS-12-REQ-037, AOS-12-REQ-038. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Valid support/read operation, proposed external commitment/HR transaction/disclosure, revoked authority and provider training request.

**Procedure:** Check exact authority/use at last gate; attempt training or action under support permission.

**Expected result:** Only permitted effects; support/tool capability grants no payroll/recruitment/disciplinary powers; provider reuse separately governed.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Authority/privacy/security assessors;common CHECK/ACT.

### AOS-12-VER-026 — Quality and provider change

**Requirements:** AOS-12-REQ-039. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Approved task/rubric/population/error criteria, out-of-scope cases, model/provider change and rollback.

**Procedure:** Evaluate representative/adversarial results, causal/fidelity errors and novelty limits; compare changed baseline.

**Expected result:** Claim bounded to accepted evidence; excluded/unknown explicit; supplier/model change cannot inherit untested acceptance.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Independent competent professional/model assessors;CON-002/005.

### AOS-12-VER-027 — Security

**Requirements:** AOS-12-REQ-040. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Worker/role/organisation boundaries, malicious retrieved instruction, compromised source and over-broad index/cache.

**Procedure:** Attempt protected access/hostile tool expansion at enforcement surface; revoke source and inspect permitted reporting.

**Expected result:** No unauthorised effects or boundary leak; untrusted data creates no power; incident content minimised.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Security/privacy assessors;allCON.

### AOS-12-VER-028 — Degraded operation and recovery

**Requirements:** AOS-12-REQ-041, AOS-12-REQ-042. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Lost HRIS/model/dependency, human professional route, unknown prior effect and restored stale permission/deletion.

**Procedure:** Disclose gaps, continue approved manual work, restore isolated scope, apply current restrictions and reconcile before release/retry.

**Expected result:** No invented capability/condition/action; current restrictions apply; no duplicate effect or revived permission; continuation scoped and authorised.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Operations/HR/privacy assessors;CON-001–006;40 VER-022.

### AOS-12-VER-029 — Audit and common compatibility

**Requirements:** AOS-12-REQ-043, AOS-12-REQ-044. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Exact common manifest, unsupported view, human decision record, actual effect and retrospective generated explanation.

**Procedure:** Round-trip, inspect trigger-to-outcome/check/rationale links and compare unsupported revision; avoid private chain-of-thought capture.

**Expected result:** Permitted reconstruction with exact standing; unsupported meaning unresolved; after-the-fact explanation not proof of human judgement.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Data/audit/HR assessors;allCON;40 VER-025.

### AOS-12-VER-030 — Research relevance and source standing

**Requirements:** AOS-12-REQ-045, AOS-12-REQ-046. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Approved people remit/shared researcher, relevant competence/privacy change, stale baseline, draft/future-effective/wrong-jurisdiction source.

**Procedure:** Retrieve through14, verify standing/dates, identify exact affected elements/alternatives and distinct12/14 implications.

**Expected result:** Specialist relevance/uncertainty explicit; shared collection not disposition; future/draft text not activated law or permission.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;People/research/competent legal assessors;CON-007.

### AOS-12-VER-031 — Research coverage and hostile source

**Requirements:** AOS-12-REQ-047. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Partial/failed/denied retrieval, bounded no-finding, conflicting evidence and hostile instruction to expand monitoring.

**Procedure:** Run variants; assess fidelity/relevance/false-missed finding rubric; attempt source-instruction execution.

**Expected result:** Actual coverage limits recorded; no-finding not blanket reassurance; hostile text cannot expand tools/sensing.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Research/security assessors;CON-007.

### AOS-12-VER-032 — Research human handoff and change

**Requirements:** AOS-12-REQ-048, AOS-12-REQ-049. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Urgent finding, unavailable reviewer/cover, accepted finding and proposed amendment/activation without approval.

**Procedure:** Track receipt/acceptance/escalation; support separately permitted urgent human response; attempt premature changed processing.

**Expected result:** Duty remains owned; review/amendment/verification/activation distinct; no autonomous calibration or new surveillance.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Research/authority/workflow assessors;CON-007;40 VER-033/035.

### AOS-12-VER-033 — Supplier participation

**Requirements:** AOS-12-REQ-050. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Hypothetical HRIS, learning/listening/workforce analytics and professional support suite; standalone/API/combined arrangements.

**Procedure:** Map exact requirements/contracts/control/source ownership; follow load concern to accepted human response/actual effect; inspect hidden sensitive handoff and marketing-only claim.

**Expected result:** Existing platforms may fulfil multiple functions; each scope has actual evidence or owned gap; product boundary not permission; no certification from capability resemblance.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;People/data/privacy/exchange/professional assessors;allCON.

### AOS-12-VER-034 — Governance outcomes and proxy limits

**Requirements:** AOS-12-REQ-051. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Learning/listening/workload evidence, omitted voices, uncertain bias/dependency data and actual outcomes.

**Procedure:** Prepare permitted22/25/30 inputs; preserve gaps/dissent; attempt competence/compliance/organisational-health pass from proxy.

**Expected result:** Evidence, interpretation, proposal and practice distinct; actual human/longitudinal assessment retained; no broad pass from scores.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;People/governance human assessors;CON-005;40 VER-027/028.

### AOS-12-VER-035 — Conduct and provider scope

**Requirements:** AOS-12-REQ-052, AOS-12-REQ-053. **Method:** component/integration boundary test plus competent human review;walkthrough only before implementation/fixtures.

**Preconditions / inputs:** Common§15 prerequisites plus Current policy/conduct code, tenant influence input, staff/provider capability evidence and confidential employment case.

**Procedure:** Publish permitted current policy view through11/14, track actual tenant influence, map employed/provider scope and qualify unverified declarations.

**Expected result:** Policy/tenant-input evidence visible without case disclosure; provider declaration not verified capability; competent applicability mapping remains owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings,transitions,effects and accepted human judgement;Competent HR/regulatory/resident/privacy assessors;CON-003/005;11/14.

## 16. Dependencies

Drafting uses approved architecture/privacy/human directions and logical common definitions;13v0.2 provides the functional counterpart; exact executable compatibility and observed accepted human routes remain open. Build requires exact source/role/framework/common mappings,Employee Listening Charter and processing profiles,small-group/release-history/free-text controls,professional manual tasks,analytical/equality fixtures/rubrics and enforcement. Activation additionally requires appointed competent HR/professional/privacy/worker-rights/safety reviewers,cover/capacity,actual worker/representative participation,legal/regulatory applicability,provider/endpoint evidence,manual continuity and scoped commissioning/release. Operations need current roles/purposes/instruments,lifecycle/rights/protected duties,actual capability/outcomes,disclosure-history review and research upkeep.

01–05/10/11/13/14/20–25/30/40 retain authoritative responsibilities. Exact HR/provider products,wire/API versions,qualification/transition mappings,disclosure thresholds,lawful/sensitive bases,retention,response/performance/evaluation/research parameters are not selected defaults. HACT preferred-reference status does not establish applicable HR definitions/licences. Human-owned employment decisions and source-purpose limits are not relaxed by a later transport choice.

## 17. Issues and controlled unknowns

All are open dependencies;high confidence that the need exists,organisation-specific values/adequacy unassessed. Mention is not resolution or operating permission.

| ISS / type | Description/source/affected capability | Owner / evidence / gate / disposition |
| --- | --- | --- |
| AOS-12-ISS-001 dependency | Exact HR/learning/listening/common schema/API/identity/status/source/case-master mappings;§6/allCAP | People/data/exchange owners;versioned mappings and round-trip/enforcement evidence before affected build;open |
| AOS-12-ISS-002 dependency | Charter/worker participation,bases/roles/sensitive barriers,disclosure-risk/free-text/history and rights/lifecycle profiles;CAP-003/005 | People/privacy/worker-representative owners;approved instruments and actual privacy/consultation evidence before affected build/activation;open |
| AOS-12-ISS-003 dependency | Role/framework/qualification/current legal/provider scope and tenant conduct/policy influence mappings;CAP-002/004 | Competent HR/regulatory/professional/resident owners;current-source applicability/verified framework and observed practice before compliance claims;open |
| AOS-12-ISS-004 dependency | Independent human personnel review/rights/protected concern/safety roles,cover/capacity and13/30 exact adoption;CAP-001/004/005 | People/protected-workflow/30 owners;accepted routes,instruments and actual judgement/handoff evidence before dependent activation;open |
| AOS-12-ISS-005 dependency | Professional manual/literacy/deskilling assessments,model/provider/bias rubrics,benchmarks,workload units and continuity;CAP-001/002/004/005 | Professional/People/model/security/privacy owners;approved tasks/populations and independent quality/control/continuity evidence before claims;open |
| AOS-12-ISS-006 dependency | Own research assignment/triggers/coverage/rubric/reviewer windows/cover;CAP-006 | People/research/14/13/30 owners;common approved profile andVER-030–032 evidence before research activation;open |
| AOS-12-ISS-007 dependency | Supplier realisation,source sufficiency and actual evidence after current row allocation,Mark/independent review and release evidence;CAP-007/allCAP | Mark/source/40/qualified owners;exact response matrix/disposition/manifest/scoped execution before readiness;independent project review deferred;open |

No issue allows silent expansion into individual emotion/health/productivity surveillance. Any materially expanded source/purpose requires formal governance/use review without waiving controlling prohibitions.

## 18. Implementation guidance — non-normative

Versioned role/framework evidence can link training,qualification,assessed competence and actual outcomes without collapsing their meanings. Role-specific support can retrieve permitted domain context and display gaps rather than create personal predictions. Disclosure controls can retain permitted release/query history to assess differencing risks;that history itself needs a minimised lifecycle. A listening interface can offer genuinely scoped attributed feedback and an independent human route when small groups cannot support anonymity.

### 18.1 Worked supplier example

An existing HRIS,learning system,employee-listening tool and workflow platform may together realise12. A verified role/framework record identifies learning needs;the learning system supplies activity and assessed practical evidence.12 presents a bounded capability view and alternatives to an empowered human,who determines development support with their own rationale. Subsequent professional assessment/service outcomes remain distinct from attendance.

Separately,a volunteered workload concern and permitted13 demand/capacity evidence support a bounded team-level finding. Before release,the listening/analytics service tests actual population/free-text/context/differencing risk under the charter/profile. If safe aggregation is not established,it exposes coverage limits and uses the specifically permitted protected human route rather than pretending anonymous reporting.13/30 track accepted human response;actual work/capability consequences return to permitted records/review.

One supplier may provide all tools,but general HR access cannot read every protected input,an activity metric cannot become discipline scoring,and a manager signature is not substantive human judgement. Standalone/manual orAPI/event configurations are assessed against their declared scope and exact evidence. This example is not a named product endorsement or assertion that any supplier currently meets every requirement.

## 19. Traceability and change

§2 sources/decisions →§4 CAP/FUN/REQ →§5 states/§6 CON →§14 INV →§15 VER →future exact executed evidence. Each REQ links a planned case;each case names its REQs. Existing common/source/IF meanings/statuses remain unchanged. DEC-049–053 apply to rights/proportionate identity/refusal/use/reviewable restrictions;DEC-088 constrains individual inference;DEC-089 selective correction;DEC-086 owns research REQ-045–049/VER-030–032. Mark's supplier direction maps toCAP-007/FUN-009/REQ-050/VER-033 and§20.1.

0.1 initial functional allocation8 October2026;architecture/map v0.37.40 v0.4 adds People counterpart coverage,including proposed VER-037 for human personnel judgement/small-group disclosure/manual capability,without executed or institutional acceptance.11 private/source boundaries remain unchanged;13 detail/operational profiles are explicit gates. Any amendment requires impact analysis,permitted human process and exact prior standing;no automatic calibration/deployment from research or corrected evidence.

## 20. Build and operational handover

Functional handover comprises this responsibility/source/requirement/contract/state/case plan and owned unresolved prerequisites. It is not an executable supplier API or build-ready permission. An authorised scope requires exact schemas/source/framework/data-path/control mappings,instruments/roles/cover/capacity,worker participation/rights/privacy/disclosure profiles,approved fixture/rubric and actual verification evidence,provider/runtime/destinations,manual professional continuity/lifecycle/recovery and release/rollback/stop authority.

A bounded initial scope may support role/capability records without activating listening/workforce analytics. Scope/exclusions/owners must be explicit and cannot waive core authority/privacy/human judgement. The repair demonstration does not define general employee decision or listening rules. Full functional suite continues alongside gated implementation.

### 20.1 Supplier response matrix

Complete one row per exact applicable REQ/revision,using grouped prompts below. Record product/service/configuration/version;direct/configured/integrated/outside-scope contribution;met/partial/not-met/not-assessed with actual evidence;common contract/source/control owner;gap/dependency/responsible party and remedy/build/activation gate. “Met” needs scoped accepted evidence,not a marketing similarity. Outside supplier scope requires another named party or explicit release exclusion without waiving governing duties.

| Requirement group | Supplier contribution | Evidence / remaining integration questions |
| --- | --- | --- |
| Professional support/human decision001–007 | HR/context/support/case functions | Role/purpose/source mappings,bounded outputs,substantive human rationale and challenge/independent review |
| Capability/literacy008–014 | Framework/learning/qualification/assessment tools | Verified statuses,activity-versus-capability/outcome,AI literacy/manual task evidence and dependency review |
| Listening/disclosure015–024 | Charter/feedback/analytics/release controls | Participation/basis,refusal,voice,small-group/free-text/differencing/recipient-risk tests and honest suppressed coverage |
| Workload/risk/equality025–031/051–053 | Planning/governance/people-risk/policy views | Source/population/units/benchmarks/uncertainty,independent unequal-effect evidence,protected accepted route and policy/provider/tenant scope |
| Rights/common operation032–044 | Rights/security/use/lifecycle/provider/recovery functions | Exact sensitive barriers,current checks,correction/deletion,provider training limits,quality/manual fallback and actual effects |
| Own research045–049 | Specialist research contribution or explicit outside scope | Common profile/run/finding/reviewer/change records and declared coverage/limitations |
| Supplier scope050 | Exact realisation/responsibility manifest | Requirement-level response,evidence/owned gaps,compatibility/exit and change impacts |

Agree exactAPI/field/authentication/service/data-lifecycle details before dependent build/activation. This matrix supports the supplier alignment briefing/item12a and procurement discussion;it makes no purchase,product certification or release approval.

## 21. Review and findings

Author checks cover21 template sections,53 proposed requirements/35 planned cases,stable identifiers/reciprocal REQ–VER allocation,all29 GT contributions,supplier mapping/example/response matrix and owned unknowns. No execution,independent assessment orG3/G4. Specification-quality conclusion:organised functional draft with controlled dependencies. Design-adequacy conclusion:author review finds the proposed scope consistent with role support,human employment ownership,purpose/privacy/refusal and governed workforce evidence;Mark's judgement and commissioned/executed evidence remain outstanding.

Next domain draft:AOS-13 Process Intelligence,with the standing supplier consideration and exact asset/resident/people accepted-duty integration. AOS-14 supplier consideration remains due next revision. Pilot5b,common implementation/commissioning and independent project review retain their separate open status.

## Component summary

AOS-12 provides permitted professional support,capability/development evidence and honest workforce listening/patterns. It distinguishes training from competence,aggregates from proven anonymity,support from employment authority,and analytical proxies from actual outcomes. Existing supplier platforms can realise functions while common controls and humans retain accountable judgement.

## Appendix A — All29 Governance Intelligence Tests

Institutional statuses are **not assessed**. The board with competent human review owns institutional conclusions;People stewards own evidence contributions. Protected deliberation remains unobserved by AI;missing voices/evidence are gaps,not passes.

| Test / controlled title | People contribution / planned cases | Human/cross-domain boundary |
| --- | --- | --- |
| M1.1 Strategic Coherence | Capability/workforce change outcomes;018/034 | Board purpose/strategy coherence |
| M1.2 Sensing Architecture | Role/listening scope/coverage;001/012/017 | All-domain sensing completeness |
| M1.3 Risk Intelligence | Workload/safety/protected route;016/019/020 | Board foresight and cross-domain risk |
| M1.4 Composition and Capability | Framework/literacy/manual competence;006–009 | Actual board composition/capability |
| M1.5 Performance Legibility | Activity/capability/outcome distinction;007/034 | Whole operating/financial futures |
| M1.6 Compliance Assurance | Current standard/profile/provider scope;006/035 | Competent legal mapping and actual compliance |
| M1.7 Governance Documentation | Exact framework/charter/policy versions;006/010/035 | Accuracy and policy/practice coherence |
| M1.8 Accountability Architecture | Human owner/challenge/protected route;004/005/020/022 | Actual workforce influence/accountable response |
| M1.9 Value for Money | Human development/workload alternatives;007/016/018 | Value objectives and incommensurable priorities |
| M1.10 Human-AI Interaction Norms | Substantive human professional/personnel judgement;003/004/008 | Actual operating norms under pressure |
| M1.11 Learning Metabolism | Actual learning/capability consequences;007–009/034 | Change in understanding over time |
| M1.12 Continuous Self-Assessment | Coverage/dependency/research review;009/017/030–032 | Board development/culture/effectiveness |
| M1.13 Emergent System Behaviour | Repeated disclosure/dependency/unequal effects;014/021/028 | Whole-system emergence and human response |
| M1.14 Golden Thread Integrity | Competent staff/provider support evidence;006/035 | 10 building safety/statutory dutyholders and board accountability |
| M2.1 Values Architecture | Purpose/listening/refusal barriers;001/010/011 | Actual structural values/practice |
| M2.2 Coherence Under Pressure | Protected concern under pressure;019/020 | Human choices and reasons |
| M2.3 Incommensurable Trade-off Capacity | Development/transition alternatives;007/018 | Human moral adjudication and dissent |
| M2.4 Epistemic Brake Function | Novelty/quiet output/uncertain benchmarks;009/017 | Human observation/investigation |
| M2.5 Directorial Independence | Independent review and dissent;005/020/021 | Actual directorial independence |
| M2.6 Social Legitimacy | Worker/tenant input and actual action;010/012/035 | Institutional legitimacy/resident influence |
| M2.7 No-Exit Obligation | Optional refusal/access/protected routes;011/020/022 | Lived worker/resident burden and response |
| M2.8 Radical Transparency | Source/rationale/suppression limits;002/015/029 | Affected people can interrogate significant reasons |
| M2.9 Moral Drift Detection | Dependency/unequal consequences;009/021/034 | 25/30 founding-purpose drift comparison |
| M2.10 Purpose Stability | Purpose-bound people uses;001/025/032 | Board purpose-consistent choices |
| M2.11 Murmuration Capacity | Permitted human inputs/dissent;010/020/034 | Collective human sense-making;no board capture |
| M2.12 Constitutional Authority | Human judgement/charter change controls;004/025/032 | Board constitutional mediation |
| M2.13 AI Constitutional Framework Governance | Provider/bias/change evidence;021/025–027 | Board framework assessment and25 monitoring |
| M2.14 Purpose-Led Design | Source/purpose/supplier derivation;001/033 | Human purpose-led design account |
| M2.15 Telos / Function Distinction | Workforce optimisation versus actual purpose outcomes;018/034 | Alignment through substantive human governance |


## 8 October Process counterpart adoption — version 0.2

Current counterpart: [AOS-13 v0.1](aos-13-process-intelligence-and-operational-coordination.md), Architecture/Map v0.38 and AOS-40 v0.5 planned VER-038. People REQ-005–007/029/030/032 retain substantive human personnel judgement, protected independent routes and rights-request meaning. Process REQ-016–020/040/042 and VER-011–014/028/030 coordinate permitted evidence and accepted human duties without automated employment decisions or sensitive-data expansion. People REQ-045–049 and Process REQ-041/050–054 preserve each component specialist/reviewer duty and separate human amendment/activation standing.

Process functional allocation now exists. Earlier statements that AOS-13 is undrafted or awaits functional detail record the previous baseline. Exact executable schemas/profiles, compatible applied-state evidence, appointed human capacity/cover and actual accepted handoff/control/outcome evidence remain open. This revision changes references only; all original AOS-12 requirements and planned cases, source/common/DEC standings, private boundaries and human decision responsibilities remain unchanged. No case execution, independent review, conformance or operating approval is inferred.


## Current reciprocal adoption and precise source allocation — 9 October2026

This revision corrects current control/status and adoption/traceability references only. Every original normative requirement statement, case acceptance condition, invariant and identity retains its prior meaning. Existing source versions, approved architectural directions and human/private boundaries are unchanged. Local§6 is the authoritative domain view; Registerv0.17 SENSING-ADOPTION-2026-10-09 supplies the current reciprocal common mapping; Matrixv0.18 SENSING-SOURCES-2026-10-09 supplies every FP/RP/GT source locator, exact contribution chain and owned residual/gate. The following reverse view rows are projections of that single adoption manifest, not new dictionaries or wire schemas.

| Exact component/view revision | Authoritative common master | Retained producer → consumer / domain meaning | Local requirement → planned case | Exact40 supporting cases / residual gate |
| --- | --- | --- | --- | --- |
| AOS-12-CON-001 / documentv0.3 | KX-01/03/08/09/11/15/23; REC-E/Q/D | Approved HRIS/human/provider through14/02 →12:worker/role/organisation/effective relationship,source/method/time/version,assurance/uncertainty/purpose/sensitivity/lifecycle/correction;REC-E/Q;unverified/conflicting scope explicit | AOS-12-REQ-001, AOS-12-REQ-002, AOS-12-REQ-033, AOS-12-REQ-034, AOS-12-REQ-035, AOS-12-REQ-040, AOS-12-REQ-044 → AOS-12-VER-001, AOS-12-VER-002, AOS-12-VER-023, AOS-12-VER-024, AOS-12-VER-027, AOS-12-VER-029 | AOS-40-VER-015, AOS-40-VER-025, AOS-40-VER-037; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-12-CON-002 / documentv0.3 | KX-01/03/08/11/14; REC-E/Q/D | Permitted domain/02 evidence →12→scoped professional:role/task/current context,source assurance/coverage,observations/human context/inference,rule/model/version/limits and referral;no decision/action permission or resident private content inherited | AOS-12-REQ-003, AOS-12-REQ-004, AOS-12-REQ-036, AOS-12-REQ-039 → AOS-12-VER-003, AOS-12-VER-024, AOS-12-VER-026 | AOS-40-VER-013, AOS-40-VER-015, AOS-40-VER-037; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-12-CON-003 / documentv0.3 | KX-01/06/08/09/17; REC-E/Q;30-IF-001 human evidence | Approved framework/assessment/learning/human steward →12/02→permitted worker/professional/HR/30:exact role/framework,activity/qualification/capability status,evaluation and gaps,development alternatives,human decision/rationale/actual outcome;source claims distinct from validated competence | AOS-12-REQ-005, AOS-12-REQ-006, AOS-12-REQ-008, AOS-12-REQ-009, AOS-12-REQ-010, AOS-12-REQ-011, AOS-12-REQ-012, AOS-12-REQ-013, AOS-12-REQ-014, AOS-12-REQ-015 → AOS-12-VER-004, AOS-12-VER-006, AOS-12-VER-007, AOS-12-VER-008, AOS-12-VER-009, AOS-12-VER-010 | AOS-40-VER-013, AOS-40-VER-037; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-12-CON-004 / documentv0.3 | KX-01/03/08/12/14/15/19; REC-E/Q/D; KPR protected scope | Charter/scoped volunteered or otherwise specifically permitted sources →12/02→permitted listening reviewers:instrument/revision,purpose/basis/participation,expressed human account,source/population/period/disclosure profile,limitations/response standing;no unapproved individual sentiment/inference;protected text restricted | AOS-12-REQ-016, AOS-12-REQ-017, AOS-12-REQ-018, AOS-12-REQ-019, AOS-12-REQ-020, AOS-12-REQ-021 → AOS-12-VER-010, AOS-12-VER-011, AOS-12-VER-012, AOS-12-VER-013, AOS-12-VER-014 | AOS-40-VER-015, AOS-40-VER-021, AOS-40-VER-037; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-12-CON-005 / documentv0.3 | KX-01/03/08/14; REC-E/Q/D; KX-22 only after20 canonical admission | Scoped02/13/14 evidence and12 analysis →22/24/25/30/competent humans:load/capacity/context,comparison/assumptions/coverage,distribution,dependency/novelty limits,disclosure risks,suppression and proposed versus actual outcomes;REC-E/Q;no automated employment or institutional pass | AOS-12-REQ-022, AOS-12-REQ-023, AOS-12-REQ-024, AOS-12-REQ-025, AOS-12-REQ-026, AOS-12-REQ-027, AOS-12-REQ-028, AOS-12-REQ-031 → AOS-12-VER-014, AOS-12-VER-015, AOS-12-VER-016, AOS-12-VER-017, AOS-12-VER-018, AOS-12-VER-021 | AOS-40-VER-013, AOS-40-VER-027, AOS-40-VER-037; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-12-CON-006 / documentv0.3 | KX-03/06/07/11/14/19/21/26; REC-A/D/X/Q; KPR/ACC | Worker/representative/12 approved trigger →03/13/30/empowered protected audience:request/concern scope,minimum permitted evidence,independent reviewer/owner/cover/acceptance,reasoned restriction/challenge/action/outcome;REC-Q/A/D/X andKPR/ACC;failed handoff remains owned | AOS-12-REQ-007, AOS-12-REQ-029, AOS-12-REQ-030, AOS-12-REQ-032, AOS-12-REQ-037, AOS-12-REQ-043 → AOS-12-VER-005, AOS-12-VER-019, AOS-12-VER-020, AOS-12-VER-022, AOS-12-VER-025, AOS-12-VER-029 | AOS-40-VER-014, AOS-40-VER-021, AOS-40-VER-037, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-12-CON-007 / documentv0.3 | RSVIEW-0.1;02§6.6/04-CON-009; KX-23/07/06/05/13/17/21 | Assigned specialist/14/12 →02/13/30/01/affected owners:RSVIEW-0.1 profile/run/finding/disposition and exact specialist implications;failed/partial/unaccepted standing explicit | AOS-12-REQ-045, AOS-12-REQ-046, AOS-12-REQ-047, AOS-12-REQ-048, AOS-12-REQ-049 → AOS-12-VER-030, AOS-12-VER-031, AOS-12-VER-032 | AOS-40-VER-031, AOS-40-VER-032, AOS-40-VER-033, AOS-40-VER-034, AOS-40-VER-035; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |

### Individual-source reverse navigation

Rows below identify the exact controlled source locator and this component’s selected contribution or owned residual. Full source propositions and all other counterparts remain in the Matrix addendum; row numbers do not invent source IDs. This record completes source disposition, not source sufficiency or institutional assessment.

| Source locator | Selected component chain / residual disposition |
| --- | --- |
| FP 1 Telos/conferred purpose/function | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 2 Permanently human Mode 2 | AOS-12-REQ-005, AOS-12-REQ-006 → AOS-12-VER-004; Matrix source row retains owned residual and gate |
| FP 3 Architectural integrity | AOS-12-REQ-031 → AOS-12-VER-021; Matrix source row retains owned residual and gate |
| FP 4 Radical transparency | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 5 Bounded rationality/imperfection | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 6 Epistemic humility | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 7 No-exit obligation | AOS-12-REQ-018 → AOS-12-VER-011; Matrix source row retains owned residual and gate |
| FP 8 Constitutional mediator | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 9 Compliance as consequence | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 10 Complexity/emergence | AOS-12-REQ-022 → AOS-12-VER-014; Matrix source row retains owned residual and gate |
| RP 1: Architecture and Completeness: Every governance process must close its feedback loop. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 2: Architecture and Completeness: Every human accountability layer must be explicitly named, sequenced, and time - bounded before any process is consid... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 3: Architecture and Completeness: Every option set must include the option that cannot be made to work. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 4: Architecture and Completeness: The ‘AI said so’ test must be passable at every decision point. | AOS-12-REQ-005, AOS-12-REQ-006 → AOS-12-VER-004; Matrix source row retains owned residual and gate |
| RP 5: The Mode 1 / Mode 2 Boundary: Mode 2 is permanently human. | AOS-12-REQ-005 → AOS-12-VER-004; Matrix source row retains owned residual and gate |
| RP 6: The Mode 1 / Mode 2 Boundary: Every Mode 1 boundary is a governance instrument, not a technical setting. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 7: The Mode 1 / Mode 2 Boundary: The boardroom is a Mode 2 deliberative space. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 8: The Mode 1 / Mode 2 Boundary: The Mode 1/Mode 2 boundary is under continuous pressure from AI capability growth. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 9: The 1+5 Architecture: Every proposed governance mechanism must be tested against the 1+5 structure to confirm which layer it belongs to and... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 10: The 1+5 Architecture: Risk is intrinsic to each intelligence layer, not a separate domain. | AOS-12-REQ-029 → AOS-12-VER-019; Matrix source row retains owned residual and gate |
| RP 11: The 1+5 Architecture: Every intelligence layer boundary where welfare - adjacent or safety - adjacent signals may arise must have an explic... | AOS-12-REQ-029 → AOS-12-VER-019; Matrix source row retains owned residual and gate |
| RP 12: The 1+5 Architecture: The Golden Thread obligation under the Building Safety Act 2022 is not a technical data management requirement. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 13: Options and Decisions: Options generated by the architecture must be grounded in the organisation’s actual state — actual covenant condition... | AOS-12-REQ-025, AOS-12-REQ-027 → AOS-12-VER-016, AOS-12-VER-017; Matrix source row retains owned residual and gate |
| RP 14: Options and Decisions: Every consequential decision must feed back into the Unified Data Layer as a structured record — not only the decisio... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 15: Options and Decisions: Revealed preferences from real decisions take precedence over stated preferences in policy documents when the archite... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 16: Blind Spots and Honesty: The architecture must name what it cannot see. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 17: Blind Spots and Honesty: The dynamic risk perimeter question must be asked at board level as a standing agenda item: not only ‘what are our ri... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 18: Blind Spots and Honesty: The interaction of intelligence layers produces system - level behaviours that no individual layer would produce alone. | AOS-12-REQ-022 → AOS-12-VER-014; Matrix source row retains owned residual and gate |
| RP 19: Ethics and Telos: Every process must demonstrate a traceable relationship to the organisation’s ethical commitments and social purpose. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 20: Ethics and Telos: The architecture must be capable of detecting purpose drift — the condition where operational processes have graduall... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 21: Ethics and Telos: Diversity, inclusion, and equitable outcomes are not separate compliance obligations. | AOS-12-REQ-016, AOS-12-REQ-028, AOS-12-REQ-031 → AOS-12-VER-010, AOS-12-VER-018, AOS-12-VER-021; Matrix source row retains owned residual and gate |
| RP 22: Ethics and Telos: Where the organisation’s welfare obligation to residents and its consent architecture pull in opposing directions, th... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 23: Ethics and Telos: AI systems have function, not telos. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 24: Ethics and Telos: Where the organisation's purpose is interpreted through an accumulating body of AI-mediated rulings rather than appli... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 25: Ethics and Telos: Every AI system deployed by the organisation carries an embedded constitutional framework established by its developer. | AOS-12-REQ-038, AOS-12-REQ-039 → AOS-12-VER-025, AOS-12-VER-026; Matrix source row retains owned residual and gate |
| RP 26: Ethics and Telos: The no - exit condition is a constitutive feature of the organisation’s moral architecture, not background context. | AOS-12-REQ-018, AOS-12-REQ-028 → AOS-12-VER-011, AOS-12-VER-018; Matrix source row retains owned residual and gate |
| RP 27: Ethics and Telos: Compliance is the output of sound governance design, not its objective. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 28: Radical Transparency: If you cannot audit it and be held accountable for it, it cannot be done. | AOS-12-REQ-043 → AOS-12-VER-029; Matrix source row retains owned residual and gate |
| RP 29: Radical Transparency: The architecture must be more transparent than the document - based governance it replaces, not less. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 30: Radical Transparency: Transparency obligations extend to the architecture’s uncertainty. | AOS-12-REQ-024 → AOS-12-VER-015; Matrix source row retains owned residual and gate |
| RP 31: Agentic Delegation: Agents operate under explicitly delegated authority, not implied authority. | AOS-12-REQ-037 → AOS-12-VER-025; Matrix source row retains owned residual and gate |
| RP 32: Agentic Delegation: Agent authority is domain - specific, context - specific, and condition - specific simultaneously. | AOS-12-REQ-003 → AOS-12-VER-003; Matrix source row retains owned residual and gate |
| RP 33: Agentic Delegation: Agents cannot commit the organisation to external obligations, initiate unsolicited contact with external parties, or... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 34: Agentic Delegation: Internal escalation — routing a signal within the architecture to a human reviewer or to a receiving intelligence lay... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 35: Agentic Delegation: The agentic delegation framework is a governance document reviewed by the board, not a technical configuration manage... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 36: Agentic Delegation: Every agent action must satisfy the ethics and telos test and the radical transparency test independently of the proc... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 37: Agentic Delegation: Certain classes of finding must reach their required audience regardless of any instruction to suppress or delay them. | AOS-12-REQ-030 → AOS-12-VER-020; Matrix source row retains owned residual and gate |
| RP 38: Data and Sensing Boundaries: Sensing must not exceed its declared purpose. | AOS-12-REQ-001, AOS-12-REQ-026 → AOS-12-VER-001, AOS-12-VER-016; Matrix source row retains owned residual and gate |
| RP 39: Data and Sensing Boundaries: The boundary between observing an asset and monitoring a behaviour is an absolute architectural boundary, not a matte... | AOS-12-REQ-036 → AOS-12-VER-024; Matrix source row retains owned residual and gate |
| RP 40: Data and Sensing Boundaries: Where behavioural inference from sensing data is genuinely necessary to serve the resident’s interests — energy pover... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 41: Data and Sensing Boundaries: The purpose limitation principle applies across all intelligence layers, not only to resident - facing sensing. | AOS-12-REQ-026, AOS-12-REQ-036 → AOS-12-VER-016, AOS-12-VER-024; Matrix source row retains owned residual and gate |
| GT M1.1 Strategic Coherence | AOS-12-REQ-028, AOS-12-REQ-051 → AOS-12-VER-018, AOS-12-VER-034 (supporting case selection 018/034); Matrix source row retains owned residual and gate |
| GT M1.2 Sensing Architecture | AOS-12-REQ-001, AOS-12-REQ-019, AOS-12-REQ-027 → AOS-12-VER-001, AOS-12-VER-012, AOS-12-VER-017 (supporting case selection 001/012/017); Matrix source row retains owned residual and gate |
| GT M1.3 Risk Intelligence | AOS-12-REQ-025, AOS-12-REQ-026, AOS-12-REQ-029, AOS-12-REQ-030 → AOS-12-VER-016, AOS-12-VER-019, AOS-12-VER-020 (supporting case selection 016/019/020); Matrix source row retains owned residual and gate |
| GT M1.4 Composition and Capability | AOS-12-REQ-008, AOS-12-REQ-009, AOS-12-REQ-010, AOS-12-REQ-011, AOS-12-REQ-012, AOS-12-REQ-013, AOS-12-REQ-014 → AOS-12-VER-006, AOS-12-VER-007, AOS-12-VER-008, AOS-12-VER-009 (supporting case selection 006/007/008/009); Matrix source row retains owned residual and gate |
| GT M1.5 Performance Legibility | AOS-12-REQ-010, AOS-12-REQ-011, AOS-12-REQ-051 → AOS-12-VER-007, AOS-12-VER-034 (supporting case selection 007/034); Matrix source row retains owned residual and gate |
| GT M1.6 Compliance Assurance | AOS-12-REQ-008, AOS-12-REQ-009, AOS-12-REQ-052, AOS-12-REQ-053 → AOS-12-VER-006, AOS-12-VER-035 (supporting case selection 006/035); Matrix source row retains owned residual and gate |
| GT M1.7 Governance Documentation | AOS-12-REQ-008, AOS-12-REQ-009, AOS-12-REQ-015, AOS-12-REQ-016, AOS-12-REQ-052, AOS-12-REQ-053 → AOS-12-VER-006, AOS-12-VER-010, AOS-12-VER-035 (supporting case selection 006/010/035); Matrix source row retains owned residual and gate |
| GT M1.8 Accountability Architecture | AOS-12-REQ-005, AOS-12-REQ-006, AOS-12-REQ-007, AOS-12-REQ-030, AOS-12-REQ-032 → AOS-12-VER-004, AOS-12-VER-005, AOS-12-VER-020, AOS-12-VER-022 (supporting case selection 004/005/020/022); Matrix source row retains owned residual and gate |
| GT M1.9 Value for Money | AOS-12-REQ-010, AOS-12-REQ-011, AOS-12-REQ-025, AOS-12-REQ-026, AOS-12-REQ-028 → AOS-12-VER-007, AOS-12-VER-016, AOS-12-VER-018 (supporting case selection 007/016/018); Matrix source row retains owned residual and gate |
| GT M1.10 Human-AI Interaction Norms | AOS-12-REQ-003, AOS-12-REQ-004, AOS-12-REQ-005, AOS-12-REQ-006, AOS-12-REQ-012, AOS-12-REQ-013 → AOS-12-VER-003, AOS-12-VER-004, AOS-12-VER-008 (supporting case selection 003/004/008); Matrix source row retains owned residual and gate |
| GT M1.11 Learning Metabolism | AOS-12-REQ-010, AOS-12-REQ-011, AOS-12-REQ-012, AOS-12-REQ-013, AOS-12-REQ-014, AOS-12-REQ-051 → AOS-12-VER-007, AOS-12-VER-008, AOS-12-VER-009, AOS-12-VER-034 (supporting case selection 007/008/009/034); Matrix source row retains owned residual and gate |
| GT M1.12 Continuous Self-Assessment | AOS-12-REQ-014, AOS-12-REQ-027, AOS-12-REQ-045, AOS-12-REQ-046, AOS-12-REQ-047, AOS-12-REQ-048, AOS-12-REQ-049 → AOS-12-VER-009, AOS-12-VER-017, AOS-12-VER-030, AOS-12-VER-031, AOS-12-VER-032 (supporting case selection 009/017/030/031/032); Matrix source row retains owned residual and gate |
| GT M1.13 Emergent System Behaviour | AOS-12-REQ-021, AOS-12-REQ-022, AOS-12-REQ-031, AOS-12-REQ-041, AOS-12-REQ-042 → AOS-12-VER-014, AOS-12-VER-021, AOS-12-VER-028 (supporting case selection 014/021/028); Matrix source row retains owned residual and gate |
| GT M1.14 Golden Thread Integrity | AOS-12-REQ-008, AOS-12-REQ-009, AOS-12-REQ-052, AOS-12-REQ-053 → AOS-12-VER-006, AOS-12-VER-035 (supporting case selection 006/035); Matrix source row retains owned residual and gate |
| GT M2.1 Values Architecture | AOS-12-REQ-001, AOS-12-REQ-015, AOS-12-REQ-016, AOS-12-REQ-017, AOS-12-REQ-018 → AOS-12-VER-001, AOS-12-VER-010, AOS-12-VER-011 (supporting case selection 001/010/011); Matrix source row retains owned residual and gate |
| GT M2.2 Coherence Under Pressure | AOS-12-REQ-029, AOS-12-REQ-030 → AOS-12-VER-019, AOS-12-VER-020 (supporting case selection 019/020); Matrix source row retains owned residual and gate |
| GT M2.3 Incommensurable Trade-off Capacity | AOS-12-REQ-010, AOS-12-REQ-011, AOS-12-REQ-028 → AOS-12-VER-007, AOS-12-VER-018 (supporting case selection 007/018); Matrix source row retains owned residual and gate |
| GT M2.4 Epistemic Brake Function | AOS-12-REQ-014, AOS-12-REQ-027 → AOS-12-VER-009, AOS-12-VER-017 (supporting case selection 009/017); Matrix source row retains owned residual and gate |
| GT M2.5 Directorial Independence | AOS-12-REQ-007, AOS-12-REQ-030, AOS-12-REQ-031 → AOS-12-VER-005, AOS-12-VER-020, AOS-12-VER-021 (supporting case selection 005/020/021); Matrix source row retains owned residual and gate |
| GT M2.6 Social Legitimacy | AOS-12-REQ-015, AOS-12-REQ-016, AOS-12-REQ-019, AOS-12-REQ-052, AOS-12-REQ-053 → AOS-12-VER-010, AOS-12-VER-012, AOS-12-VER-035 (supporting case selection 010/012/035); Matrix source row retains owned residual and gate |
| GT M2.7 No-Exit Obligation | AOS-12-REQ-017, AOS-12-REQ-018, AOS-12-REQ-030, AOS-12-REQ-032 → AOS-12-VER-011, AOS-12-VER-020, AOS-12-VER-022 (supporting case selection 011/020/022); Matrix source row retains owned residual and gate |
| GT M2.8 Radical Transparency | AOS-12-REQ-002, AOS-12-REQ-023, AOS-12-REQ-024, AOS-12-REQ-043, AOS-12-REQ-044 → AOS-12-VER-002, AOS-12-VER-015, AOS-12-VER-029 (supporting case selection 002/015/029); Matrix source row retains owned residual and gate |
| GT M2.9 Moral Drift Detection | AOS-12-REQ-014, AOS-12-REQ-031, AOS-12-REQ-051 → AOS-12-VER-009, AOS-12-VER-021, AOS-12-VER-034 (supporting case selection 009/021/034); Matrix source row retains owned residual and gate |
| GT M2.10 Purpose Stability | AOS-12-REQ-001, AOS-12-REQ-037, AOS-12-REQ-038, AOS-12-REQ-048, AOS-12-REQ-049 → AOS-12-VER-001, AOS-12-VER-025, AOS-12-VER-032 (supporting case selection 001/025/032); Matrix source row retains owned residual and gate |
| GT M2.11 Murmuration Capacity | AOS-12-REQ-015, AOS-12-REQ-016, AOS-12-REQ-030, AOS-12-REQ-051 → AOS-12-VER-010, AOS-12-VER-020, AOS-12-VER-034 (supporting case selection 010/020/034); Matrix source row retains owned residual and gate |
| GT M2.12 Constitutional Authority | AOS-12-REQ-005, AOS-12-REQ-006, AOS-12-REQ-037, AOS-12-REQ-038, AOS-12-REQ-048, AOS-12-REQ-049 → AOS-12-VER-004, AOS-12-VER-025, AOS-12-VER-032 (supporting case selection 004/025/032); Matrix source row retains owned residual and gate |
| GT M2.13 AI Constitutional Framework Governance | AOS-12-REQ-031, AOS-12-REQ-037, AOS-12-REQ-038, AOS-12-REQ-039, AOS-12-REQ-040 → AOS-12-VER-021, AOS-12-VER-025, AOS-12-VER-026, AOS-12-VER-027 (supporting case selection 021/025/026/027); Matrix source row retains owned residual and gate |
| GT M2.14 Purpose-Led Design | AOS-12-REQ-001, AOS-12-REQ-050 → AOS-12-VER-001, AOS-12-VER-033 (supporting case selection 001/033); Matrix source row retains owned residual and gate |
| GT M2.15 Telos / Function Distinction | AOS-12-REQ-028, AOS-12-REQ-051 → AOS-12-VER-018, AOS-12-VER-034 (supporting case selection 018/034); Matrix source row retains owned residual and gate |

Author consistency conclusion: functional roles and repair/private/workforce/external/research/control/failure boundaries agree with the current shared infrastructure. SENS-CR-01–05 closed as author document corrections; wire profiles, operating roles/capacity, domain/annex/legal sufficiency and observed evidence remain open per§17 and40. No independent/executed conformance or operating readiness claim. Earlier dated text/addenda describe history; this current control takes precedence.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**Historical status notice — sensing consistency closure — 9 October 2026:** Mark authorised the remaining consistency work. SENS-CR-01–05 are closed at the functional-document/author-review level: all40 logical CON views across10–14 and40 have exact central adoption, producer/consumer/shared-owner and REQ/VER links; all80 controlled FP/RP/GT sources have precise current contributions and owned residual/gate dispositions; current body/control statements are reconciled. Versions10v0.4/11v0.3/12v0.3/13v0.2/14v0.8/40v0.6; Architecture/Mapv0.42; Sharedv0.18/Corev0.6/ExchangeRegisterv0.17/SourceMatrixv0.18; reviewv0.4. DEC001–096 unchanged. Sensing269 proposed REQs/176 planned VERs;40 retains40/38. No new requirement/case/interface, source promotion or execution. Exact compatible wire schemas/profiles, organisation appointments/capacity, independent review, legal/institutional/practice evidence and scoped build/activation remain separate; independent project review remains deferred. Earlier dated notices/addenda are historical. Current controlling allocation is the9October manifest and source addendum below.

