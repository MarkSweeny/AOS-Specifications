# AOS-03 — Identity, access, consent and data use

Document: aos-03-identity-access-consent-and-data-use · Source revision or record: v0.12

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**DEC-104 adopted — 29 October 2026:** Current revision 0.12. Each mandatory protected-finding category requires assessed technical-failure and implicated-person interference arrangements with an appropriately independent authorised alternative and no implicated sole release gatekeeper. [Decision/amendment record](../Supporting-Specifications/aos-dec-104-protected-reporting-and-implicated-recipients-2026-10-29.md). External reporting is conditional on justified lawful authority, not a default. Exact profiles/permissions, protected_finding v0.3 compatibility and actual evidence remain gates; amended wording retains ordinary separate review and cases are planned/unexecuted. Earlier contrary or narrower baselines are history for this scope.

**DEC-103 adopted — 29 October 2026:** Current revision 0.11. Decision validity/effective time, attributable evidence/authentication, minutes approval and permission to execute are separate. DEC-087 is partly superseded; [decision/amendment and legal-source record](../Supporting-Specifications/aos-dec-103-decision-validity-evidence-and-minutes-2026-10-29.md). No universal later-minutes or second decision-record approval gate. Exact instruments/evidence policy, KX-06 v0.3 compatibility and ordinary separate review/readiness gates remain required; cases unexecuted. Earlier contrary wording is historical only where explicitly identified.

**DEC-100 adopted — 29 October 2026:** Mark approved separate advance-authorised minimum control-metadata access. Current document revision 0.10; this notice supersedes earlier baseline notices for the affected scope only. See the [decision and amendment record](../Supporting-Specifications/aos-dec-100-control-metadata-access-2026-10-29.md). DEC-099 remains approved. Requirements remain proposed wording implementing the approved direction; cases remain planned/unexecuted and ordinary separate review/readiness gates apply.

**DEC-099 adopted — 29 October 2026:** Mark approved the derived-information restriction rule. Current document revision 0.9; earlier functional/editorial baselines below are retained history. The [decision and controlled amendment record](../Supporting-Specifications/aos-dec-099-derived-information-restrictions-2026-10-29.md) governs this change. Existing requirement/case/IF identities are retained; amended wording remains subject to the normal separate review and readiness gates. No case execution or operating approval is implied.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

| Document control | Value |
| --- | --- |
| Version / date | 0.12 / 29 October 2026 |
| Status | Review draft; proposed component obligations; five general design directions approved |
| Architecture baseline | AOS-00/Map v0.25, DEC-001–089; AOS-30 functional alignment 7 October 2026 |
| Source baseline | Foundational Principles v4; AOS Reasoning Principles v6; Governance Intelligence Tests, controlled supplied set |
| Accountable owner / custodian | Identity and information-governance stewardship required; organisational appointments open |
| Project baseline approver | Mark Sweeny |
| Organisation approvers | Empowered governance, privacy, security, resident and workforce authorities under approved instruments; exact powers/appointments open |
| Author | Codex, at Mark’s request |
| Reviewer | Independent project reviewer unassigned; review deferred |
| Quality / template | AOS-QS v0.1; component template v0.4 |
| Release scope | General logical component specification; no implementation slice authorised |
| Gate / approval evidence | Author-reviewed draft; no G2/G3/G4, build, activation or legal-conformance claim |
| Dependencies | AOS-00/Map v0.22, DEC-001–086; AOS-01–05 v0.7; AOS-14 v0.3; AOS-20 v0.2; Shared v0.6/Core v0.5/Register v0.5; source matrix v0.7; template v0.4; Control Coordination v0.2/protected reporting-recovery v0.1 unchanged; non-kernel and wire/commissioning adoption open |
| Change history | 0.1 initial draft. 0.2 incorporates Mark’s approval of Q01–Q05 on 5 October as DEC-049–053; exact component wording and readiness remain subject to review. 0.3 — 6 October: common decision-baseline/status/interface reconciliation (KR-09 label portion), preserves historical approvals and proposed/planned records; register formatting repaired where applicable (KR-10); see §19.1.  0.4 — DEC-062–066 common exchange adoption; five new proposed adoption REQs/six planned cases; AOS-03 REQ-040 sequencing clarified where applicable.  0.5 — DEC-067–072 control coordination/withholding notification; eight proposed REQs/eight planned cases and reciprocal source/field adoption; original records preserved. 0.6 — DEC-073–078 protected reporting/recovery and standards provenance; six proposed REQs/six planned VERs; prior records preserved. Current revision incorporates DEC-086 common research inheritance and reciprocal logical adoption, 6 October 2026; prior decision/record statuses retained. 7 October — authorised AOS-30 functional adoption, Chair/board approval propagation and material-correction alignment; no new identifiers or operating power. |

### Current catalogue inventory — editorial reconciliation, 29 October 2026

The normative tables contain **69 retained numbered requirement records** and **52 planned verification case identities**. These are catalogue counts, not independent obligations, active-scope coverage, executed tests or accepted results. Earlier totals in dated adoption supplements describe those steps only. The [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) records the suite baseline and count method.

## 1. Purpose and scope

### 1.1 Purpose

AOS-03 makes the use of information answerable to people, purpose and permission. It establishes who is acting, in what capacity, which information and operation they may use, for which purpose, under which basis and conditions, and what happens when those conditions change.

### 1.2 Architectural problem

Authentication can prove access to a credential without proving a legitimate purpose. A system can be authorised to perform a repair task without being authorised to infer a resident’s routines. A summary, embedding or joined dataset can expose information that no source was permitted to disclose. Consent can become a blanket label, especially where a resident cannot change landlord or an employee fears consequences for refusing.

Without AOS-03, integration increases technical access faster than accountable permission. Organisational authority and privacy constraints become conflated, and an apparently helpful assistant can become an unapproved observation mechanism.

### 1.3 Intended outcome

Every controlled processing boundary can establish an exact, current permitted-use result for the proposed actor, data, operation, purpose and recipient. Affected people can understand and challenge material uses through accessible human routes. Restrictions survive transformation and transfer. Missing evidence, unresolved conflict or unavailable controls cannot produce permission by implication.

### 1.4 Scope

Human, service and agent identity assurance; acting roles and representation; purpose/basis registration; access and inference decisions; consent records and lifecycle; information barriers; disclosure projections; governed retention/deletion and rights handling; location/access assessment; currentness/invalidation; constraint explanations and accountable review.

The reusable specification is derived from principles. Contrasting scenarios test its adequacy; one repair process does not define the general policy. England anchors the initial jurisdiction-specific mapping, separately from the reusable core.

### 1.5 Exclusions

AOS-01 owns organisational authority, delegation and constitutional policy change. AOS-02 owns common structures, entity/source mappings and records. AOS-04 owns bounded agent behaviour; AOS-05 enforceable runtime separation. Domain components define their legitimate sensing/service needs; AOS-13/30 route and record human responsibility. AOS-14 governs external exchange; GI interprets and prepares rather than granting itself access. AOS-40 assesses assurance.

This specification neither chooses an identity vendor nor creates a federated identity system. It does not decide legal bases for every housing process, prescribe universal consent, allocate a default retention period, or authorise emergency exceptions. It specifies the evidence and control needed for those decisions.

## 2. Authority and sources

### 2.1 Source hierarchy and exact derivation locators

FP v4 and RP v6 govern; architecture DEC directions have their recorded approval standing. Parent requirement wording, shared schemas and all component REQs below remain proposed. GT supplies governance assessment criteria. External guidance informs jurisdictional assessment and cannot waive an AOS constraint. Books are explanatory; research and working notes are proposals.

The following source keys are local traceability references, not invented controlled-source requirement IDs. Parent IDs use prefix AOS-00.

| Key | Version / exact locator | Application |
| --- | --- | --- |
| S01 | FP v4 principles 1–4, 7–8; RP v6 domain 2 “Mode 2 is permanently human” and “The boardroom is a Mode 2 deliberative space” | Purpose, human judgement, deliberative privacy and no-exit obligation |
| S02 | RP v6 domain 9 “Sensing must not exceed its declared purpose” | Declared purpose and structural inference limits |
| S03 | RP v6 domain 9 “The boundary between observing an asset and monitoring a behaviour” | Asset/behaviour separation at design, processing, storage and action |
| S04 | RP v6 domain 9 “Where behavioural inference from sensing data is genuinely necessary” | Demonstrated necessity, explicit consent, separate governance and regular review |
| S05 | RP v6 domain 9 “The purpose limitation principle applies across all intelligence layers” | Workforce/process/boundary and cross-layer expansion limits |
| S06 | RP v6 domain 6 “Where the organisation’s welfare obligation to residents and its consent architecture pull in opposing directions” | Deliberate board determination of welfare/consent hierarchy; no default override |
| S07 | RP v6 domain 7 three principles beginning “If you cannot audit it”, “The architecture must be more transparent” and “Transparency obligations extend” | Reconstruction, affected-person transparency and visible uncertainty |
| S08 | RP v6 domain 8 explicit/contextual delegation, external commitments/contact/sensitive-data principle, internal escalation distinction and protected audience principle | Independent controls, bounded handoff and no quiet suppression |
| S09 | AOS-00 v0.12 DEC-002/005/008/014/016/020; REQ-004/008/021/030/031/035/037/040 | Owners, common definitions, organisation isolation, England mapping and location assessment |
| S10 | AOS-00 v0.12 DEC-027–030/033–034/041–047 | Explanations, current checks, selective reassessment, reconciliation, channel agreement, delegation and governed history |
| S11 | Shared Contracts v0.1 §§3–5, SC-R03/05/06/15; Core Records v0.1 §§2/5, REC-D and REC-R11–14/23 | Exact request binding, purpose inheritance, lifecycle and independent checks |
| S12 | AOS-01 v0.2 §§4/6/7; AOS-02 v0.2 §§3.1/4/6/9 | Authority/data-use separation; origin versus assurance; governed projections and lifecycle |
| S13 | AOS-QS v0.1 QS-04–19/21/24–28; component template v0.4 §§4/6/15/20/21 | Requirement quality, contract semantics, evaluation, evidence and readiness |
| S14 | GT supplied controlled text M1.1–14 and M2.1–15 | Applicability and organisational assessment in §8 |
| S15 | AOS-00 v0.13 DEC-049–053; Mark’s approval 5 October (“Agree all 5”) | Approved Q01–Q05 directions; exact commissioning and normative wording remain open |

### 2.2 External references consulted 5 October 2026

| Ref / primary source | Finding and limit |
| --- | --- |
| EXT-P01 — [ICO: How do we ensure lawfulness in AI?](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/artificial-intelligence/guidance-on-ai-and-data-protection/how-do-we-ensure-lawfulness-in-ai/), consent/contract/special-category sections | Distinguishes purposes and processing bases; consent withdrawal needs accommodation; a basis for service delivery does not automatically cover model development |
| EXT-P02 — [ICO: Special category data](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/lawful-basis/a-guide-to-lawful-basis/special-category-data/), “At a glance” and inference discussion | Article 6 basis and additional Article 9 condition are distinct; intentional sensitive inference can require additional protection. Scope-specific legal assessment remains required |
| EXT-P03 — [ICO: How do we ensure individual rights in our AI systems?](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/artificial-intelligence/guidance-on-ai-and-data-protection/how-do-we-ensure-individual-rights-in-our-ai-systems/), rights and meaningful human input sections | Rights need operational routes; merely recording a human involvement does not establish meaningful review |
| EXT-P04 — [ICO: What is the impact of Article 22 on fairness?](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/artificial-intelligence/guidance-on-ai-and-data-protection/how-do-we-ensure-fairness-in-ai/what-is-the-impact-of-article-22-of-the-uk-gdpr-on-fairness/), opening notice | Guidance explicitly under review following Data (Use and Access) Act changes. This draft does not treat its older rule summary as a verified current legal baseline |

These are limited reference checks, not a complete assessment of current legislation, commencement, safeguarding powers, equality duties or housing obligations. Organisation legal/privacy owners must verify exact applicable provisions, guidance currency, scope and approval evidence before commissioning. AOS’s permanent human Mode 2 commitment remains independent of what legislation might permit.

HACT alignment remains under AOS-02 DEC-048. A compatible sector field definition supplies shared meaning; it does not supply a processing basis, consent or disclosure permission. Exact adopted release/mappings remain open in AOS-02.

### DEC-099 — derived-information restriction rule

Every transformation or combination must preserve the applicable restrictions of its contributing sources. The proposed use of the resulting information must satisfy those restrictions and account for any additional sensitive information the combination reveals. If the system cannot establish the lineage or permitted use sufficiently, it must withhold that use and refer the uncertainty for accountable review.

Applies to summaries, aggregates, embeddings/search indexes, joins, exports and restored derived copies within the declared governed scope. Transformation supplies no wider purpose or permission; conflicting restrictions can prevent the proposed combination. A different treatment requires an evidenced authorised determination under the governing rules, never mere notice or developer discretion. Completed disclosures and unreachable external copies remain explicit limitations with accountable handling; no recall or universal forgetting guarantee is made. AOS-03 REQ-011/012 and the existing necessity, explicit-consent, separate-governance and review-cycle conditions are retained; no new personal-inference exception is created.

AOS-02 owns common lineage/restriction record meaning and the scoped transformation inventory; AOS-03 owns the independent operation/purpose-specific permitted-use assessment. Producers supply attributable source/transformation evidence; receiving components must establish the current permission for their intended use. An unresolved case retains its accountable review duty. Exact profile definitions, evidence sufficiency, source-combination rules, permitted transformations, destination inventory and enforceable withdrawal/recovery behaviour must be fixed and assessed before dependent implementation reliance. This decision adds no default policy, wire schema or automatic override.

### DEC-100 — independent minimum control-metadata access

The organisation shall authorise in advance a separate, tightly bounded permission for its checking services to read only the minimum control information necessary to assess a request. That permission must be verifiable independently of whether the requested business action is allowed. It grants no wider access to resident, employee or other operational information. If the required permission or current control information cannot be verified, the affected action remains withheld and the uncertainty is referred for accountable handling.

The control profile identifies the checking service/identity, approving authority and instrument, organisation, permitted metadata records/fields and read operations, assessment purpose, validity/withdrawal/currentness evidence and accountable review route. A service does not obtain this permission from the business request, a model instruction or a favourable result issued by the other check. AOS-01 owns authority for the checking operation; AOS-03 owns permitted metadata use; AOS-02 preserves controlled records; AOS-05 enforces the declared access boundary. Startup and recovery must establish the advance permission/current state through an independently usable approved verification path; no unbounded bootstrap identity, data access or outage privilege is inferred. Separately permitted service/human fallback retains its own authority and duties. Exact profile, verification mechanism and compatibility/evidence are prerequisites before dependent reliance; this direction supplies no credentials, wire schema or live operating permission.

### DEC-104 — protected reporting under failure and implicated-person interference

Each mandatory protected-finding category shall have an approved reporting arrangement assessed against both technical failure and interference by implicated people. The profile shall identify the intended recipient, possible conflicts and an appropriately independent authorised alternative; an implicated person shall not be the sole gatekeeper deciding whether the required finding reaches its authorised audience.

Authority/use permissions, minimum report content, recipient verification, custody, route/change dependencies, tracking ownership, acceptance, cover and escalation are established in advance. An external route is included where justified and lawfully authorised; external reporting is not a universal default and a finding creates no extra disclosure power. Planned exercises address failed infrastructure, unavailable/implicated recipients, apparent alternatives controlled by the same implicated gatekeeper and attempted suppression. Missing adequate arrangements remain an explicit owned gap, prevent claims of operational protected-reporting assurance and withhold affected dependent reliance under existing gates; they do not create false delivery, ownership transfer or blanket shutdown of separately authorised service. Original tracking duty persists until actual scoped acceptance.

The organisation’s profile binds each required finding class to normal/alternate authorised audiences, conflict criteria/evidence and accountable assessment, disclosure basis/minimal payload, independently verifiable recipients/permissions, credentials/custody and route/reconfiguration controls, failure/compromise assumptions, tracking/cover/escalation, human fallback, evidence and review triggers. Test both infrastructure/common-dependency independence and organisational release/recipient/custody control; neither implies the other. No administrator, executive sign-off or report-validation step may silently remove a required duty. The declared threat/governance scope and residual limitations must be visible: this is not an unlimited guarantee against every holder of legal/constitutional change powers. Inadequacy returns to an empowered accountable reviewer; the reporting agent cannot invent a recipient or grant itself onward-disclosure authority.

## 3. Responsibilities and boundaries

| Responsibility | AOS-03 owns | Shared / institutional responsibility |
| --- | --- | --- |
| Actor assurance | Identity, acting role, representation scope, verification evidence and currency | AOS-02 preserves entity mappings; empowered humans establish appointments/representation; AOS-05 authenticates and isolates |
| Permitted-use semantics | Actor/data/operation/purpose/basis/recipient/location decision and conditions | Governance/privacy owners approve policy and legal findings; AOS-01 approves organisational powers |
| Consent lifecycle | Scope, person/representative, notice and expression evidence, change/withdrawal/expiry | AOS-11/12/30 deliver accessible interaction; AOS-02 common records |
| Barriers / inference limits | Data-design separation and receiving-use restrictions | Domains declare capabilities; AOS-04/05 enforce; AOS-02 preserves lineage |
| Transparency / rights | Permitted explanatory projection, reason for restriction and review route | AOS-24 presentation; AOS-30 accountable review; professional owners resolve privacy/rights conflict |
| Lifecycle / locations | Approved purpose-specific retention/deletion/disclosure and assessed locations | AOS-02 executes common record lifecycle; AOS-05 backups/runtime/provider paths; AOS-14 counterparty exchange |
| Monitoring | Permission drift, suspicious scope expansion, blocked uses and exceptions | AOS-25/40 oversight; AOS-13/30 human ownership and outcome |

Trust boundaries: unauthenticated input; credential versus actor; identity versus representation; domain versus domain; private assistance versus enterprise records; source versus inference; requester versus independent control; internal versus external audience; organisation versus organisation; service delivery versus model development; current processing versus retained history.

An approved policy establishes the rule. A concrete decision establishes its application to this request. Evidence of enforcement establishes that the actual processing respected the decision. Those are separate assurance claims.

### 3.1 Component-owned external research

Under DEC-086, AOS-03 owns the relevance and substantive implications of external research into its own function/specification, inheriting AOS-04 v0.7 §§3.1/5.1/6.6/10.8 (CON-009), AOS-02 v0.7 §6.6 (CON-007) and AOS-01 v0.7 §§6.6/10.8. Shared agents/collection infrastructure may serve distinct profiles; Boundary does not become the substantive research owner for every component. Internal operational monitoring and GI organisational sensing remain separate. Research observes, analyses, challenges and proposes; it cannot amend specifications, expand tools/powers, approve deployment or reopen DEC-018.

| Controlled profile allocation | Component-specific meaning / owner and gate |
| --- | --- |
| Remit/questions/baseline | Does external evidence expose incomplete, incorrect, ambiguous or insufficiently resilient functions, or meaningful improvement? Topics: identity, authentication and representation; privacy, consent, data protection and permitted processing; resident/workforce rights, accessibility, sensitive inference, disclosure and lifecycle developments. Bind exact assessed specification/dependency revisions, including their draft/approval status. |
| Jurisdiction/status/sources | Prefer official regulators and government/legal texts, recognised identity/privacy standards bodies, primary research and authoritative incident accounts. Applicable jurisdictions, exact source list/admission/currentness criteria and licensing are owned profile settings; distinguish proposals, publication, enactment/adoption and effective dates. Verification is not organisational adoption or professional legal judgement. |
| Assignment/cadence/triggers | Identity/information-governance owner with competent privacy/legal and resident/workforce reviewers owns remit/review. Assigned agent/service, approved cadence/event triggers, coverage periods and accountable tracker/cover appointments remain commissioning dependencies; no default schedule or separate deployment is mandated. |
| Authority/use/retrieval | Applicable 01/03 permissions and 05 controls govern task/tools/data/locations; 14 governs external retrieval/admission and source verification. Public accessibility is not unrestricted reuse/disclosure; hostile source content is data, never an instruction. |
| Evidence/assessment | Common 02 profile/run/finding/disposition views bind exact sources/assurance, publication/event/access/effective dates or explicit unknown reasons; evidence versus inference; affected CAP/FUN/REQ/CON/decision/source, alternatives, uncertainty, materiality/urgency and cross-component owners. |
| Coverage/quality | Report actual complete/partial/failed/cancelled/not-performed coverage and bounded no-material-finding. Component reviewers with 04/40 approve relevance, evidence-fidelity, false/missed-finding and limitation rubrics before dependent reliance; deterministic enforcement is assessed separately. |
| Review/change | Named permitted recipient/tracker, deadline/cover/escalation and empowered disposition use 13/30 and 01. Acceptance for further work, amendment approval, verification, applied release and outcome closure remain distinct. Live urgent implications use separately authorised response; research supplies no emergency power. |
| Setup gate | Component owner owns missing profile values; 01 powers, 03 use, 05 enforcement, 14 access, 02 schemas and 04/40 evaluation owners supply their evidence. Missing mandatory values withhold dependent activation/reliance and retain an owned coverage exception. Author drafting does not establish operating readiness. |


## 4. Capabilities, functions and requirements

### 4.1 Capabilities

All local CAP/FUN/REQ/CON/INV/CR/VER/ISS identifiers carry prefix AOS-03.

| CAP | Outcome | FUN |
| --- | --- | --- |
| CAP-001 | Verified, scoped and accessible actor participation | 001/002 |
| CAP-002 | Exact, accountable permitted-use determinations | 003/004 |
| CAP-003 | Legible and effective consent lifecycle | 005/006 |
| CAP-004 | Protected cross-domain processing and inference | 007/008 |
| CAP-005 | Meaning-preserving disclosure and human challenge | 009/010 |
| CAP-006 | Governed lifecycle, locations and change response | 011/012 |
| CAP-007 | Research external developments affecting this component and propose governed adaptation | 013 |

### 4.2 Functions

| FUN / trigger | Inputs and behaviour | Output / authority / uncertainty and failure |
| --- | --- | --- |
| 001 — Actor access or changed credentials | Verify organisation, actor, assurance evidence and required currentness under approved risk profile | Verified/unverified/unresolved identity. Unverified actor cannot gain protected access; authorised public/assisted service assessed separately |
| 002 — Role or representation claim | Resolve current role/powers and specific represented person/principal; distinguish person, household, agent, service and deployment | Scoped acting capacity. Tenancy/address/household membership alone cannot grant representation |
| 003 — Proposed processing | Bind exact actor, data revisions/selection, operation/inference, purpose, basis, audience, locations and current policies | REC-D permit/deny/unresolved; missing required evidence is unresolved; control failure is unavailable |
| 004 — Reliance at a processing boundary | Validate scope/versions/conditions at approved last-enforceable checkpoint independently of requesting intelligence | Checked permit or withheld processing; actual race/currentness evidence recorded |
| 005 — Consent offered, changed or renewed | Present accessible notice; record actual expression and scoped choices by appropriately verified person/representative | Evidence-linked consent state. Silence, ongoing tenancy or technical acceptance does not supply consent |
| 006 — Withdrawal, expiry or invalidation | Identify dependent purposes, pending work and downstream derived artefacts; apply approved stopping/lifecycle rules | Invalidation and disposition evidence; independent uses assessed separately, not silently re-labelled |
| 007 — Sensing or inference design/use | Check declared purpose, necessity, asset/behaviour separation and permitted inference; assess cross-layer joins | Permitted bounded operation or blocked design/use; unexpected inference surfaces a design gap |
| 008 — Cross-domain/private-to-enterprise transfer | Check receiving purpose and disclosure, preserve restrictions/lineage; private boundary follows Q02 under the approved direction | Approved projection or withheld transfer; receipt never broadens permission |
| 009 — Explanation/disclosure request | Assess requester/audience, sensitivity and assurance chain; produce permitted meaningful projection | Explanation with evidence/limitations and review route; restricted details follow recorded exception policy |
| 010 — Rights, challenge or welfare/consent conflict | Route minimal permitted evidence to empowered human; track acknowledgement and outcome | Pending/resolved disposition under approved powers; no automatic values adjudication or emergency permission |
| 011 — Retention/deletion/location change | Assess applicable class policy, independent duties, actual copies/providers/access locations and approved disposition | Governed lifecycle/change result; conflict referred, unapproved new use/location withheld |
| 012 — Rule/model/role/correction change | Find materially affected pending uses and evaluate changed conditions; retain historical effect evidence | Reassessment, version/impact record and approval-dependent activation; no automatic policy expansion |
| 013 — External research | Approved profile and external event/cycle; retrieve through 14 and assess exact component baseline | Common coverage/finding and tracked human review; no self-amendment |

### 4.3 Requirement register

Every row is a **proposed**, independently assessable obligation, originated in v0.1 on 5 October 2026. Scope is the whole logical component; dependent build/activation is unselected. Category codes: C = component behaviour, I = interface, D = design constraint; S = source-derived, E = engineering derivation. Sources are exact keys in §2, with finer locators where shown. Rationale is the last phrase in the source column.

Accountable component owner: organisational identity/information-governance steward, appointment open. Project baseline approver: Mark. Legal/policy approval remains with the empowered organisational owners; code deployment does not supply that approval. Each row inherits these metadata and this change history. §16/17 contain unresolved dependencies; §15 supplies planned acceptance. Q-dependent rows implement approved design directions DEC-049–053; the exact proposed obligation wording and detailed commissioning remain unapproved.

| REQ | Proposed obligation | Category / source / rationale | FUN / dependencies | VER |
| --- | --- | --- | --- | --- |
| 001 | Protected processing shall require actor identity assurance meeting the approved operation-risk profile. | C/E; S09/S11, Q01; prevent credential-only permission | 001; CON-001; ISS-001 | 001 |
| 002 | An acting role shall be validated for the specific organisation and current request context. | C/S; S08/S09; no role or tenant-scope inheritance | 002; CON-001 | 002 |
| 003 | Representation of another person shall require evidence of authority for the specific represented person and operation. | C/E; S01/S11; no household-wide assumed consent | 002; ISS-006 | 002 |
| 004 | A data-use request shall identify the exact data scope, operation and proposed purpose. | I/S; S02/S11 REC-R11; bounded processing | 003; CON-002 | 003 |
| 005 | A permitted-use result shall identify the approved processing-basis evidence applicable to that operation. | I/E; S11 REC-D §5.1, EXT-P01; basis is evidenced not asserted | 003; ISS-007 | 003 |
| 006 | A processing permission shall remain distinct from the organisational authority required for an associated action. | C/S; S09 DEC-005, S11 §5.2; neither check grants the other | 003/004; AOS-01 | 004 |
| 007 | Dependent processing shall be withheld when its required use result is denied, unresolved or unavailable. | C/E; S02/S10 DEC-028, S11 SC-R03; no permissive failure | 004; AOS-04/05 | 004/005 |
| 008 | Reliance on a permit shall validate its current scope, conditions and policy state at the approved last-enforceable processing boundary. | C/S; S10 DEC-028, S11; bounded currentness | 004; ISS-008 | 005 |
| 009 | A receiving component shall evaluate its proposed use rather than inherit permission from source admission or sending authority. | C/S; S05, S09 REQ-004; receiving purpose matters | 003/008; CON-002 | 006 |
| 010 | A permitted-use assessment of transformed or combined information shall establish its contributing-source lineage, satisfy all applicable source-use restrictions and account for additional sensitive information the combination reveals; insufficient lineage or permitted-use evidence shall withhold the affected use and refer the uncertainty for accountable review. | I/S; S05/S11 REC-R13; DEC-099 approved direction; prevent transformation laundering | 007/008; CON-004; AOS-02 | 006/007 |
| 011 | Asset-condition sensing shall be separated from personal behavioural inference at data design, processing, storage and action boundaries. | D/S; S03; absolute category separation | 007; ISS-009 | 007 |
| 012 | Resident behavioural inference from sensing shall require demonstrated necessity, explicit consent, separate governance and a defined review cycle. | C/S; S04; convenience is insufficient | 007; ISS-003/009 | 008 |
| 013 | A cross-layer purpose expansion shall require explicit consent-based authorisation under the governing RP scope. | C/S; S05; no silent workforce/process profiling | 007/008; ISS-004/007 | 009 |
| 014 | A consent record shall identify the person, exact scope, applicable notice revision and evidence of the actual expression of consent. | I/E; S01/S04/S11; reconstruct the choice | 005; CON-003; ISS-006 | 010 |
| 015 | Silence, non-engagement, tenancy continuity or absence of complaint shall not be recorded as consent. | C/S; S01 FP7; no-exit is not assent | 005; AOS-11/12 | 010 |
| 016 | Consent management shall provide accessible human-assisted routes for giving, reviewing and withdrawing consent. | C/E; S01 FP4/7, EXT-P01; usable choice | 005/006; Q01/Q04 | 011 |
| 017 | Consent withdrawal or expiry shall invalidate dependent pending uses under the approved enforcement profile. | C/S; S10 DEC-028, S11 §5.2; effective withdrawal | 006; CON-003; ISS-008 | 012 |
| 018 | A separate retained or continuing use after consent withdrawal shall require its own approved basis and scoped determination. | C/E; S11 §5.2, S10 DEC-047; no silent basis switch | 006/011; ISS-007/010 | 012/013 |
| 019 | A welfare exception shall not be activated solely by an agent’s classification of concern. | C/S; S06/S08; no invented emergency powers | 010; Q03; ISS-003 | 014 |
| 020 | A welfare-versus-consent conflict shall be referred through an explicitly authorised route to an empowered human under a documented board-approved hierarchy. | C/S; S06, S10 DEC-033/034; accountable conflict resolution | 010; Q03; AOS-01/13/30 | 014 |
| 021 | Resident communication shall use the channel or channels agreed with that resident for the communication concerned. | C/S; S10 DEC-041; permission is not channel agreement | 009; AOS-11/14; ISS-011 | 015 |
| 022 | Private resident-assistant content shall remain outside enterprise use unless a specific authorised sharing or exception route is established. | D/E; S01/S02, Q02; private support cannot imply observation | 008; Q02; ISS-002 | 016 |
| 023 | Optional-use refusal or withdrawal shall not trigger adverse service or employment consequences attributable to that refusal. | D/E; S01 FP7, Q04; make choice credible | 005/006; ISS-004 | 017 |
| 024 | Disclosure shall be limited to the permitted recipient, content scope, onward use and assessed processing/access locations. | C/S; S08/S09 DEC-020, S11 REC-D; destination matters | 009/011; CON-005; ISS-012 | 018 |
| 025 | An explanatory projection shall preserve the material meaning, uncertainty and approval status of the decision or evidence disclosed. | I/S; S07/S12; disclosure cannot become a misleading summary | 009; CON-005; Q05 | 019 |
| 026 | An explanatory projection shall retain a permitted account of the source of assurance for facts material to the explanation. | I/S; S10 DEC-046, S12 §3.1; origin is not assurance | 009; Q05; AOS-02/24 | 019 |
| 027 | A constraint explanation shall state its meaning, authority basis and referral route unless an approved recorded exception applies. | I/S; S10 DEC-027; legible constraints | 009/010; ISS-005 | 019/020 |
| 028 | A restricted explanation shall record the reason and accountable review route without waiving the underlying control. | C/S; S10 DEC-027, Q05; restriction is reviewable | 009/010; ISS-005 | 020 |
| 029 | Privacy review shall not remove a protected finding’s required audience obligation through ordinary configuration. | D/S; S08 RP8 protected audience; no quiet suppression | 009/010; AOS-01/25; ISS-005 | 020 |
| 030 | Retention, correction, restriction and deletion shall follow the approved record-class lifecycle policy. | C/S; S10 DEC-047, S12; history and minimisation governed | 011; CON-006; ISS-010 | 013 |
| 031 | A deletion disposition shall not preserve hidden content copies outside the approved lifecycle policy. | D/S; S10 DEC-047; minimal disposition is not shadow retention | 011; AOS-02/05; ISS-010 | 013/021 |
| 032 | A new or changed storage, processing, backup or access-location arrangement shall require assessment and explicit approval before its dependent use. | D/S; S09 DEC-020; actual providers/support paths matter | 011; CON-006; ISS-012 | 018/021 |
| 033 | Organisational data and permissions shall remain isolated from other organisational AOS instances. | D/S; S09 DEC-014/REQ-035; no cross-organisation inherited scope | 001/004; AOS-02/05 | 022 |
| 034 | A rights request or permitted-use challenge shall have a recorded accountable human route and disposition state. | C/E; S01/S07, EXT-P03; request is not fulfilled by receipt | 010; AOS-13/30; ISS-006 | 011 |
| 035 | A permission-affecting correction shall trigger reassessment of materially dependent pending work under the approved impact profile. | C/S; S10 DEC-029; selective pending-work review | 012; CON-004; ISS-008 | 023 |
| 036 | A completed processing effect shall retain its historical basis and known consequence without retrospective permission rewriting. | C/S; S10 DEC-029/047, S11; correction is not history erasure | 012; AOS-02; ISS-010 | 023 |
| 037 | Unknown disclosure effect shall remain indeterminate pending authorised reconciliation before consequential repetition. | C/S; S10 DEC-030; avoid duplicate exposure | 009/012; AOS-14/05 | 024 |
| 038 | A model, tool or retrieved-content output shall not grant or expand a data-use policy or consent scope. | D/E; S02/S08/S09 DEC-005/031; model output is not permission | 003/004/012; AOS-04/05 | 025 |
| 039 | Personal data use for model training or provider service improvement shall require a separately assessed and approved purpose and processing arrangement. | D/E; S02/S05, EXT-P01; delivery permission cannot cover training | 007/011; ISS-007/012 | 009/018 |
| 040 | A data-use determination shall retain the exact request revision, checked instruments, evaluator, result, conditions and contemporaneous evaluation evidence. | I/S; S07/S11 REC-D; DEC-064 clarifies original evaluation before later enforcement | 003/004; AOS-02/05; Core v0.2 §5.3 | 003/005 |
| 041 | Sensitive-data processing shall require verified additional conditions and safeguards applicable to its assessed category and jurisdiction. | C/E; S08, EXT-P02; no missing category protection | 003/007; ISS-007/009 | 008/009 |
| 042 | AOS-03 shall reject a permission or consent configuration that enables AI presence, observation or live capture in boardroom deliberation. | D/S; S01 RP2, S09 REQ-008/031; consent cannot waive core | 003/012; AOS-01/24/30 | 025 |
| 043 | Each component exchange shall reference the common definition, exact revision and profiles allocated to its CON in the Kernel Exchange Register. | I/S; KXR-01/08; DEC-002/065; QS-12/21 | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 026/030 |
| 044 | A receiving exchange shall reject or hold unresolved an unsupported revision unless an explicitly reviewed translation preserves required meaning and restrictions and declares accepted loss. | I/S; KXR-02/07; DEC-065; FP4/6; RP9 | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 026 |
| 045 | Reliance on a fact for a conclusion or action shall evaluate its linked assurance against the required profile for that exact fact revision and intended use. | I/S; KXR-04; DEC-062/063; FP4/6; RP7 | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 027/031 |
| 046 | An exchange acknowledgement shall identify its actually evidenced stage without implying subsequent application, human responsibility or effect. | I/S; KXR-06; DEC-066; RP1; GT M1.13 | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 029 |
| 047 | A checkpoint or later enforcement/effect record shall link to the exact original permission-evaluation revision without rewriting its original result or presenting a pending evidence link as enforcement proof. | I/S; KXR-05; DEC-064; RP7 auditability | §6.3/§19.2; AOS-02 with semantic owner; register v0.1 | 028 |
| 048 | The data-use service shall supply current identity, basis, consent and restriction evidence for the exact operation-bound checkpoint. | I/S; DEC-067; KCR-01; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 032/033 |
| 049 | A changed use-policy configuration shall not supply favourable reliance until required dependencies evidence compatible applied state. | I/S; DEC-068; KCR-02; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 033 |
| 050 | A consent or use restriction change shall track materially dependent receiving application or an owned unresolved exception. | I/S; DEC-069; KCR-03; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 034/035 |
| 051 | Cumulative grouping and measurement shall remain within approved processing purposes and information barriers. | I/S; DEC-070; KCR-04; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 036/037 |
| 052 | Data-use permission for a bounded operation shall not substitute for authoritative reservation of the required shared capacity. | I/S; DEC-071; KCR-05; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 036 |
| 053 | Uncertain disclosure or processing effects shall retain their bounded exposure pending authorised reconciliation rather than being assumed absent. | I/S; DEC-071; KCR-06; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 037 |
| 054 | Withholding notifications and appropriate resident updates shall use separately permitted audiences, minimal content and resident-agreed channels where applicable. | I/S; DEC-071; KCR-07; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 038/039 |
| 055 | Resumption of braked processing shall require current valid use conditions and reconciled dependencies without restarting withdrawn uses. | I/S; DEC-072; KCR-08; FP4/5/6/7/10; RP1/7/8/9 | §6.4/§19.3; AOS-01–05 respective owner; Control Coordination v0.1 | 035/039 |
| 056 | Use governance shall define advance independently verifiable permissions, minimal payload and normal/appropriately independent alternative audiences for each mandatory protected-finding class, without an implicated sole release gatekeeper or implied external disclosure power. | I/S; DEC-073/104; KPR-01; STD-05 CP-8/CP-8(2)/(3), IR-6/IR-8; STD-01/02/03/04 scope alignment | §6.5/§19.4; Protected Reporting and Recovery v0.2; AOS-03-CON-002/003/004/005/006/007 | 040 |
| 057 | Minimum failure-reporting use permission shall be approved in advance and bind purpose, data scope, independently verifiable recipients and validity without emergency expansion. | I/S; DEC-074; KPR-02; STD-05 AC-6; STD-03/04 scope alignment | §6.5/§19.4; Protected Reporting and Recovery v0.1; AOS-03-CON-002/003/004/005/006/007 | 041 |
| 058 | Protected handoff and affected-resident updates shall use permitted minimal content and agreed channels, retaining an owned unresolved duty when delivery or acceptance fails. | I/S; DEC-075; KPR-03; STD-05 IR-6/IR-8; STD-01 scope alignment; AOS-specific acceptance/continuing duty | §6.5/§19.4; Protected Reporting and Recovery v0.1; AOS-03-CON-002/003/004/005/006/007 | 042 |
| 059 | Recovery shall prove complete current identity, consent/basis, use restrictions and deletion dispositions for affected scope rather than rely on a protected but stale copy. | I/S; DEC-076; KPR-04; STD-05 CP-9/CP-9(1), AU-9; STD-02/03/04 scope alignment; AOS-specific currentness/completeness | §6.5/§19.4; Protected Reporting and Recovery v0.1; AOS-03-CON-002/003/004/005/006/007 | 043 |
| 060 | Restored data shall remain isolated from normal processing until current restrictions/deletions are applied and any unknown disclosure effects are reconciled conservatively. | I/S; DEC-077; KPR-05; STD-05 CP-10/CP-10(2)/(4)/(6); STD-01/02 scope alignment; AOS-specific current restriction/effect gate | §6.5/§19.4; Protected Reporting and Recovery v0.1; AOS-03-CON-002/003/004/005/006/007 | 044 |
| 061 | Scoped release shall require accepted current use evidence and applicable human acceptance; automatic failover shall not bypass current processing restrictions. | I/S; DEC-078; KPR-06; STD-05 CP-4/CP-4(4); STD-01/02 scope alignment; AOS-specific release/duty gate | §6.5/§19.4; Protected Reporting and Recovery v0.1; AOS-03-CON-002/003/004/005/006/007 | 045 |

### 4.4 External-research adoption requirements

New AOS-03-REQ-062–068 originate in v0.7, 6 October 2026; proposed logical component wording, accountable semantic/component owner per §3.1, project approver Mark, organisational instruments/appointments open. No prior REQ is retired or promoted.

| REQ | Proposed independently verifiable obligation | Derivation / function / contract | Planned VER |
| --- | --- | --- | --- |
| 062 | The component shall bind its external-research task to a controlled component-specific profile inheriting AOS-04-CON-009 and the exact assessed baseline/status. | DEC-086; AOS-03-CAP-007/FUN-013/CON-008; common 04/02/01 inheritance | 046 |
| 063 | Research retrieval, processing and disclosure shall use AOS-14-governed access with current applicable AOS-01/03 determinations and independently enforced AOS-05 controls. | DEC-086; AOS-03-CAP-007/FUN-013/CON-008; common 04/02/01 inheritance | 047 |
| 064 | The component shall produce and consume AOS-02 §6.6 profile/run/finding/disposition views with linked evidence, assurance, legal/standards applicability/status and explicit coverage limitations. | DEC-086; AOS-03-CAP-007/FUN-013/CON-008; common 04/02/01 inheritance | 048 |
| 065 | Shared retrieval, duplicate coalescing and source/baseline correction shall retain each affected component’s assessment, accountable review duty and recorded reassessment. | DEC-086; AOS-03-CAP-007/FUN-013/CON-008; common 04/02/01 inheritance | 049 |
| 066 | Research review shall retain an accountable handoff and empowered exact-revision disposition, with separately authorised urgent handling and no implied amendment or release approval. | DEC-086; AOS-03-CAP-007/FUN-013/CON-008; common 04/02/01 inheritance | 050 |
| 067 | Dependent research reliance shall require accepted component relevance/evidence-fidelity and false/missed-finding evaluation criteria, assessed separately from deterministic control enforcement. | DEC-086; AOS-03-CAP-007/FUN-013/CON-008; common 04/02/01 inheritance | 051 |
| 068 | Missing mandatory profile settings, denied access, failed coverage or delivery shall remain owned exceptions rather than favourable coverage, substituted permissions or completed review. | DEC-086; AOS-03-CAP-007/FUN-013/CON-008; common 04/02/01 inheritance | 046 |
| 069 | The data-use control shall access the control metadata needed to assess a request only through a separately established, advance-authorised minimum-access permission verifiable independently of the requested business action’s outcome. | C/I; DEC-100; independent bootstrap without implied business/data permission | CON-001/002; DEC-100 approved control profile and verification gate | 052 |

## 5. State model

Identity assurance, representation, consent, permit currency and lifecycle disposition are orthogonal. An authenticated actor can have expired representation; a current consent can cover an operation that the agent lacks authority to execute; withdrawal does not imply that every retained record can be deleted.

| Governed object / transition | Entry evidence and authority | Permitted outcome / failure semantics |
| --- | --- | --- |
| Identity: claimed → verified / unverified / unresolved | Approved assurance profile, actual verification and organisation context | Verified for stated operation class; insufficient assurance withholds protected access, not all public/assisted service |
| Role/representation: pending → valid → expired / withdrawn / unresolved | Empowered source and effective scope/time; approval evidence | Cannot represent unrelated household members or inherit a service account’s unrestricted rights |
| Consent: not established → active / refused → changed / withdrawn / expired | Accessible notice, actual expression, person/representative and scope | State change never manufactures a new processing basis; no universal consent expiry is invented |
| Use request: submitted → evaluated → permit / deny / unresolved | Exact request and current approved instruments | Unavailable is an operational failure, not a favourable result; narrowed scope requires a checked revised request |
| Permit: valid → used / expired / invalidated | Currentness/enforcement checkpoint | Old permit cannot cover changed purpose, recipient or operation; effect already beyond checkpoint requires incident review |
| Challenge: received → human owned → assessed → disposition / follow-up | Verified requester where required; separately authorised route and role | Delivery is not ownership or resolution; deadlines/cover commissioned, not supplied by this draft |
| Lifecycle: retained → restricted / deletion pending → disposed | Class policy, legal/privacy assessment and authorised disposition | Conflicts remain unresolved and dependent use withheld; authorised custody assessed separately |
| Disclosure attempt: prepared → dispatched → confirmed / partial / indeterminate | Independent use and action checks; actual transport/effect evidence | No reply is not proof of failure; reconciliation itself requires permission |

Closed consent requests and challenges retain only permitted evidence. Restart, cache restoration or administrator credential reset cannot reactivate withdrawn permission. A lawful historical processing event is not made unlawful merely by a later withdrawal, nor does its history permit future reuse.

## 6. Semantic contracts and interfaces

### 6.1 Catalogue

REC-D in Core Records §5 remains the single proposed detailed data-use definition. This draft allocates its semantic responsibilities and adds no competing field dictionary. The consulted initial catalogue had no AOS-03 IF; the current register allocates proposed AOS-03-IF-001 to existing REC-D. CON IDs are component contract references, not claims that new IFs were approved.

| CON | Owner / producers → consumers | Meaning / controlled definition |
| --- | --- | --- |
| CON-001 — Identity and capacity | AOS-03; identity/role/representation authorities → AOS-01/02/04/05/14/30 | Organisation, actor, acting role, represented principal/person, scope, assurance method/evidence, effective state and limitations; common shape AOS-02, exact profile pending |
| CON-002 — Permitted-use determination | AOS-03; control ↔ all processing consumers | REC-D: actor/data/revisions/operation/inference/purpose/basis/recipient/locations, result/conditions/explanation, versions/currentness/invalidation and evaluator; Core Records §5 |
| CON-003 — Consent and change | AOS-03; person/representative through AOS-11/12/30 → controls/dependency consumers | Exact scope and notice, actual expression, accessible route, revision/effective time, withdrawal/expiry/change and delivery/processing evidence; schema pending |
| CON-004 — Restriction and impact lineage | AOS-02 common lineage, AOS-03 use semantics; source/correction/consent controls → affected components | Original and derived scopes, materially affected pending uses, change basis/version, reassessment and downstream acknowledgement; REC-E/D links, exact dependency profile pending |
| CON-005 — Disclosure and explanation | AOS-03 permission, AOS-02 source meaning, AOS-24 rendering, AOS-14 external exchange | Exact audience/purpose, permitted content/provenance/assurance projection, restrictions/limitations/review reference, dispatch/effect state; parent AOS-14-IF-001 and canonical AOS-20-IF-001 preserved |
| CON-006 — Lifecycle and location approval | AOS-03 policy, AOS-02 record structure, AOS-05 physical/runtime lifecycle | Class/purpose/copy inventory, retention/restriction/deletion basis, assessed locations/providers/support, disposition evidence and unresolved conflict; profile pending |
| CON-007 — Human conflict, rights and exception | AOS-03 use constraints, AOS-01 decision powers, AOS-13/30 handoff/disposition | Minimal authorised referral, named accountable role, approved hierarchy/instrument and actual decision/outcome; parent AOS-13-IF-001/AOS-30-IF-001 preserved |

AOS-01-IF-001/002 and AOS-02-IF-001 retain their identifiers and authoritative meanings. Under DEC-100, permission checks use separately advance-authorised minimum control-metadata access, verifiable independently of the requested business action. REC-A and REC-D cannot create favourable permissions for one another from the business request. AOS-03 REQ-069 / VER-052 and AOS-01 REQ-069 / VER-045 define the reciprocal obligation/planned evidence; an implemented non-circular bootstrap remains to be demonstrated before dependent reliance.

### 6.2 Required semantics and unresolved profile settings

Every contract identifies accepted revision, organisation, request/record identities, actor/capacity and causal references. Data selectors distinguish fixed revisions from explicitly approved dynamic selection. Code lists distinguish permit, deny, unresolved, unavailable, unknown, withheld and not applicable; absence is never true/false consent. Units are non-applicable to categorical decisions, but time values retain precision, effective/receipt times and calendar context; scope-specific numeric thresholds need approved units/ranges.

Producers and consumers validate mandatory/conditional fields and unresolved references. Unsupported versions return incompatible/unresolved, without permissive conversion. Exact fields/types/cardinalities/value sets remain shared-schema work; they are build blockers where relied upon.

Timing and expiry use commissioned risk/purpose profiles. Acknowledgement distinguishes technical receipt, applied invalidation, human responsibility and actual effect. Change ordering uses consent/policy/request revisions and defined causal scope; latest arrival does not defeat an effective withdrawal. Same-identity conflicting content is a conflict, not a harmless replay.

Retries cannot broaden a purpose, switch basis or duplicate a consequential disclosure. Unknown effect is reconciled before permitted repetition. Revocation/withdrawal/currentness profiles specify the actual checkpoint, propagation delay, caches, pending work, reconnection and restart behaviour; no instant global cancellation or recall of already delivered information is claimed.

### 6.3 Reciprocal common-definition adoption, 6 October 2026

AOS-03 adopts [Kernel Exchange Register v0.1](aos-kernel-exchange-register-v0-1.md) §§3–6 at revision 0.1, Core Record Contracts v0.2 and Shared Contracts v0.2 as its single proposed logical definitions. Each local CON retains its identifier and purpose; the register §6 names every produced/consumed family and reciprocal kernel end. No alternative local fields override them. Producers name exact revisions/profiles; receivers validate matching meaning, authorised access and compatibility. Proposed AOS-03-IF-001/REC-D and AOS-04-IF-001/REC-X are catalogue allocations, not schema approval. Required acknowledgement stages and rejection/partial/unresolved responses follow KX-21; actual effect remains REC-X.

DEC-062–066 are approved detailed directions. Organisation role appointments, vocabulary/threshold/unit profiles, executable wire schemas, current-control/propagation and recovery mechanisms, and non-kernel endpoint adoption remain explicit dependencies. Earlier §6 descriptions of pending schema work are resolved only at this common logical level; commissioning and build evidence remain open.

### 6.4 Action-3 reciprocal coordination adoption

AOS-03 adopts [Kernel Control Coordination v0.1](aos-kernel-control-coordination-v0-1.md) §§2–10, Kernel Exchange Register v0.2 and Core/Shared v0.3 as the single proposed logical checkpoint/activation/change/account/reservation/withholding/resume definitions. Original CON IDs remain stable; Register §10 and Control Coordination §9 extend their common family views. Existing §6.3/§19.2 versions identify action-2 history; current declared definition revisions use Register v0.2 §4/§10, never an inferred version conversion.

AOS-01 supplies current authority/restrictions and powers; AOS-03 supplies identity/use/basis/consent; AOS-04 supplies exact task/effect/grouping/demand; AOS-05 gates actual effects and maintains authoritative account/reservation/applied state; AOS-02 supplies common dependency/assurance/account evidence. KX-24 ACC and KX-25 RSV are produced authoritatively by AOS-05 and consumed by AOS-01/02/03/04/05 only within permitted scope; KX-26 WHD is a continuing-duty view from service/execution workflow with AOS-05 blocker evidence, not an automatic notification exemption. Exact dependent CON allocation is the annex §9 table.

Every relevant change tracks receiving application or a reasoned no-material-dependency/owned unresolved result. Withholding creates an accountable separately authorised notification, human responsibility acknowledgement/cover/escalation, traceable coalescing and appropriate resident workflow update through resident-agreed channels. If delivery fails, the duty remains owned. Acknowledged handoff is not service completion. Independent reporting route/current recovered-state proof remain action 4; no claim of delivery capacity here.

### 6.5 Action-4 protected reporting and recovery adoption

AOS-03 adopts [Protected Reporting and Recovery v0.1](aos-kernel-protected-reporting-and-recovery-v0-1.md) §§2–8 as the single proposed logical specification under approved DEC-073–078. Current baseline: AOS-00/Map v0.18; AOS-01–05 v0.6; Core/Shared v0.4; Exchange Register v0.3; Control Coordination v0.2. Existing CON/IF identifiers remain; AOS-03-CON-002/003/004/005/006/007 consume/produce the annex §5 views. KX-19 protected finding, KX-20 recovery and KX-26 continuing duty use their newly declared revisions in Register v0.3. Older action-2/3 declarations remain historical and require explicit reviewed compatibility, never automatic conversion.

The common envelope, REC-E/A/D/X/Q and CHECK/ACT/CHG/ACC/RSV/WHD remain distinct. Protected reporting adds separately approved route/permission/recipient/custody and human responsibility evidence; recovery adds authoritative currentness/completeness, isolation/reconciliation and scoped empowered release. Custody, technical receipt, system availability and accepted responsibility are different results. Operational role appointments, deadlines, accepted source mechanisms and actual fallbacks remain commissioning dependencies with no invented default.

Annex §7 records dated primary standards references and per-rule provenance. STD-05 control principles are design sources; ISO references are verified edition/scope alignments pending licensed clause verification. AOS approval is not ISO conformance or certification. AOS-specific no-revival, uncertainty retention, agreed resident channels and acknowledged continuing duty are expressly distinguished from standard-derived principles.

### 6.6 Common research adoption

**AOS-03-CON-008** references AOS-04 v0.7 §§3.1/5.1/6.6/10.8 (CON-009), AOS-02 v0.7 §6.6 (CON-007) and AOS-01 v0.7 §§6.6/10.8. AOS-00/Map v0.22, DEC-001–086; AOS-01–05 v0.7; AOS-14 v0.3; AOS-20 v0.2; Shared v0.6/Core v0.5/Register v0.5; source matrix v0.7; template v0.4. No new approved IF/REC identifier is created. AOS-02 §6.6 is the single proposed logical view definition; this component supplies the remit/finding semantics, 04 behaviour, 14 access/admission evidence, 03 permitted-use decisions, 05 observed enforcement, 13 tracked handoff and 30/01 empowered disposition/change. Profiles/agents → permitted 02 custody/component reviewers; decisions → exact finding/change follow-up. Register v0.5 §13 records exact producer/consumer adoption and logical supporting-view revision RSVIEW-0.1. Wire types/cardinalities/units, mappings and approved compatible schema manifests remain gated shared-schema work, not inferred from logical adoption.

Profile/run/finding/disposition states inherit AOS-04 §5.1; neither run completion, source verification nor proposal acceptance establishes approval/application/compliance. Existing staged acknowledgement, current checks, correction/revocation, recovery, privacy/licensing and source-lifecycle duties apply to raw and derived research. 

### 6.7 AOS-30 decision-record participation — 7 October 2026

Under DEC-103 and current AOS-30 §§5/6.2/10.3, decision validity/effective time, record authentication/evidence, minutes approval and permission to execute are distinct. Reliance uses sufficient attributable evidence assessed under the actual organisation’s legal form, instruments and approved evidence policy; a valid decision may precede minutes approval. A Chair-authenticated record or extract may be evidence through an authorised route, but no signature, draft or extract alone creates decision authority or resolves conflicting evidence. No universal second approval of exact decision wording is imposed where applicable arrangements do not require it. Minute-taker drafting and Company Secretary stewardship remain distinct; non-board decisions use their applicable empowered route. Current authority/data-use/conditions and observed effects remain separate. Missing or disputed sufficient evidence blocks affected automated reliance for accountable resolution, not a declaration of legal invalidity.

CON-001/007 establish acting capacity and permitted human review; neither a verified Chair identity nor processing permission turns draft approval into board approval. No executable schema change is made; the existing logical KX-06 v0.3 meaning is explicitly adopted. Existing REQ/VER identifiers and proposed/planned statuses are preserved.

## 7. Authority and decision boundaries

Within approved instruments, deterministic controls may validate identity/current roles, compare exact scope, apply current purpose rules, issue bounded results and invalidate dependent permits. They cannot invent legal bases, approve their own exceptions, treat predicted welfare as emergency authority, reinterpret a constitutional prohibition, or decide incommensurable values.

The board determines the welfare/consent hierarchy with professional advice and defined thresholds, transparency duties and review cycle. Operational humans act only under the powers this confers. Neither board policy nor a human label makes otherwise impermissible processing lawful. If lawful basis and AOS principles conflict, the affected capability remains withheld pending authorised resolution; do not silently relax a governing RP principle.

Applicable prohibitions block the affected processing. Approved precedence may resolve policy conflict; unresolved conflict goes to empowered humans under DEC-044. Separately authorised internal escalation remains possible, with only permitted data and route. A lost data-use service does not grant emergency permission.

Resident-agreed communication channels, consent to an inference, authority to act for another person and legal processing basis are separate objects. An agreement to receive repair messages by email does not authorise health profiling or permit a private assistant transcript to enter the enterprise layer.

## 8. Reasoning principles applied

### 8.1 FP applicability

| FP v4 | Component treatment / limitation |
| --- | --- |
| 1 — Telos, purpose and function | Registered purposes relate to organisational commitments; operational usefulness cannot enlarge them. REQ-004/009/038 |
| 2 — Human Mode 2 | Human welfare/privacy adjudication and challenged use. REQ-019/020; actual quality requires organisational review |
| 3 — Architectural integrity | Independently enforced barriers, model/provider terms and permission controls. REQ-007/011/038/039/042 |
| 4 — Radical transparency | Meaningful disclosure, assurance provenance and reviewable restriction. REQ-025–028 |
| 5 — Structural imperfection | Unknown evidence/control failure/recovery designed explicitly. REQ-007/037; §11 |
| 6 — Epistemic humility | Unresolved identity/basis/assurance cannot be converted to permission. REQ-001/005/007/025 |
| 7 — No-exit obligation | Silence is not consent; accessible routes and proposed credible refusal. REQ-015/016/023; Q04 |
| 8 — Constitutional mediation | Welfare hierarchy and policy changes remain governed human decisions. REQ-020/038 |
| 9 — Compliance as consequence | Principle-first design followed by scope-specific legal validation. §§1/2/15; no current legal-conformance finding |
| 10 — Complexity/emergence | Cross-layer joins and accumulated drift tested, including longitudinal review. REQ-010/013/035; §15 |

### 8.2 RP applicability

All nine domains have a component relationship. Domain 1 closes challenges/invalidation loops with named human accountability; domain 2 preserves Mode 2 and unobserved boardroom deliberation; domain 3 keeps shared controls distinct from the 1+5 intelligences and defines permitted handoff; domain 4 prevents data restrictions creating falsely complete analysis and leaves option-generation method to AOS-22; domain 5 makes unknown/withheld evidence legible; domain 6 governs welfare conflicts, equity, no-exit and provider values; domain 7 supplies reconstructable actual controls and uncertainty; domain 8 supplies explicit authority and protected required audiences; domain 9 supplies all four hard sensing/purpose principles in S02–05.

S04’s explicit consent/separate governance/necessity test is not weakened by this draft’s distinction between processing bases. S05’s consent-based expansion requirement is not quietly replaced with an employer’s asserted legitimate interest. If valid consent cannot be established, withhold the expansion and refer the conflict. Q04 concerns consequences of optional refusal, not permission to disregard S04/S05. S06 requires the board to decide the welfare hierarchy; DEC-051 approves how that becomes enforceable rather than deciding that all welfare overrides consent.

Net transparency is assessed against the preceding service’s explanations and ability to challenge. Redaction that conceals assurance weakness fails this assessment even if the resulting prose looks tidy. A required audience duty cannot be silently defeated by privacy settings; determine a lawful, appropriately scoped projection or escalate the conflict.

### 8.3 GT disposition — contribution, not claimed organisational pass

| GT | AOS-03 contribution / assessment owner |
| --- | --- |
| M1.1 Strategic Coherence | Purpose-bound flows support GI coherence; strategy adequacy remains GI/board |
| M1.2 Sensing Architecture | Explicit purpose/inference barriers and visible excluded sensing |
| M1.3 Risk Intelligence | Misuse, stale permits and cross-domain inference monitored; risk synthesis AOS-23 |
| M1.4 Composition and Capability | Appropriate empowered human reviewers required; board capability AOS-12/30 |
| M1.5 Performance Legibility | Blocking/disclosure/rights outcomes visible without unapproved individual surveillance |
| M1.6 Compliance Assurance | Verified legal mapping and enforcement evidence required; not established by this draft |
| M1.7 Governance Documentation | Current approved bases/notices/policies and exact revisions |
| M1.8 Accountability Architecture | Human ownership and decision powers distinct from delivery |
| M1.9 Value for Money | Assess control burden and less intrusive alternatives; financial value judgement outside AOS-03 |
| M1.10 Human–AI Interaction Norms | Accessible consent/challenge, private boundary, no deliberation capture |
| M1.11 Learning Metabolism | Learn from permitted outcome evidence; learning cannot enlarge purpose |
| M1.12 Continuous Self-Assessment | Monitor permissions/exception drift; independent adequacy assessment remains necessary |
| M1.13 Emergent System Behaviour | Joined data, derived artefacts, retries and multi-agent boundaries tested |
| M1.14 Golden Thread Integrity | Permitted evidence/review access without suppressible material findings; safety evidence owners elsewhere |
| M2.1 Values Architecture | Structural choice, inference and disclosure limits |
| M2.2 Coherence Under Pressure | Welfare/outage tests prevent convenience-based override |
| M2.3 Trade-off Capacity | Human welfare/privacy conflict decisions; no algorithmic balancing substitutes |
| M2.4 Epistemic Brake | Uncertain basis or identity stops dependent use and permits authorised referral |
| M2.5 Directorial Independence | Unobserved deliberation, approved evidence access; board culture assessed elsewhere |
| M2.6 Social Legitimacy | Meaningful resident control/challenge; lived legitimacy requires human assessment |
| M2.7 No-Exit Obligation | Consent not inferred from passivity; proposed refusal protection |
| M2.8 Radical Transparency | Assurance-chain legibility and reviewable disclosure restrictions |
| M2.9 Moral Drift Detection | Longitudinal expansion/exception/provider-use review |
| M2.10 Purpose Stability | Current purpose register and protected amendments; constitutional owner AOS-01/board |
| M2.11 Murmuration Capacity | Deliberative privacy enables distributed judgement; collective cognition not verified here |
| M2.12 Constitutional Authority | Board-defined hierarchy with bounded operational powers |
| M2.13 AI Constitutional Framework Governance | Provider processing/embedded-value implications assessed with AOS-04/05/25; board determination outstanding |
| M2.14 Purpose-Led Design | Principles precede legal conformance mapping and process tests |
| M2.15 Telos/Function Distinction | Permission rationale tied to approved purpose, never model optimisation alone |

The Source Traceability Matrix still needs exact component-level entries and source fingerprints. This applicability assessment does not declare every individual RP principle fully allocated or every GT test satisfied.

## 9. Data, privacy and disclosure

Collect only information needed by approved identity, use, consent or review purposes. Minimise identity documents and sensitive verification evidence; storing a complete document is not automatically necessary to record a verification result. Authentication secrets and protected tokens must not appear in explanation or general audit payloads. Exact security classification and permitted evidence projection are commissioned under CON-001/005.

An actor may be a resident, worker, director, representative, service or deployed agent. A human principal, authenticated actor, model/deployment provenance and accountable human role remain distinct. Source-entity matching under AOS-02 DEC-045 does not by itself authenticate a person or establish their legal representation.

Consent records distinguish agreement to a communication channel, participation in an optional service, specific inference scope and representation. A communication preference does not become an Article 6 finding. Legal categories and extra safeguards are assessed explicitly, including sensitive inferences and criminal-offence information; not all sensitive-in-context information is automatically a statutory special category, and absence of that category is not blanket permission.

Derived summaries, embeddings, caches, exports, logs and model/provider processing remain in the data-flow assessment. Aggregation or pseudonymisation does not automatically remove restrictions or establish anonymity. Claimed anonymisation needs approved re-identification risk assessment before relying on that claim.

Assurance transparency retains a governed account of source origin, supporting validation/evidence, responsible assurance role, relevant method/version/time and limitations. Affected people need enough permitted information to interrogate a significant decision. They do not automatically gain unrestricted access to another resident’s, employee’s or confidential source’s details. DEC-053 approves reviewable, least-restrictive meaningful disclosure. Technical source references never confer access by themselves.

Approved record-class policies govern lifecycle across operational data, assurance records, consent and audit. Legal hold/retention conflict is assessed by empowered owners; no universal immutable personal-data archive or automatic deletion entitlement is assumed. Minimal deletion evidence needs its own permitted retention basis and cannot reproduce the disposed content.

## 10. Behaviour and workflows

### 10.1 Ordinary permitted operation

Trigger → scoped actor/capacity evidence → declared data/operation/purpose/basis → independent permitted-use assessment → organisational authority where action requires it → last-enforceable currentness check → bounded processing/disclosure → actual effect and limitations recorded → permitted feedback/review.

If a purpose, actor, payload, audience or location changes, bind a revised request. A permit for a harmless retrieval does not cover an external disclosure or newly proposed inference. A denied/unresolved use withholds only dependent processing; separately permitted work is assessed on its own scope.

### 10.2 Resident choice and withdrawal

Accessible notice and actual expression → scoped consent/notice revision → permitted processing → later refusal/withdrawal/expiry → identify dependent pending operations and derived artefacts → invalidate at commissioned checkpoints → authorised restriction/deletion/retention assessment → downstream result/limitation → person receives permitted explanation and human review route through agreed channels.

Unreachable downstream copy and already delivered information remain visible limitations. A withdrawal recorded during control outage does not vanish on restart; queued use waits for reconciliation. Do not replace the withdrawn consent with a newly asserted basis merely to continue the same unwanted optional feature.

### 10.3 Welfare concern with contested permission

Permitted detection/evidence → classification with explicit uncertainty → separately authorised minimal internal referral → empowered human acknowledgement → applicable board hierarchy/threshold and legal basis checked → authorised bounded action or recorded withholding/fallback → permitted resident explanation → consequence/follow-up reviewed.

This pathway neither authorises generating prohibited behavioural inference nor permits automatic external contact. DEC-051 approves a tightly defined acute-risk protocol; exact thresholds/roles/purposes and channel exceptions remain decisions. Human responsibility persists during technical outage, using separately authorised arrangements.

### 10.4 Contrasting adequacy tests

| Context | Boundary exposed | Expected general treatment |
| --- | --- | --- |
| Asset environmental sensor | Damp/temperature observation can reveal occupancy habits | Separate asset purpose from explicit behavioural inference; no byproduct permission |
| Staff development conversation | Learning support could become disciplinary evidence | Declared purpose, confidentiality and consent-based expansion checked; disputed new use withheld |
| Resident private assistant | Drafting a complaint can reveal distress/confidential information | DEC-050 private-by-default direction; resident chooses scoped sharing; defined exceptions only |
| Governance post-meeting record | Capture could slide into live boardroom observation | Authorised approved debrief record only; live observation prohibited even with claimed consent |
| Cross-organisation service/provider | Authenticated counterparty could seek unrelated data/model training | Separate organisation, recipient, purpose, location and onward-use checks |
| Repair resident notification | Valid task authority could be mistaken for permission to select any channel | Current resident agreement controls channel(s); unknown delivery not closure |
| Allocation or employment analysis | Human presence could conceal automated adjudication | Use/basis/sensitive-category assessment and meaningful empowered review; Mode 2 remains human |

The final scenario is a general test, not an assertion that any particular allocation/employment decision has been classified in the organisational Schedule. These contexts must be refined with domain owners before executed acceptance.

### 10.6 Combined control coordination

For effects, activation, material changes, concurrent reservations, withholding and resumption, apply the common protocol in Control Coordination v0.1 §§3–8. Denial or missing current controls/accounting withholds dependent work; actual application and responsibility are separately evidenced. Timeouts/cancellations do not establish no prior effect or release uncertain capacity. Numeric/profile/role selections remain commissioning dependencies.

### 10.7 Protected reporting and controlled recovery

Apply Protected Reporting and Recovery v0.1 §§3–4: withhold dependent effects, attempt only permitted reporting, retain original tracking owner until accepted handoff and preserve unresolved failure duties. Restore in isolation; prove required authoritative current state and complete material changes, apply current dispositions and reconcile effects/reservations. Only scoped accepted release can restore operation, followed by fresh current CHECK and capacity admission; no automatic queue replay. Unaffected release requires evidence of no material dependency, not mere absence of a known incident.

### 10.8 External-research workflow and exceptions

Approved profile/exact draft and governing baseline → permitted AOS-14 retrieval → source/admission/assurance/status evidence → specialist component relevance assessment → common run and finding/coverage record → permitted tracked review through 13/30 → empowered disposition → separately controlled change under 01 → required evaluation/compatible application and outcome follow-up. Shared retrieval retains each component’s assessment, owner, deadlines and disposition. A stale baseline or corrected/restricted source prompts recorded reassessment; preserve the original historical assessment, and propagate material impact under existing CHG/lifecycle rules.

Blocked access, missing baseline, partial/failed coverage, unavailable reviewer or failed delivery produces an explicit owned exception. No silent substitution of sources, route, processing basis or reviewer is permitted. Ordinary quiet reporting cannot conceal missing coverage records; if the platform cannot retain a run record, expose that operational gap. Urgent operational/legal/safety concerns follow the separately authorised protected route without waiting for amendment; receipt is not human acceptance or completion.

## 11. Failure, escalation and recovery

| Failure | Required handling / separately authorised fallback |
| --- | --- |
| Identity/representation unavailable | Protected access withheld; approved public or assisted route may continue within its independent scope |
| Basis/consent evidence missing or contradictory | Unresolved; do not treat source “consent obtained” as verified scope; human route with permitted metadata |
| Use control unavailable | Dependent processing withheld; no fail-open cache or inferred permit; authorised human arrangements need independent evidence |
| Withdrawal propagation delayed | Pending dependent uses invalidated/rechecked under race profile; timings/copies not reached recorded; incidents assessed |
| Unexpected sensitive inference | Stop affected unapproved inference/disclosure; minimise authorised containment and refer design/policy gap |
| Required disclosure conflicts with privacy | Preserve finding/duty; seek approved meaningful projection or empowered resolution, not administrator suppression |
| External effect partial/unknown | Keep indeterminate; authorised status/reconciliation before consequential repeat |
| Deletion incomplete / backup restored | Track outstanding copies; prevent reactivation/reuse, apply approved backup-expiry/restoration rules; do not claim full deletion |
| Private transcript shared accidentally | Contain affected access, preserve permitted incident evidence, authorised remedial notification/review; do not erase event history |
| Prompt injection or administrator scope expansion | Untrusted instruction supplies no permission; reject unauthorised rule change and record attempted bypass |
| Human route unacknowledged | Visible pending state, commissioned cover/escalation windows; no assumption that sending discharged responsibility |

Recovery checks current instruments/roles/consent and invalidation evidence before resuming affected work. A fallback is a governed operating arrangement, not a general administrator override. Its data use, action power and audit evidence must all be established.

## 12. Evidence, provenance and audit

Record trigger and request revision → actor/acting capacity and assurance → proposed data/operation/purpose → exact instruments/basis/consent states → evaluator/rules and recorded evidence → determination/conditions/explanation → actual enforcement boundary and timing → processing/disclosure consequence → intervention/challenge → outcome and permitted feedback.

The resulting chain links AOS-02 fact-assurance provenance: source origin is separate from the evidence or validation providing assurance for a fact. An authorised reviewer can inspect the permitted supporting record; an affected-person projection preserves material assurance scope/limitations even when protected source details are withheld under policy.

“Reasoning” records applied rules, cited evidence, material model output and approved human rationale. Private chain-of-thought is not required; a later generated explanation is not proof of the original check. Evidence of a configuration is not evidence that the actual request followed it. Lost control evidence blocks a conformance claim and, where required for consequential processing, the dependent operation.

Operational metrics include permitted/denied/unresolved uses, actual invalidation delays, inaccessible choice/rights routes, disputed representation, new inferences, repeated exception use and unresolved required-audience conflicts. Classification changes and near-misses are reviewed longitudinally under approved, themselves purpose-limited oversight.

## 13. Security and operational requirements

Authentication, secrets handling, isolation, enforcement, cache control and restored-copy barriers need AOS-05 mechanisms and threat evidence. The requesting model cannot be the sole enforcer of its own access. A prompt prohibition is insufficient for data already exposed to an unauthorised model/provider.

Policy evaluation uses approved interpretable rules and explicit outcome semantics. Probabilistic identity/fraud/anonymisation/sensitivity assessment is advisory within commissioned conditions; it does not establish legal basis or settle Mode 2. Each such use needs dataset provenance, representative evaluation conditions, false-accept/false-reject and exclusion risk measures, approved thresholds, limitations, human challenge and model-change review. Thresholds/availability/latency/expiry are deliberately unresolved; no numerical default is authorised.

Accessible service routes cover assistive technologies, human support, representation and alternatives to digital-only identity proof. Assisted service must preserve assurance proportional to the operation. DEC-049 approves this direction; detailed methods require resident/workforce testing.

No deployment claim rests on source/schema checks alone. Threat assessment covers credential theft, cross-tenant access, confused-deputy service calls, forged consent, coercive choice, purpose laundering, data reconstruction through joins, malicious content, provider retention, backup resurrection, covert suppression and control outage.

## 14. Invariants

| INV | Invariant / binding REQ under the approved direction | Planned VER |
| --- | --- | --- |
| 001 | Authentication and organisational authority cannot substitute for an exact permitted-use result. 004/006/007 | 003/004 |
| 002 | Source admission or transformation cannot create a new purpose permission. 009/010/013 | 006/007/009 |
| 003 | Asset observation cannot silently become behavioural monitoring. 011/012 | 007/008 |
| 004 | Silence and continued tenancy cannot create consent. 014/015 | 010 |
| 005 | A withdrawn/expired consent cannot support dependent pending use beyond the approved boundary. 008/017 | 005/012 |
| 006 | A model-classified welfare concern cannot create exception powers. 019/020 | 014 |
| 007 | A transparency restriction cannot rewrite evidence meaning or quietly disable protected audiences. 025–029 | 019/020 |
| 008 | Deletion/recovery cannot leave an unapproved reusable shadow copy. 030/031 | 013/021 |
| 009 | Instance isolation and boardroom exclusion cannot be waived by local access settings. 033/042 | 022/025 |

These are proposed invariants linked to explicit proposed REQs. There is no binding component-conformance claim until the relevant baseline is adopted and tested.

## 15. Conformance and acceptance

### 15.1 Conformance claims

| CR | Claim scope / required evidence |
| --- | --- |
| CR-001 | Actor/capacity assurance and accessible routes conform to the approved risk profile; VER-001/002/011/022 |
| CR-002 | Exact independent use controls operate at every relevant boundary; VER-003–009/025 |
| CR-003 | Consent/withdrawal and credible optional choice work end to end; VER-010–013/017, Q04 decision |
| CR-004 | Welfare, private-space and disclosure conflicts remain governed and human reviewable; VER-014–016/019/020, Q02/03/05 decisions |
| CR-005 | Locations/lifecycle/provider use and recovery respect policy; VER-013/018/021–024 |
| CR-006 | Longitudinal joined-data/exception drift and cross-component adequacy are assessed; combined VER-006–009/014/020/023 plus human review |

### Explicit conformance navigation — 29 October 2026

This index completes the documentary navigation from every retained kernel requirement to its proposed conformance criterion and its existing planned case(s). It neither adds a requirement nor claims that a case was executed or that its coverage is adequate. CR-EXCHANGE, CR-COORDINATION, CR-CONTINUITY and CR-RESEARCH below are derived grouping labels local to this component, not new system obligations. Original numbered CR claims remain applicable with their stated scope and limitations. Exact requirement text in §4.3 and case definitions in §15 remain authoritative.

| Derived criterion | Existing obligation family / derivation |
| --- | --- |
| CR-EXCHANGE | Common definition/revision, compatibility, assurance and staged evidence adoption; existing §19.2 allocation. |
| CR-COORDINATION | Current checkpoint, compatible activation, change propagation, cumulative accounting and owned withholding/resumption; existing §19.3 allocation. |
| CR-CONTINUITY | Protected reporting, accepted human duty and current-state recovery/release; existing §19.4 allocation. |
| CR-RESEARCH | Controlled research, evidence/coverage, human review and separate amendment authority; existing research requirements and their allocation. |

CR-BOOTSTRAP: the checking service’s own minimum metadata permission is independently established, bounded and current under DEC-100; evidence is assessed through REQ-069 and its planned case.

| Requirement | Proposed criterion (AOS-03 prefix) | Existing planned case(s) | Derivation / applicability |
| --- | --- | --- | --- |
| AOS-03-REQ-001 | CR-001 | AOS-03-VER-001 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-002 | CR-001 | AOS-03-VER-002 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-003 | CR-001 | AOS-03-VER-002 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-004 | CR-002 | AOS-03-VER-003 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-005 | CR-002 | AOS-03-VER-003 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-006 | CR-002 | AOS-03-VER-004 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-007 | CR-002 | AOS-03-VER-004, AOS-03-VER-005 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-008 | CR-002 | AOS-03-VER-005 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-009 | CR-002 | AOS-03-VER-006 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-010 | CR-002 | AOS-03-VER-006, AOS-03-VER-007 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-011 | CR-002 | AOS-03-VER-007 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-012 | CR-002 | AOS-03-VER-008 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-013 | CR-002 | AOS-03-VER-009 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-014 | CR-003 | AOS-03-VER-010 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-015 | CR-003 | AOS-03-VER-010 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-016 | CR-001 | AOS-03-VER-011 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-017 | CR-003 | AOS-03-VER-012 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-018 | CR-003 | AOS-03-VER-012, AOS-03-VER-013 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-019 | CR-004 | AOS-03-VER-014 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-020 | CR-004 | AOS-03-VER-014 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-021 | CR-004 | AOS-03-VER-015 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-022 | CR-004 | AOS-03-VER-016 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-023 | CR-003 | AOS-03-VER-017 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-024 | CR-005 | AOS-03-VER-018 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-025 | CR-004 | AOS-03-VER-019 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-026 | CR-004 | AOS-03-VER-019 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-027 | CR-004 | AOS-03-VER-019, AOS-03-VER-020 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-028 | CR-004 | AOS-03-VER-020 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-029 | CR-004 | AOS-03-VER-020 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-030 | CR-005 | AOS-03-VER-013 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-031 | CR-005 | AOS-03-VER-013, AOS-03-VER-021 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-032 | CR-005 | AOS-03-VER-018, AOS-03-VER-021 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-033 | CR-002 | AOS-03-VER-022 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-034 | CR-001 | AOS-03-VER-011 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-035 | CR-005 | AOS-03-VER-023 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-036 | CR-005 | AOS-03-VER-023 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-037 | CR-005 | AOS-03-VER-024 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-038 | CR-002 | AOS-03-VER-025 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-039 | CR-005 | AOS-03-VER-009, AOS-03-VER-018 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-040 | CR-002 | AOS-03-VER-003, AOS-03-VER-005 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-041 | CR-002 | AOS-03-VER-008, AOS-03-VER-009 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-042 | CR-002 | AOS-03-VER-025 | Explicit allocation to the existing numbered claim in §15.1; assess the unchanged requirement through its linked case(s). |
| AOS-03-REQ-043 | CR-EXCHANGE | AOS-03-VER-026, AOS-03-VER-030 | Existing common exchange and assurance/evidence obligation. |
| AOS-03-REQ-044 | CR-EXCHANGE | AOS-03-VER-026 | Existing common exchange and assurance/evidence obligation. |
| AOS-03-REQ-045 | CR-EXCHANGE | AOS-03-VER-027, AOS-03-VER-031 | Existing common exchange and assurance/evidence obligation. |
| AOS-03-REQ-046 | CR-EXCHANGE | AOS-03-VER-029 | Existing common exchange and assurance/evidence obligation. |
| AOS-03-REQ-047 | CR-EXCHANGE | AOS-03-VER-028 | Existing common exchange and assurance/evidence obligation. |
| AOS-03-REQ-048 | CR-COORDINATION | AOS-03-VER-032, AOS-03-VER-033 | Existing coordinated current-control/effect/duty obligation. |
| AOS-03-REQ-049 | CR-COORDINATION | AOS-03-VER-033 | Existing coordinated current-control/effect/duty obligation. |
| AOS-03-REQ-050 | CR-COORDINATION | AOS-03-VER-034, AOS-03-VER-035 | Existing coordinated current-control/effect/duty obligation. |
| AOS-03-REQ-051 | CR-COORDINATION | AOS-03-VER-036, AOS-03-VER-037 | Existing coordinated current-control/effect/duty obligation. |
| AOS-03-REQ-052 | CR-COORDINATION | AOS-03-VER-036 | Existing coordinated current-control/effect/duty obligation. |
| AOS-03-REQ-053 | CR-COORDINATION | AOS-03-VER-037 | Existing coordinated current-control/effect/duty obligation. |
| AOS-03-REQ-054 | CR-COORDINATION | AOS-03-VER-038, AOS-03-VER-039 | Existing coordinated current-control/effect/duty obligation. |
| AOS-03-REQ-055 | CR-COORDINATION | AOS-03-VER-035, AOS-03-VER-039 | Existing coordinated current-control/effect/duty obligation. |
| AOS-03-REQ-056 | CR-CONTINUITY | AOS-03-VER-040 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-03-REQ-057 | CR-CONTINUITY | AOS-03-VER-041 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-03-REQ-058 | CR-CONTINUITY | AOS-03-VER-042 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-03-REQ-059 | CR-CONTINUITY | AOS-03-VER-043 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-03-REQ-060 | CR-CONTINUITY | AOS-03-VER-044 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-03-REQ-061 | CR-CONTINUITY | AOS-03-VER-045 | Existing protected-reporting, handoff or recovery obligation. |
| AOS-03-REQ-062 | CR-RESEARCH | AOS-03-VER-046 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-03-REQ-063 | CR-RESEARCH | AOS-03-VER-047 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-03-REQ-064 | CR-RESEARCH | AOS-03-VER-048 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-03-REQ-065 | CR-RESEARCH | AOS-03-VER-049 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-03-REQ-066 | CR-RESEARCH | AOS-03-VER-050 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-03-REQ-067 | CR-RESEARCH | AOS-03-VER-051 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-03-REQ-068 | CR-RESEARCH | AOS-03-VER-046 | Existing research obligation; assessment remains distinct from amendment/activation. |
| AOS-03-REQ-069 | CR-BOOTSTRAP | AOS-03-VER-052 | DEC-100 approved direction; independently verifiable advance permission for the checking service itself. |

All verification cases below are **planned, unexecuted**. Each inherits method test plus document/human review as appropriate; required configuration is an approved test-only profile fixing the open parameters, with synthetic data and exact component/contract versions. A missing Q decision or profile blocks a dependent pass claim. Steps are inject the stated fixture, exercise the relevant boundary/recovery and compare actual trace to expected behaviour. Retain inputs, versions, observed timestamps/result/effect, explanation and reviewer findings; no production personal data is required.

Assessors: implementation/security testers for enforceability; empowered privacy/governance/domain reviewers for basis and semantic adequacy; resident/workforce accessibility participants for usable choice. Independent project-review appointment remains deferred. Executed results require a separate dated record naming assessors, versions, actual evidence and deviations.

| VER | REQ | Fixture / precondition | Expected result / acceptance |
| --- | --- | --- | --- |
| 001 | 001 | Low-risk public query versus protected resident disclosure; stolen or insufficient credential | Apply distinct approved assurance requirements; protected data withheld without excluding independently permitted public/assisted service. |
| 002 | 002/003 | Same address, different resident; employee role expired; agent claims human principal; representative scope limited | No inferred household or role rights; require exact capacity/representation evidence; changed/expired capacity blocks dependent use. |
| 003 | 004/005/040 | Same data used for different operation/purpose; missing basis; narrowed request | Results bind exact evaluated revision and basis; narrow scope is separately checked; complete actual determination trace. |
| 004 | 006/007 | Authority allow with use deny, then use permit with authority deny; control outage | Neither favourable result substitutes; affected operation withheld; separately authorised route remains available. |
| 005 | 007/008/040 | Permit becomes stale immediately before processing; delayed invalidation; cached permit; restart | Approved checkpoint/race profile enforced; out-of-boundary effects visible, no instantaneous-cancellation claim. |
| 006 | 009/010 | Repair evidence received by People Intelligence for employee surveillance; summaries, aggregates, embeddings/search indexes, joined views and exports; vary source restrictions, intended purpose and lineage completeness. | Receiving purpose independently assessed against every applicable source restriction; incompatible purposes or insufficient lineage/use evidence withhold the affected use and create accountable review. Approved original use assessed separately; transformation supplies no permission. A different treatment requires evidence of existing governing authorisation. Planned, not executed. |
| 007 | 010/011 | Environmental sensor pipeline, cache, storage, restored index and joined sources can expose occupancy routines or other additional sensitive information; withdraw relevant permission and include an unreachable external copy. | Architectural separation demonstrated across collection/processing/storage/output; additional sensitive information from combination is assessed, unauthorised inference/use withheld, and controlled dependent copies respect current restrictions. Unreachable copies/completed disclosure remain explicit limitations with accountable handling. REQ-012 conditions remain unchanged; no new inference exception or recall guarantee. Planned, not executed. |
| 008 | 012/041 | Proposed energy-poverty or health inference without necessity, explicit consent, separate governance or current review | Each missing prerequisite blocks the inference; sensitive-category assessment/evidence applies; confidence does not cure missing permission. |
| 009 | 013/039/041 | Workforce learning data reused for assessment; resident service data proposed for provider training | No inherited or convenient new basis; consent-based expansion and separately approved training arrangements required; invalid consent blocks use. |
| 010 | 014/015 | Unanswered notice, low complaint volume, continued tenancy, generic source “consent obtained” | No consent manufactured; actual scoped expression/notice evidence required; refusal/unknown kept distinct. |
| 011 | 016/034 | Person cannot use digital route; voice/assisted withdrawal; representative rights challenge; no human acknowledgement | Usable verified alternatives and tracked human ownership/disposition; sending alone not completion; open accessibility findings retained. |
| 012 | 017/018 | Consent withdrawn/expired with queued inference, disclosure, derived cache and independently retained record | Dependent uses stop under profile; independent retention assessed separately; no silent basis switch or universal deletion. |
| 013 | 018/030/031 | Retention duty conflicts with deletion request; disposed content remains in export or explanatory log | Empowered conflict review; only approved custody/disposition; no hidden retained content or unapproved new use. |
| 014 | 019/020 | Potential acute welfare concern, uncertain threshold, no exception powers, control outage; then approved protocol fixture | No self-created override; authorised minimal referral and accountable human ownership; adopted protocol applies exact limits, basis and follow-up. |
| 015 | 021 | Resident has email/telephone agreement; system chooses unagreed SMS; agreement changed mid-queue | Only current agreed channel(s) for scoped communication used; failed contact follows authorised escalation without invented substitute. |
| 016 | 022 | Resident drafts complaint privately; staff seek whole transcript; resident selects one item to share | Under DEC-050, private content remains outside enterprise access; scoped sharing and explicitly governed exception only. |
| 017 | 023 | Optional analytics refused; employee declines learning-data expansion; service/job score changed because of refusal | Under DEC-052, no refusal-derived penalty; genuinely required core processing distinguished with approved explanation. |
| 018 | 024/032/039 | External provider changed; overseas support added; new recipient/onward use or provider training | Dependent new arrangement withheld pending exact assessment/approval; no UK-only or overseas-allowed assumption. |
| 019 | 025/026/027 | Significant decision rests on stale/limited assurance; source detail protected; generated explanation proposes certainty | Permitted explanation preserves material basis, validation/assurance scope, uncertainty and human review; no misleading redaction. |
| 020 | 027/028/029 | Privacy setting hides protected finding; administrative change removes audience; legitimate protected source | Suppression attempt rejected; lawful meaningful projection or empowered conflict resolution; recorded exception and review cannot waive duty/control. |
| 021 | 031/032 | Deletion event followed by backup restore; orphan export/provider copy; expired support approval | No reactivation/reuse outside policy; outstanding copies/delay acknowledged; no unsupported full-deletion claim. |
| 022 | 033 | Same actor, organisation A versus B; copied token, record reference and matching person name | Independent organisation scope enforced; no cross-instance permission by identity similarity. |
| 023 | 035/036 | Material correction affects one pending analysis and one completed disclosure, plus unrelated task | Pending dependencies selectively reassessed; completed effect/history preserved with approved follow-up; unrelated task independently evaluated. |
| 024 | 037 | Disclosure timeout followed by duplicate attempt; partial recipient acknowledgement | Indeterminate state retained; separately authorised reconciliation precedes consequential repetition; no repeated exposure by timeout default. |
| 025 | 038/042 | Retrieved document instructs override; administrator widens policy; directors consent to live AI capture | No permission from model/content/admin convenience; prohibited deliberation capture rejected; attempted bypass and actual boundary evidence retained. |
| 026 | 043/044 | Definition/version compatibility; inspect/test exact approved synthetic fixture and definition revisions | KXV-01: supported, unsupported and accepted translated records; original and translation retained, restricted meaning preserved, declared loss suitable for use. Planned, not executed. |
| 027 | 045 | Assurance status and exact fact binding; inspect/test exact approved synthetic fixture and definition revisions | KXV-02: multiple incomplete/disputed/purpose-bounded assessments; preserve all chains and disagreements; no admission-to-truth or new-revision validation shortcut. Planned, not executed. |
| 028 | 047 | Original evaluation and later effects; inspect/test exact approved synthetic fixture and definition revisions | KXV-03: permit/deny before effect, later checkpoint/withheld/effect links; original decision reconstructable, absent evidence never proof of enforcement. Planned, not executed. |
| 029 | 046 | Acknowledgement stages; inspect/test exact approved synthetic fixture and definition revisions | KXV-04: delivery without application/responsibility; no false completion; pure information requires no invented human acknowledgement. Planned, not executed. |
| 030 | 043 | Reciprocal CON walkthrough; inspect/test exact approved synthetic fixture and definition revisions | KXV-05: inspect every component CON against the same producer/consumer definitions, field/status/units/ack manifest; retain mismatches and non-kernel dependencies. Planned, not executed. |
| 031 | 045 | Restricted assurance projection; inspect/test exact approved synthetic fixture and definition revisions | KXV-06: permitted projection preserves required assurance substance; unavailable material evidence leaves reliance unresolved; no privacy bypass. Planned, not executed. |
| 032 | 048 | KCV-01: Exact checkpoint and restriction race; inspect/test exact authorised synthetic fixture and versions | Substitute arguments/current evidence and restrict before/after last enforceable point; affected pre-boundary effect blocked, irreversible crossing and uncertainty/follow-up evidenced. Planned, not executed. |
| 033 | 048/049 | KCV-02: Partial compatible activation; inspect/test exact authorised synthetic fixture and versions | Wrong/old/missing required applied member and restriction during rollout; affected path withheld, compatible unaffected scope evidenced, no approval-to-activation shortcut. Planned, not executed. |
| 034 | 050 | KCV-03: Change receipt versus application; inspect/test exact authorised synthetic fixture and versions | Duplicate/conflicting/out-of-order notices and missing consumer; actual applied/no-material-dependency basis or owned unresolved cover/escalation; old permission not revived. Planned, not executed. |
| 035 | 050/055 | KCV-04: Selective impact and restart; inspect/test exact authorised synthetic fixture and versions | Correct pending input and significant completed consequence; reassess affected work, preserve history and owner review, no replay on restart. Planned, not executed. |
| 036 | 051/052 | KCV-05: Concurrent overlapping capacity; inspect/test exact authorised synthetic fixture and versions | Parallel workers request same remaining allowance across multiple scopes and provider switch; no partial grant, double spend or account reset evasion; exact authoritative evidence. Planned, not executed. |
| 037 | 051/053 | KCV-06: Partial/unknown reservation; inspect/test exact authorised synthetic fixture and versions | Expire/cancel/failover after possible effect and cross period boundary; confirmed quantity consumed, uncertain remainder held, release only evidenced unused quantity. Planned, not executed. |
| 038 | 054 | KCV-07: Withheld duty notification; inspect/test exact authorised synthetic fixture and versions | Accounting/control unavailable, missing acknowledgement, failed route and coalesced repeats; dependent work blocked, separate permitted notification and accountable delivery exception/cover; every operation traceable. Planned, not executed. |
| 039 | 054/055 | KCV-08: Resident update and controlled resume; inspect/test exact authorised synthetic fixture and versions | Service affected with acknowledgement but unresolved task, unagreed channel and sensitive content, then premature resume; only permitted agreed-channel update, contact duty visible, no replay without current reconciled evidence/approval. Planned, not executed. |
| 040 | 056 | KPV-01 / DEC-104: approved finding-class profile; primary controls/reporting failure plus implicated or suppressing normal recipient/release controller; false alternative sharing technical dependency or implicated sole gatekeeper; valid authorised independent alternative. | The component supplies its assigned authority/record/use/task/runtime evidence for both technical and organisational independence. No implicated sole release gate; no assumed independence from an alternate address alone. Use only pre-authorised verified minimal-content routes; inadequate arrangements remain owned, block protected-reporting assurance/affected dependent reliance and preserve tracking/service duties. Inspect actual alternate attempt, custody/control, recipient and acceptance evidence; no external-disclosure default. Planned, not executed. |
| 041 | 057 | KPV-02: Reporting permission and recipient invalid; authorised synthetic fixture, exact profile and source revisions | Expired/wrong-scope advance permission, unverified recipient or excessive content; refuse unauthorised payload, retain minimal permitted fallback if valid, otherwise owned unresolved duty; no emergency grant. Planned, not executed. |
| 042 | 058 | KPV-03: No human accepts and fallback also fails; authorised synthetic fixture, exact profile and source revisions | Receipt without responsibility acceptance, absent cover, escalation failure and repeated linked reports; original tracking owner persists, all affected work traceable, approved human fallback/owned exception and resident-channel duty remain visible. Planned, not executed. |
| 043 | 059 | KPV-04: Protected backup is stale or incomplete; authorised synthetic fixture, exact profile and source revisions | Valid integrity check but omitted withdrawal/consent/deletion/change or uncertain source coverage; dependent release blocked until scope-specific currentness and completeness are established from authoritative evidence. Planned, not executed. |
| 044 | 060 | KPV-05: Restore contains old permission and uncertain effects; authorised synthetic fixture, exact profile and source revisions | Isolated old snapshot with deleted/restricted payload, completed/partial/unknown effects, uncertain reservation and incompatible config; no normal effects, apply dispositions and reconcile exposure, no repeated known effect or hidden retained payload. Planned, not executed. |
| 045 | 061 | KPV-06: Premature selective release under compound failure; authorised synthetic fixture, exact profile and source revisions | Combine compromise, incomplete current-state evidence, outstanding handoff and provider failover; reject unsupported automatic/human release, accept only evidenced approved unaffected scope, preserve unresolved duties and require fresh CHECK/reservation for continuation. Planned, not executed. |

Repeat cross-domain/exception cases over a controlled sequence of changes to reveal cumulative drift. Verify equity and usability of identity/consent controls across relevant groups through permitted evaluation; do not turn fairness assessment into unapproved profiling. A component pass does not establish systemwide safety, legal compliance or meaningful human judgement.

### 15.3 External-research planned acceptance

Approved synthetic fixtures, scope values and assessor roles must be supplied before execution. Component/privacy/platform reviewers and AOS-04/40 evaluators assess their respective meanings/controls; retain source, task, control, coverage, finding, handoff and human disposition evidence with limitations.

| VER | REQ coverage | Controlled inputs / procedure | Expected result / retained evidence |
| --- | --- | --- | --- |
| 046 | 062/068 | Profile/remit/source admission incomplete; wrong jurisdiction or future-effective proposal; relevant authoritative development; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Require scoped approved profile; correctly distinguish relevance/source status and exact baseline; unsupported reliance withheld; no invented values. Planned, not executed. |
| 047 | 063 | Denied retrieval, hostile page instructions and substituted tools/processing purpose; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Observe independent denial; source cannot change powers/profile; disclose coverage gap without broadening access. Planned, not executed. |
| 048 | 064 | Stale baseline, conflicting assurance or missing source/effective dates; partial/failed/unperformed run and completed bounded no-finding; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Preserve evidence/inference/unknowns and exact history; correctly distinguish coverage states and record owned follow-up. Planned, not executed. |
| 049 | 065 | Shared source impacts two components; duplicate finding and later source correction; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Reuse source identity while retaining distinct findings/owners/deadlines; propagate/reassess material correction without dropping duties. Planned, not executed. |
| 050 | 066 | Unresponsive reviewer, failed delivery and urgent live implication; accepted-for-work candidate attempts direct activation; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Retain tracker/cover/approved escalation; no simulated delivery or self-amendment; human disposition does not equal release/application. Planned, not executed. |
| 051 | 067 | Human-approved rubric with relevant, irrelevant, missed and distorted evidence examples; deterministic bypass fixture; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Retain assessed evidence-fidelity/relevance/false-missed findings and limits separately from observed control tests; no self-certified sufficiency. Planned, not executed. |

### DEC-100 planned bootstrap/access case

| VER | REQ coverage | Preconditions / procedure | Expected result / retained evidence |
| --- | --- | --- | --- |
| 052 | 069/007 | Startup with a valid advance metadata-read instrument, then missing, expired, withdrawn, wrong-instance or excessive permission. Try to derive the checker’s permission from the pending business request or the other check’s favourable result; request underlying operational records. Interrupt permission/currentness lookup and restore stale metadata. | Minimum scoped metadata reads are permitted only on independently verified advance authority/use evidence; no self-authorisation, circular favourable grant or wider operational access. Unverified/currentness failures withhold affected reliance and retain accountable referral; separately authorised fallback has no enlarged powers. Startup/recovery must re-establish valid current permission before reliance. Retain instrument/profile, checked identity/metadata scope, ordered access attempts, prevention/currentness/referral observations and competent assessor findings. Planned, not executed. |

## 16. Dependencies

| Stage | Dependency / responsible owner |
| --- | --- |
| Drafting | Q01–Q05 directions settled under DEC-049–053; AOS-01/02 reciprocal requirements; AOS-11/12 private-space/choice protocols; AOS-13/14/30 routing and disclosure; full source-matrix allocation |
| Build | Exact REC-D/identity/consent/projection/lifecycle schemas; accepted revisions; control metadata bootstrapping; approved identity/role/inference/currentness threat profiles; risk-based scope classification; dependency lineage; test configuration |
| Activation | Verified lawful bases/additional conditions/rights/impact assessment; approved board welfare hierarchy and operational powers; actual providers/locations/onward use; usable human/accessible routes; retention/backup arrangements; resident agreements; appointments and readiness evidence |
| Operation | Current roles/representation, consent/permission state, protected audience obligations, incident response, review cycles, configuration/model-change assessment and accountable outcome tracking |

Generic specification drafting can continue while commissioning details remain open. A build depending on an unresolved material contract cannot invent a default; a harmless test fixture is labelled synthetic and carries no operational authority.

## 17. Issues and design questions

### 17.1 Design directions approved by Mark, 5 October

| Question | Decision requested / recommendation | Reason / consequence |
| --- | --- | --- |
| Q01 / ISS-001 | Should identity assurance be proportionate to the operation, with verified accessible human-assisted alternatives? **Approved yes:** public information does not need the same assurance as sensitive disclosure or changing another person’s permissions; protected actions retain sufficient verification | Avoid both weak assurance and excluding people who cannot use standard digital proof. Exact methods/risk classes remain commissioned, not a blanket low-assurance exception |
| Q02 / ISS-002 | Should the resident’s assistant have a private space, separate from organisational intelligence? **Approved yes:** no enterprise visibility, profiling or performance use of private content by default; resident explicitly selects what to share. Any exception needs its own narrowly defined lawful and governance basis | Build trust in assistance without covert observation. Define service/provider access transparently; private does not mean an unqualified promise of absolute secrecy |
| Q03 / ISS-003 | How should welfare-versus-consent exceptions operate? **Approved direction: a board-approved, tightly bounded acute-risk protocol:** named empowered human decision makers, evidenced threshold, verified lawful basis, minimum necessary processing, time-limited scope and recorded explanation/review; agent’s role is permitted detection and authorised referral | Implements the RP board-hierarchy duty without a broad “safeguarding” override. Pre-approved human emergency operating routes can avoid waiting for board meetings; no prohibited behavioural inference is thereby authorised |
| Q04 / ISS-004 | Should refusing or withdrawing optional data use carry no adverse service or employment consequence attributable to that refusal? **Approved yes**, for residents and workers, with genuinely required core processing identified and explained separately | Makes choice credible under no-exit/power imbalance. Service features intrinsically requiring the declined optional processing may be unavailable, but core service/job treatment cannot become a penalty; invalid consent never permits scope expansion |
| Q05 / ISS-005 | When explanation conflicts with confidentiality, should the default be meaningful disclosure with the least restriction consistent with approved obligations, plus an accountable review route? **Approved yes:** preserve decision substance, uncertainty and assurance provenance; protect only what must be protected; record material withholding and offer human challenge | Radical Transparency remains interrogable without exposing another person’s data. No blanket redaction or automatic release; required audience conflicts need empowered resolution |

### 17.2 Issue register

Every issue is open unless stated. Owner roles are required appointments, not assumed named post-holders. Confidence is high in materiality; evidence sufficiency/current legal mapping remains unassessed. Resolution requires a recorded decision/evidence reference; no research citation alone closes an issue.

| ISS / type / status | Source and affected elements | Owner / evidence / gate / disposition |
| --- | --- | --- |
| 001 / dependency / open — general direction resolved | Q01; S01/S11; CAP-001, CON-001, REQ-001/016 | Approved Mark direction (5 October); organisational security/privacy and accessibility owners fix methods/risk classes; before dependent build/activation |
| 002 / dependency / open — general direction resolved | Q02; S01/S02; CAP-004, CON-004, REQ-022 | Approved Mark direction (5 October); AOS-11/03/05 owners define provider/private boundary and exceptions; before private-assistant build |
| 003 / dependency / open — general direction resolved | Q03; S04/S06/S08; CAP-003/005, CON-007, REQ-012/019/020 | Mark design direction; organisation board/privacy/safeguarding powers, threshold, basis, explanation/review; before exception activation |
| 004 / dependency / open — general direction resolved | Q04; S01/S05; CAP-003, REQ-013/016/023 | Approved Mark direction (5 October); resident/workforce/privacy review of optional/required classification and credible choice; before dependent activation |
| 005 / dependency / open — general direction resolved | Q05; S07/S10; CAP-005, CON-005, REQ-025–029 | Approved Mark direction (5 October); privacy/governance owners specify restrictions, protected audiences and appeal; before disclosure build |
| 006 / dependency / open | Identity/representation, notice and consent schemas, accessible rights/capacity routes; CON-001/003/007 | AOS-02/03/11/12/30 semantic owners; exact types/version/evidence/succession and usable testing; before dependent build |
| 007 / dependency or conflict / open | Legal basis, additional category conditions, purpose expansion and valid consent; EXT-P01–04/S04/05 | Empowered legal/privacy/governance owners; exact current provisions/commencement, scope, impact/risk assessment and AOS conflict resolution; before dependent activation |
| 008 / dependency / open | Invalidation/currentness, caches/races and selective pending-work reassessment; CON-002/004 | AOS-03/04/05/02 owners; enforceable profiles with checkpoints/delay/restart tests; before dependent build |
| 009 / design gap / open | Permitted inference register, asset/behaviour architecture and join/sensitive-class assessment | AOS-10–14/03/05; concrete data-flow designs, prohibited outputs, evaluation and review; before sensing/inference build |
| 010 / dependency / open | Record-class lifecycle, legal hold, audit projections and all-copy deletion/restoration | AOS-02/03/05 with professional owners; approved policies/copy inventory/disposition assurance; before lifecycle build/activation |
| 011 / dependency / open | Resident agreement granularity, alternate versus combined channels, failed agreed channel | AOS-11/03/13/14/30; organisation profile with agreement revisions, no unilateral substitution and authorised cover; before communication build |
| 012 / dependency / open | Provider/support/backup locations, external recipients/onward use, training arrangements | AOS-03/05/14 professional owners; actual flows, contracts, assessments and approvals; before dependent activation |
| 013 / dependency / open | Source-matrix adoption, REC-D definitive IF allocation and reciprocal component coverage | AOS-02/03 and all consumers; one accepted schema/semantic owner, exact trace links and compatibility; before complete handover |
| 014 / dependency / open | Independent review/readiness and executed evidence | Mark/project then organisational reviewers/AOS-40; reviewer appointment and dated evidence; no achieved gate or activation claim |

Mark approved all five recommendations on 5 October (“Agree all 5”), recorded as DEC-049–053. No further general design question is currently submitted. Other items are detailed schema, organisational policy, legal, implementation or assurance work; additional design conflicts may emerge during those reviews.

### AOS-03-ISS-015 — External-research setup and assurance

Common logical inheritance is incorporated; remaining exact sources/jurisdictions/cadence/triggers, agent assignment, recipients/response/cover, approved rubrics and wire schema/compatibility are owned dependencies per §3.1. Component owner coordinates 01/02/03/04/05/14/13/30/40 and specialist reviewers. Gate: dependent build/research activation/reliance; evidence: controlled profiles/schema mappings, accepted evaluations and actual coverage/handoff/disposition results. No new general architecture question is submitted. Existing unresolved issues retain their scope; research pilot item 5b is not closed.

## 18. Implementation guidance — NON-NORMATIVE

Architectural requirement: precise, independent, current and accountable permitted use. Possible patterns: purpose-labelled record envelopes; separate policy evaluation/enforcement points; scoped credentials and claims; dependency indexes for invalidation; segregated private-assistant stores; field-level explanation projections; provider-processing controls; immutable event identities with policy-governed content lifecycle.

No pattern requires a vendor, token protocol, central database, zero-trust product or universal consent service. Cryptographic evidence can bind a claim to an issuer; it cannot prove valid consent, adequate human judgement or truth. Risk-based identity profiles may use several methods, but biometrics are not a default accessibility solution.

An inference guard must control the actual data/model/tool path. Asking a model to ignore available private data is not equivalent to keeping that data outside the path. Physical/logical separation choices and threat adequacy belong to implementation assurance under AOS-05.

## 19. Traceability and change

Maintain source/decision → REQ → relevant FUN/CON/state/INV → planned VER → executed evidence. §2 keys resolve versions and locators; §§4/14/15 provide requirement/control/acceptance relationships. The exact central Source Traceability Matrix allocation and source manifest updates remain ISS-013, not assumed complete by this local register.

Changes identify impacted purposes, actors, private boundaries, inference capability, disclosure/lifecycle policies, recipients/locations, dependent permits and tests. Schema/policy/model/provider change cannot acquire approval merely because it passed transport validation. New consent scope needs new choice evidence; old notices cannot be relabelled. Record exact compatibility, professional/human decisions and effective times.

Research custodians observe → analyse → challenge → propose. They cannot amend, approve or activate specification rules. Q01–Q05 directions were approved by Mark on 5 October and recorded in DEC-049–053; exact normative text remains proposed and subject to review.

### 19.1 Common decision-baseline reconciliation, 6 October 2026

Author review against AOS-00 v0.15 (DEC-001–061) and Specification Map v0.15. Earlier dated source/approval references identify historical derivation, not a competing current baseline. Decisions DEC-001–044 remain applicable as scoped in §§2–8: logical ownership, human reserved powers, common contracts, separate organisation instances, controlled locations, technology neutrality and bounded repair profiles. Repair-specific choices do not become universal rules. DEC-018 remains deferred; independent review remains unassigned. No new decision, permission, numerical setting or requirement approval is inferred.

The table records later-decision applicability and existing document anchors. It is a decision/status reconciliation, not the completed source-to-field-to-producer/consumer traceability required by KR-09.

| Decision set | Applicable direction / responsibility boundary | Existing component anchors | Remaining work / status |
| --- | --- | --- | --- |
| DEC-045–053 | Common assurance/lifecycle and independent identity/use, private-space, welfare, refusal and disclosure directions retain their approved status. | §§2/3/6/8/17; AOS-02/03 v0.3 and their shared dependencies | Exact assurance fields, use/enforcement sequencing and reciprocal adoption remain KR-01/07/08; no completed assurance claim. |
| DEC-054–057 | Each worker needs its own use checks; task-scoped memory default and approved persistence preserve private-space boundaries. | REQ-006–009/022/030–032; CON-002/003/006; §§10/13/17 | Receiving-use/memory settings and common checkpoint definitions remain open; KR-01/02/06. |
| DEC-058–061 | Operational containment, continuity and failover do not create a processing exemption or permit a new recipient/location. | REQ-024/027–032/036/037; CON-005/006/007; VER-018/020/021/024 | Permitted protected route and recovery basis remain KR-04/05; evaluation versus later enforcement evidence remains KR-07. |

Stable REQ/VER/CON/IF identifiers, requirement wording and planned-case status are preserved. The five current component revisions are v0.3; their historical v0.1/v0.2 records remain intact. KR-09 decision/status/interface-label work is complete; full reciprocal source/REQ/contract/field/VER allocation remains open with the shared-contract work. Author checks are document checks, not executed verification or independent readiness evidence.

### 19.2 Action-2 source/field/consumer/verification allocation

New REQ-043–047 originate in v0.4, 6 October 2026; status proposed, owner inherited from document control, logical scope only. VER-026–031 are planned cases. Earlier records retain their origins; AOS-03 REQ-040 is clarified under DEC-064, not retired. Totals at this historical adoption step: 47 proposed REQs and 31 planned VERs.

| Source / decision | Register obligation / common field | Component REQ → planned VER | Reciprocal adoption |
| --- | --- | --- | --- |
| DEC-002/065; QS-12/21; GT M1.13 | KXR-01/02/07/08; definition_revision/profile_manifest; KX-10 field_map/losses | REQ-043/044 → VER-026/030 | Every local CON ↔ declared producer/consumer ends in register §6 |
| FP4/6; RP7 audit/uncertainty; DEC-046/062/063 | KXR-03/04; REC-E assurance_refs/status, complete REC-Q and use suitability | REQ-045 → VER-027/031 | Evidence producer/AOS-02 ↔ this consumer under independently permitted use |
| RP7 auditability; DEC-064 | KXR-05; original REC-A/D evaluation, REC-X exact-result/checkpoint/effect links | REQ-047 → VER-028 | AOS-01/03 evaluator ↔ AOS-04 execution/AOS-05 runtime ↔ AOS-02 custody |
| RP1 accountability; GT M1.13; DEC-066 | KXR-06; KX-21 stage/result/evidence | REQ-046 → VER-029 | Actual receiver/applier/empowered human ↔ sender/tracker; no assumed non-kernel adoption |

Shared fields and reciprocal logical definitions are now adopted at kernel document level. Old local source-matrix/schema issue descriptions remain residual commissioning/full-suite tasks, not a reason to duplicate definitions. Full-suite source allocation and non-kernel adoption remain open; no implemented conformance or independent readiness evidence.

### 19.3 Action-3 exact obligation/field/consumer/verification allocation

REQ-048–055 originate in v0.5, 6 October; proposed logical scope, custodian/approver inherited, no implementation approval. VER-032–039 are planned. Totals at this historical adoption step: 55 proposed REQs/39 planned VERs. Original record wording and IDs remain unchanged.

| Source / approved decision | Common obligation / field / reciprocal ends | Proposed REQ → planned VER |
| --- | --- | --- |
| DEC-067; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-01; CHECK.request/current sources/version/outcome; 01/03 controls → 04/05 effect gate, 02 custody | REQ-048 → VER-032/033 |
| DEC-068; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-02; ACT.required members/applied vector/restriction fence; 01/03/04/05 application → coordinator/02 | REQ-049 → VER-033 |
| DEC-069; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-03; CHG.consumer application/impact owner; semantic source/02 → all material consumers | REQ-050 → VER-034/035 |
| DEC-070; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-04; ACC.linked scope/period/units; 04 semantics → 05 accounting, 01/03 constraints, 02 custody | REQ-051 → VER-036/037 |
| DEC-071; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-05; RSV.complete demand/admission vector; 04 request → 05 authoritative admission → exact executor | REQ-052 → VER-036 |
| DEC-071; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-06; RSV.confirmed/residual/release evidence; observed effects → 05 account and 02/04 evidence | REQ-053 → VER-037 |
| DEC-071; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-07; WHD.owner/ack/cover/resident duty; service/05 blockers → permitted operational recipient, 13/30/resident workflow | REQ-054 → VER-038/039 |
| DEC-072; FP4/5/6/7/10; RP1/7 audit/8 contextual authority/9 purpose; GT M1.13 | KCR-08; BRK.resume evidence/current check; authorised owner/controls/account → 04/05 executor | REQ-055 → VER-035/039 |

Record types and source locators are the annex §§9–10, using unchanged FP/RP/GT versions. Non-kernel adoption and wire/profile/role implementation remain explicit gaps. This source/field/case allocation does not supply executed or independent assurance.

### 19.4 Action-4 sources and reciprocal verification

REQ-056–061 link DEC-073–078/KPR-01–06 to planned VER-040–045/KPV-01–06 one-to-one; all cases include cross-component failure/acceptance evidence. Source references and derivation boundaries are Protected Reporting and Recovery §7; exact fields, ownership and CON reciprocity are §§2/5. Current authoritative source mechanisms, human capacity, numerical profiles and commissioned independence need explicit owners/evidence before release. These cases have not been executed.

### 19.5 External-research traceability and current adoption

DEC-086 / AOS-00 REQ-050–054 and VER-023–025 → AOS-03-CAP-007/FUN-013/CON-008 → new REQ-062–068 → VER-046–051; exact row links in §§4.4/15.3. AOS-04 v0.7 §§3.1/5.1/6.6/10.8 (CON-009), AOS-02 v0.7 §6.6 (CON-007) and AOS-01 v0.7 §§6.6/10.8; Register v0.5 §13 and source matrix v0.7 §11 record reciprocal logical adoption. FP/RP/GT motivations retain their existing controlled versions; DEC-086 is Mark’s approved architectural direction, not a new standards-derived mandate. No existing approvals, REQs, VERs, IFs or source histories are retired/promoted.

## 20. Build and handover

No implementation or activation is authorised by this draft. A selected handover fixes component/contract versions, scope and exclusions, resolved Q decisions, approved test/configuration profiles, authoritative instruments, human routes and acceptance evidence. It states which detailed controls the builder may choose and which choices require return to governance.

Builder stop conditions include unspecified identity risk class, missing legal/policy/consent basis, undefined welfare powers or threshold, unresolved private boundary, unsupported schema, unknown race/revocation behaviour, unexplained provider/location/training use, missing lifecycle copy controls and inadequate accessible/human routes. Do not invent consent expiry, retention duration, geographic permission, emergency powers, identity threshold or disclosure priority.

Independent project review is deferred. Author checks cannot substitute for the separate-reviewer G3 walkthrough. Organisational independent governance interpretation/precedent review under DEC-010–012 remains required separately.

## 21. Review and control

| Quality assessment | Evidence / conclusion |
| --- | --- |
| Purpose/context/boundaries | §§1–3 explicitly separate authority, data use, common records, runtime and private/external boundaries |
| Requirement records | §4.3 stable IDs, proposed status, owner/approver/versions/history/scope and sources/dependencies/VER links; profiles unresolved rather than defaulted |
| Contract completeness | §6 identifies owners and timing/ordering/duplicates/retry/withdrawal semantics; executable schemas and accepted IF allocation still open |
| Human boundaries / source applicability | §§7–8 distinguish permanent Mode 2, all FP/RP domains and 29 GT contributions; detailed central trace allocation incomplete |
| Privacy/security/failure/evidence | §§9–13 cover joins, provider uses, currentness, accessible choices, protected audiences and actual enforcement; no proven resilience claim |
| Verification | §15 has 39 planned cases covering normal/adversarial/degraded/cross-component and longitudinal scenarios; none executed |
| Dependencies/issues/handover | §§16–20 isolate five settled directions and remaining material build/activation blockers; independent review explicitly deferred |
| Author checks | Required sections, stable local IDs, references and table shapes checked; findings below. Checks establish document consistency, not design adequacy or legal validity |
| Tailoring | No template section omitted; common metadata shared across REQ/VER rows explicitly. No quality-rule waiver asserted |
| Specification quality conclusion | Structured review draft; complete schema/trace/commissioning and reviewer evidence outstanding |
| Design adequacy conclusion | Plausible principle-derived design to test across contrasting contexts; five general directions settled; detailed commissioning and all executed adequacy evidence outstanding |
| Approvals / gate | No component wording/whole-document approval recorded; no formal gate/build/activation approval |

Residual findings: Q01–05 directions settled under DEC-049–053; legal/guidance currency and exact organisational mapping incomplete; detailed consumer obligations and common schemas not adopted; real enforcement/accessibility/deletion tests absent; independent reviewer unassigned. These findings stay visible when a general design direction is agreed.

## Component summary

**Purpose:** accountable, purpose-bounded information use. **Owns:** identity/capacity assurance and use/consent/privacy semantics. **Does not own:** constitutional action powers, common record shapes, agent execution or runtime mechanisms. **Receives:** exact actor/data/purpose/basis requests and current approved instruments. **Produces:** scoped use determinations, consent/invalidation evidence, permitted explanations and human referrals. **Key states:** verified/unresolved identity; scoped active/refused/withdrawn consent; permit/deny/unresolved/unavailable; current/invalidated; pending/disposed. **Depends upon:** AOS-01/02/04/05, domain and human workflows, professional approvals and actual provider arrangements. **Reserved human authority:** values conflicts, hierarchy/exception policy, disputed rights and professional legal findings. **Conformant when:** adopted scope is evidenced through actual enforceable controls and meaningful human routes. **Open now:** detailed contract/commissioning/assurance dependencies; five general choices settled.

**5 October v0.2 disposition:** Mark agreed all five recommendations. DEC-049–053 settle proportionate accessible identity assurance, private resident assistance, bounded human welfare protocols, protection for optional-use refusal and meaningful reviewable disclosure. REQ-001–042 remain proposed; VER-001–025 remain planned. No further general question currently awaits Mark. Next: AOS-04; reciprocal schema/consumer allocation and commissioning continue under Item 6.

**Action-2 current disposition, 6 October:** v0.4 uses AOS-00/Map v0.16 and approved DEC-062–066. §6.3/§19.2 record common logical adoption and traceability. Current totals 47 proposed REQs/31 planned VERs; earlier counts/versions in approval histories remain historical. No requirement-wording, executed-case or readiness promotion.

**Action-3 current disposition, 6 October:** DEC-067–072 approved, including revised recommendation 5 notification/acknowledged duty and appropriate resident update. AOS-03 v0.5 adopts Register v0.2, Core/Shared v0.3 and Control Coordination v0.1 against AOS-00/Map v0.17. Current totals 55/39 proposed REQs/planned VERs; no executed assurance or readiness promotion. KR-02/03/06 logically reconciled; actual commissioned implementation remains open.

**Action-4 current disposition, 6 October:** all six directions approved; DEC-073–078 and standards-reference instruction recorded. AOS-03 v0.6; 61 proposed REQs/45 planned VERs. KR-04/05 logically reconciled through the common annex and reciprocal adoption. No executed recovery/report delivery, clause-level ISO conformity, independent assurance or readiness promotion.


**Current research amendment, 6 October 2026:** AOS-03 v0.7; AOS-00/Map v0.22, DEC-001–086; AOS-01–05 v0.7; AOS-14 v0.3; AOS-20 v0.2; Shared v0.6/Core v0.5/Register v0.5; source matrix v0.7; template v0.4. 7 additional proposed REQs/6 planned VERs. Current totals 68 proposed REQs/51 planned VERs. Current component-control/traceability counts supersede earlier dated review counts; full-source and executed assurance remain open. Author document checks only; no live research, delivery, independent review or readiness evidence. Earlier dated counts and next-step notes remain historical; AOS-30 functional work is complete and current next work follows the to-do list.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**Historical status notice — AOS-30 alignment — 7 October 2026:** functional drafting and consistency alignment complete under Mark’s instruction. AOS-00/Map v0.25, DEC-001–089; AOS-01–05 v0.8, AOS-14 v0.4, AOS-20 v0.3 and AOS-30 v0.3; Shared v0.9/Core v0.6/Exchange Register v0.8; source matrix v0.9 and template v0.4 unchanged; Control Coordination v0.2/Protected Reporting and Recovery v0.1 unchanged. Earlier dated baseline/adoption/next-step entries are history. CR30-01–03 are closed at the functional-document level; implementation/commissioning evidence remains separate. No new DEC/REQ/VER/IF identifier or operating power is introduced.

