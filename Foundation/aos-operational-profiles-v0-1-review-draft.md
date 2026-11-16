# AOS operational profiles — review draft

Document: aos-operational-profiles-v0-1-review-draft · Source revision or record: v0.6

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**DEC-105 adopted — 29 October 2026:** Current revision 0.6. Operational technical-control reliance requires declared scope/limits and accepted observed enforcement/failure/recovery evidence; build/prototype and G4/live approval gates remain separate. [Decision/amendment record](../Supporting-Specifications/aos-dec-105-technical-control-limits-and-evidence-2026-10-29.md). Earlier counts/baselines are dated history; current inventory and annex addendum control catalogue navigation. Existing non-waivable rules and DEC-099–104 retained; all new cases/variants remain planned/unexecuted.

**DEC-104 adopted — 29 October 2026:** Current revision 0.5. Each mandatory protected-finding category requires assessed technical-failure and implicated-person interference arrangements with an appropriately independent authorised alternative and no implicated sole release gatekeeper. [Decision/amendment record](../Supporting-Specifications/aos-dec-104-protected-reporting-and-implicated-recipients-2026-10-29.md). External reporting is conditional on justified lawful authority, not a default. Exact profiles/permissions, protected_finding v0.3 compatibility and actual evidence remain gates; amended wording retains ordinary separate review and cases are planned/unexecuted. Earlier contrary or narrower baselines are history for this scope.

**DEC-103 adopted — 29 October 2026:** Current revision 0.4. Decision validity/effective time, attributable evidence/authentication, minutes approval and permission to execute are separate. DEC-087 is partly superseded; [decision/amendment and legal-source record](../Supporting-Specifications/aos-dec-103-decision-validity-evidence-and-minutes-2026-10-29.md). No universal later-minutes or second decision-record approval gate. Exact instruments/evidence policy, KX-06 v0.3 compatibility and ordinary separate review/readiness gates remain required; cases unexecuted. Earlier contrary wording is historical only where explicitly identified.

**DEC-102 adopted — 29 October 2026:** Mark approved demonstrated adequacy of organisation-defined classifications/settings against governing constraints. Current document revision 0.3; see the [decision and amendment record](../Supporting-Specifications/aos-dec-102-classification-and-configuration-adequacy-2026-10-29.md). Earlier baselines are dated history. DEC-099–101 retained; detailed amended requirements remain subject to separate review/readiness gates and cases remain planned/unexecuted.

**DEC-101 adopted — 29 October 2026:** Mark approved demonstrated human capacity and meaningful review as conditions of operational reliance. Current document revision 0.2; [decision and amendment record](../Supporting-Specifications/aos-dec-101-human-capacity-and-meaningful-review-2026-10-29.md). Earlier dated baselines remain history. DEC-099/100 are retained; requirements remain amended proposed wording and cases planned/unexecuted, with separate review/readiness gates unchanged.

| Document control | Value |
| --- | --- |
| Working identifier | AOS-OP; drafting annex to the shared and core record contracts, not a new component |
| Version / date | 0.6 / 29 October 2026 |
| Status | Review draft; architectural directions approved, detailed wording and profile values proposed/open |
| Project owner / baseline approver | Mark Sweeny |
| Author | Codex, at Mark's request |
| Independent review | Deferred; no independent assurance claimed |
| Scope | Reusable operational profile definitions, organisation configuration and synthetic overdue-repair example |
| Baseline | AOS-00 v0.10; Specification Map v0.7; AOS Shared Contracts v0.1 and Core Record Contracts v0.1, with 4–5 October approval dispositions |
| Approval boundary | DEC-031–041 record Mark's 5 October approvals of the two five-question sets and resident-agreed channels; no operational delegation, legal basis, exact schema, whole-document or build approval follows |
| Quality basis | Existing AOS-QS v0.1 and component template v0.3; this annex develops profiles for subsequent component adoption |
| Readiness | Drafting/review only; no G2/G3/G4, implementation or activation approval |

## 1. Purpose and place in the project

This document specifies the configuration that makes the four common record families usable: evidence (REC-E), authority (REC-A), data use (REC-D) and execution (REC-X). It complements rather than duplicates their logical fields and lifecycles in [Core Record Contracts](aos-core-record-contracts-v0-1-review-draft.md). The [Shared Contracts dossier](aos-shared-contracts-v0-1-review-draft.md) remains the joint interface catalogue.

The reusable AOS must identify the controls and evidence every organisation needs. Each organisation supplies its valid operational instruments, appointed roles and numerical settings. A synthetic demonstration illustrates the composition without supplying sector defaults.

The first demonstration remains one overdue repair, not a production repairs service. The complete AOS specification remains the wider objective. No supplier, database, model, credential format or transport is selected.

### Source and decision derivation

This annex uses the controlling architecture, map and the two contract drafts consulted in this thread; it does not claim a new full reading or independent revalidation of the FP/RP/GT source set. Those governing sources and the existing source manifest retain their standing. Complete source-item allocation must be extended during component drafting.

| Direction | Source / standing | Application here |
| --- | --- | --- |
| Overdue resident promise; human escalation; owner and team contacts | DEC-021–023/026; architecture §1; REC-R21–23 | Sections 4–6 and 10 |
| Withhold action when permission is missing; shared enforcement | DEC-003/005; REC-R06–16 | Sections 5, 7 and 8 |
| Current check, material correction and reconciliation | Approved DEC-028–030; Core Records §11 | Sections 4, 7 and 8 |
| Preserve conflicting accounts; dispute prevents automatic closure | Approved DEC-031, 5 October | Sections 4 and 6 |
| Bounded automatic detection/escalation/factual contact; reserved human decisions | Approved DEC-032, 5 October | Section 5 |
| Named human acknowledgement; originating workflow tracks pending handoff | Approved DEC-033, 5 October | Section 6 |
| Visible unresolved state; authorised fallback; pause dependent actions | Approved DEC-034, 5 October | Sections 6–8 |
| Organisation configuration, labelled synthetic fixtures and minimal repair data | Approved DEC-035, 5 October | Sections 2–3, 9–10 |

## 2. Three distinct layers

| Layer | Contains | Who supplies or approves it |
| --- | --- | --- |
| Reusable AOS definition | Profile meaning, required settings, non-waivable constraints, evidence and failure behaviour | Project baseline process; Mark currently approves design direction |
| Organisation configuration | Approved action schedule, processing rules, roles/cover, source mappings, clocks, deadlines, retention, recovery and permitted channels | Relevant commissioning/governance/operational authorities; their actual identities and powers must be established |
| Synthetic fixture | Fictitious repair, identities, events and illustrative profile values for a planned demonstration | Project review; clearly labelled and isolated from live systems |

Approval of one layer does not approve the others. A profile placeholder has no default value. A synthetic actor or permission is not a live appointment or delegation. Organisation configuration cannot waive foundational constraints or expand reserved human powers.

### DEC-101 — human capacity and meaningful-review acceptance

Every workflow that depends on human judgement must demonstrate sufficient empowered human capacity and meaningful review before operational reliance, with proportionate reassessment during use. Capacity includes realistic demand, response arrangements, cover and owned unresolved duties. Meaningful review requires observable evidence that people can understand the material, question an AI recommendation, introduce other evidence and exercise their own judgement.

The organisation approves workflow-specific assessment criteria, competent assessors and review triggers. Representative exercises include absences, demand surges and materially flawed AI recommendations. Speed, agreement with AI, signatures and acceptance clicks are insufficient individually to establish good or bad judgement; assessment concerns observable process and evidence, not claimed access to a person’s internal thought. If required capacity or review conditions cease to hold, the affected workflow enters its approved degraded or human fallback arrangements. Service duties remain owned; workload pressure cannot discard mandatory referrals or silently widen automation permissions. Separately permitted urgent/service action retains its existing authority; this decision grants no emergency power, universal staffing ratio, deadline, pass rate or individual surveillance permission.

The accountable service/governance owner supplies capacity and approved degraded/fallback arrangements; empowered human reviewers exercise actual judgement; AOS-30 carries the workflow and evidence; AOS-13 retains operational tracking; AOS-40 assesses the evidence against the approved scope and rubric. The profile records demand assumptions, role/powers/competence, information and accessible review facilities, cover, response/queue limits, representative/adverse exercises, assessment method/assessor, results/limitations, reassessment triggers and action on deterioration. Missing mandatory evidence prevents a readiness claim for the affected use. No software pass alone certifies an institution’s judgement.

### DEC-102 — classification and configuration adequacy

Organisation-defined classifications and settings must demonstrate that they preserve AOS governing constraints before they can be relied upon. Accountable competent assessment is required before use and after material changes; authorisation alone does not establish adequacy. Missing or inadequate settings block the affected reliance and require owned resolution.

Classification considers actual effects on organisational commitments, protected information, rights, services, financial exposure and resource use, including cumulative effects; financial and resource consequences remain distinct. Settings cannot transfer permanently reserved human judgement to automation, remove mandatory reporting, manufacture data-use permission or bypass a prohibition. “Consequential” triggers the applicable controls; it does not automatically require individual human approval for every properly delegated routine action. Organisations retain responsibility for justified local values and legitimate powers. No universal threshold, duration, moral weight or permission is supplied by this decision.

The profile identifies its owner/approver and competent assessor, scope, governing constraints, chosen values/class definitions and reasons, financial/resource units and aggregation assumptions, normal/boundary/cumulative/adverse examples, assessment evidence/limitations, material-change triggers and action on missing or inadequate settings. An AI recommendation or approval record is insufficient by itself. Actual effect and applicable constraints govern assessment, not the label assigned to an operation. A smaller action cannot evade a bound by splitting related work; mandatory reporting and reserved judgement remain protected. AOS-01 owns the governing validation obligation with relevant domain/control owners; AOS-40 assesses scope-specific gate evidence; profile owners supply the actual configuration and review. Dependent effects remain withheld where required, while separately permitted service/reporting duties retain their own powers and owners.

### DEC-103 — separate decision, evidence, minutes and execution

AOS shall distinguish the validity and effective time of a human decision, the provenance/authentication and evidential standing of its record, the separate approval status of minutes, and current permission to execute an action. It shall assess decision validity and sufficient evidence under the organisation’s applicable law, legal form, constitution/registered rules, powers and approved evidence/reliance policy. It shall not universally require later minutes approval to bring a decision into existence, nor require a second board approval of a separate decision record where those applicable arrangements do not require it.

Minutes approval and authentication are evidence events, not universal substitutes for the actual decision process. An authenticated record or extract may support reliance through an authorised evidence route, but neither its signature nor its label can manufacture a decision, cure missing powers/conditions or make disputed evidence conclusive. Preserve actual decision, record, authentication/approval, effective and execution times separately; no automatic backdating. Contradictory, missing or insufficient evidence withholds affected automated reliance for accountable human resolution without declaring that an otherwise valid legal decision does not exist. Organisation-specific additional assurance gates may be adopted, but must be labelled as AOS/organisation reliance policy rather than general law. Separately authorised urgent/service duties remain owned. Minute-taker drafting and Company Secretary stewardship remain distinct; human decision powers, protected constitutional processes, boardroom AI exclusion, current authority/data-use checks and DEC-088/089 remain unchanged.

The approved organisation profile binds legal form/jurisdiction, actual constitution/registered rules and powers, valid decision/record/authentication routes, relevant statutory evidence standing, exact required source/validity conditions and competent evidence-assessment/escalation roles. AI cannot infer unseen deliberation or declare legal validity; record the authorised human assessment and limits. No compulsory extra decision-wording approval is invented. A stricter automated-reliance threshold is explicit policy. KX-06 v0.3 is a revised logical view; exact types, code lists, required/conditional fields and reviewed old/new consumer compatibility must be fixed before dependent use. DEC-087 original text is history to the extent superseded; role separation and protected powers remain.

### DEC-104 — protected reporting under failure and implicated-person interference

Each mandatory protected-finding category shall have an approved reporting arrangement assessed against both technical failure and interference by implicated people. The profile shall identify the intended recipient, possible conflicts and an appropriately independent authorised alternative; an implicated person shall not be the sole gatekeeper deciding whether the required finding reaches its authorised audience.

Authority/use permissions, minimum report content, recipient verification, custody, route/change dependencies, tracking ownership, acceptance, cover and escalation are established in advance. An external route is included where justified and lawfully authorised; external reporting is not a universal default and a finding creates no extra disclosure power. Planned exercises address failed infrastructure, unavailable/implicated recipients, apparent alternatives controlled by the same implicated gatekeeper and attempted suppression. Missing adequate arrangements remain an explicit owned gap, prevent claims of operational protected-reporting assurance and withhold affected dependent reliance under existing gates; they do not create false delivery, ownership transfer or blanket shutdown of separately authorised service. Original tracking duty persists until actual scoped acceptance.

The organisation’s profile binds each required finding class to normal/alternate authorised audiences, conflict criteria/evidence and accountable assessment, disclosure basis/minimal payload, independently verifiable recipients/permissions, credentials/custody and route/reconfiguration controls, failure/compromise assumptions, tracking/cover/escalation, human fallback, evidence and review triggers. Test both infrastructure/common-dependency independence and organisational release/recipient/custody control; neither implies the other. No administrator, executive sign-off or report-validation step may silently remove a required duty. The declared threat/governance scope and residual limitations must be visible: this is not an unlimited guarantee against every holder of legal/constitutional change powers. Inadequacy returns to an empowered accountable reviewer; the reporting agent cannot invent a recipient or grant itself onward-disclosure authority.

### DEC-105 — declared technical control limits and observed assurance

Operational reliance on implemented technical controls requires explicit scope, limits and failure/recovery behaviour supported by accepted observed evidence. The evidence must cover all enabled action paths within the declared control/threat scope, independently of the acting agent; permission-change enforcement points and timing uncertainty; shared cumulative bounds under concurrency; conservative treatment of unknown effects/reservations; and recovery that applies current restrictions without reviving withdrawn authority or repeating completed effects.

The approved control profile fixes exact functions/paths/dependencies/versions, threat assumptions, effect boundary, currentness and revocation/fencing mechanism, timing/uncertainty bounds and units, accounting scopes/consistency and admission, uncertain exposure/release evidence, recovery source/currentness/completeness, permitted fallback/continuing duty, observability/oracle, assessors and objective acceptance conditions. Timeout, cancellation, worker retirement or failover alone cannot prove no effect, release possibly used capacity or permit consequential repetition. No instantaneous global revocation or recall of an irreversible disclosure is promised. Limits are assessed under actual constraints and powers, not silently accepted as waivers of non-waivable safeguards. Missing/failed evidence blocks affected operational-reliance claims with an owned remedy; separately authorised service/reporting duties remain owned and do not acquire extra permissions.

G3 remains authorisation of a bounded build with fixed scope, explicit dependencies/profiles and required separate review; G4 requires implemented observations, and actual operational approval is separate. An explicitly authorised bounded prototype can investigate the mechanisms before operational assurance exists; this decision itself authorises neither a prototype nor live effects. A failed prototype requires investigation of the implementation, assumptions and alternatives; it is not alone proof of architectural impossibility. Model refusal, a generated explanation, intended configuration, an old checkpoint or retrospective log alone is not evidence that all effect paths were enforced or recovery was current. Actual acceptance must link observations to the exact requirement/local-case/variant/profile and endpoint scope, with limitations and competent assessor disposition.

AOS-05 produces control-boundary/dependency observations and declares the implemented limits with authoritative semantic/control owners. AOS-40 evaluates scoped acceptance and preserves build, implementation-verification and operational approval distinctions. Approved profile/instrument owners determine legitimate settings; accountable human assessors disposition limitations without waiving non-waivable constraints.

## 3. Common profile control record

Proposed logical fields below complement the existing record envelope; final component schema adoption remains open.

| Required field/group | Meaning and validation |
| --- | --- |
| Profile identity, kind and exact revision | Stable identity and accepted revision; incompatible versions cannot be silently coerced |
| Organisation and applicable scope | Case/action/data/source classes covered; separate instances remain separate |
| Semantic owner and accountable configuration role | One controlled definition and an accountable role; actual appointments evidenced |
| Approving authority and instrument references | Exact approved records and evidence that the approver holds the required powers |
| Effective period and current state | Draft, approved-but-not-active, active, suspended or retired; proposed vocabulary only |
| Parameters and completeness result | Explicit typed values/units or unresolved fields; unresolved required settings block their dependent capability |
| Dependencies and compatibility | Referenced contracts/profiles, supported versions and cross-component impact |
| Change/supersession evidence | Reason, earlier version and approval/effective-time history |
| Verification and activation evidence | Planned/executed status, results, environment and authorised activation; a populated record does not prove readiness |
| Access and retention policy references | The profile and its approval evidence are themselves governed records |

Activation requires the applicable organisational approval, current compatible dependencies and readiness evidence. Publishing a draft file does not activate it. Corrections preserve earlier versions; changed action scope or material parameters require fresh determinations.

AOS-02 owns the common structure. The responsible semantic owner defines each profile's meaning. AOS-01/03/04/05 apply the appropriate policy, processing, execution and runtime controls; technical access alone confers no approval power.

## 4. Fact, source, time and correction profile

**Owners:** AOS-02 with Asset/Process; corresponds to P02.

The profile must distinguish resident-communicated completion promise, internal target, contractor completion claim, verified completion, resident disagreement, partial completion and case closure. Each assertion retains source, revision, event/effective/receipt times, precision and restrictions. A closed job flag alone does not establish that the repair was completed.

Under DEC-038, an approved repair-specific evidence rule requires an identifiable completion record with supporting work or inspection evidence. A contractor job-closed flag alone is insufficient; resident confirmation can support completion, but silence cannot establish it. The source profile specifies which records can establish each fact, what corroboration is required, who resolves disagreement and the evidence of that resolution. It must not silently turn source precedence into a finding that a resident account is false.

Under DEC-031, conflicting accounts coexist and completion becomes disputed. Route the dispute to accountable review. Prevent automatic closure while unresolved; permitted communication and escalation may continue. Under DEC-029, reassess only pending work materially dependent on changed evidence. Preserve completed history and review significant consequences.

Under DEC-039, once the promised boundary has passed, unknown completion triggers accountable verification escalation labelled **completion unverified after promised date**, rather than a definite incompletion assertion. Resident notification explains uncertainty accurately and provides appropriate contacts. Under DEC-040, outstanding work within the promised scope means the original repair remains incomplete; preserve completed and outstanding elements separately. Scope redefinition or a new promise requires authorised human review and resident communication; job splitting cannot erase the original commitment.

Required settings include source identifiers and repair matching, partial completion semantics, duplicate/correction ordering, dependency mapping, accountable review authority and permitted resolution evidence.

**Approved comparison direction (DEC-036):** a calendar-date promise becomes overdue once that date has ended in the organisation’s approved timezone; a precise promised time uses that time. No automatic grace period. Actual timezone/calendar mapping, source precision, clock uncertainty and reevaluation mechanisms remain profile settings. Do not invent precision absent from the promise.

A later internal target or uncommunicated date cannot reset the resident promise. A promise amendment requires authorised change and resident communication evidence; a new promise itself requires the human decision specified in section 5. Under DEC-037, preserve the original promise and any breach already incurred; a revised date cannot automatically close an existing escalation.

## 5. Action and delegation profile

**Owners:** AOS-01 with AOS-04/13/20/30; corresponds to P07.

DEC-032 permits the following demonstration behaviours only within approved delegation, data-use permission and current control checks.

| Action class | Approved design direction | Configuration/evidence required |
| --- | --- | --- |
| Detect overdue condition | May be automatic | Valid source/time profile; permitted processing; evidence and limitations |
| Create internal escalation | May be automatic | Trigger rule, authorised audience, accountable route and trackable handoff |
| Send factual resident notification | May be automatic | Approved content scope, channel(s) agreed with the resident, recipient binding and current valid owner/team contacts |
| Make a new completion promise | Authorised human decision required | Decision-maker's powers, exact new promise and communication evidence |
| Commit expenditure | Authorised human decision required | Applicable schedule, scope/amount and decision evidence; no implied budget |
| Close a contested case | Authorised human decision required | Resolution authority, preserved dispute accounts, rationale and evidence |
| Repeat a potentially consequential effect | Reconciliation required first | Approved permitted continuation or authorised human next decision, with fresh controls |

The factual notification reports evidenced status and contacts. It must not invent a completion date, assure an outcome unsupported by evidence or include unnecessary personal information. A dispute is disclosed only to the audience and level permitted by the data-use/explanation profiles.

This table does not create universal production autonomy, settle every action's consequential classification or approve live operational permission. Organisations classify actions and approve their schedules within the reusable constraints. A human instruction cannot waive a core prohibition or automatically provide a processing basis.

## 6. Handoff, contact and closure profile

**Owners:** AOS-13/30 with AOS-11; corresponds to P06.

Under DEC-033, message delivery is not acknowledged responsibility. A named authorised human acknowledges the case/action scope and responsibility. Until then, the originating workflow tracks the uncompleted transfer. The organisation must also appoint the accountable human role for that tracking workflow; software is not institutional accountability.

Proposed handoff states: prepared, dispatched, delivery confirmed, awaiting acknowledgement, acknowledged, response overdue, referred to authorised fallback, resolved, or unresolved. Delivery and acknowledgement evidence are distinct. An acknowledgement does not prove the repair is resolved.

Required configuration: receiving role/holder, acknowledgement and response deadlines and their clock basis, available cover, acknowledgement mechanism, reassignment/rejection route, non-response escalation and closure authority. Identity and powers are checked at the relevant time. A rejection or absent recipient leaves the transfer incomplete.

The resident must receive valid contact details for both the named case owner and accountable repairs team through a permitted channel agreed with that resident. Under DEC-041, all communication with the resident uses the applicable resident-agreed channel(s). Record the agreement’s source, scope, current revision and agreed channel set, with the chosen channel(s) and agreement reference bound to the action. The profile must specify whether agreed channels are alternatives or required in combination; a set alone does not establish that. Agreement changes require evidence and reassessment of affected pending sends. Resident channel agreement is distinct from processing permission and does not itself supply a legal basis.

**Proposed failure handling:** where no current agreed channel can be established, or the applicable agreed channels are unavailable, retain communication as unresolved and route to an authorised human to establish/reconfirm the agreement or arrange a permitted response. Use another channel only where the agreement already allows it and current controls permit it; do not silently substitute an unagreed channel. Detailed accessibility, preference-change and multi-channel ordering rules remain profile work.

Missing contacts prevent claiming complete contact provision; the workflow may still pursue an authorised route to obtain them. A delivered notification does not automatically establish resident receipt or usable contacts.

Under DEC-034, non-response keeps the case visibly unresolved. An escalation to the fallback route is itself tracked to accountable receipt. If no permitted fallback exists, preserve the unresolved state and surface the gap through an available separately authorised incident/review route. Do not fabricate a recipient.

Separate closure conditions must be specified for execution attempt, handoff, escalation and repair case. A dispatch record cannot close all four. Contested case closure needs the section 5 human decision; dispute resolution must preserve both accounts and accountable rationale. Where certainty cannot be recovered, an administrative disposition must explicitly preserve unresolved facts and further duties rather than label the repair completed.

## 7. Enforcement, identity and unavailable controls

**Owners:** AOS-01/03/04/05; external exchange profile with AOS-14; corresponds to P03/P04/P12.

Before the consequential effect, validate current authority and data use at the last enforceable point, as approved under DEC-028. Bind results to exact actor/principal, action, case, payload, recipient, purpose and material context. Earlier planning checks cannot substitute after material change.

The organisation/implementation must define the enforceable boundary, freshness, propagation and clock limits, interruption handling, changes during irreversible action and bypass threat model. A current-looking timestamp alone is not proof of enforcement. Irreversible effects are preserved as historical facts and handled through authorised follow-up.

Unavailable/denied/unresolved authority or data use withholds dependent actions. Separately permitted work and fallback can continue; their permission must be independently established. Identify which capability depends on each setting/control so outages do not unnecessarily freeze unrelated work.

Identity profiles must establish the relevant principal, delegation lineage, actor provenance and current restrictions proportionately to exchange. Source authentication, valid delegation and permitted data use are distinct checks. Cross-organisation federation remains deferred; no identity system or cryptographic format is prescribed here. External trust evidence acceptance and disclosure rules remain explicit prerequisites.

## 8. Recovery and effect reconciliation

**Owners:** AOS-04/05/13/14; corresponds to P09.

Retain the intended action and required pre-effect evidence, dispatch attempts and resulting effect evidence. Use separate outcomes for known success, known failure, partial effect and indeterminate effect. The vocabulary remains proposed; timeout never proves failure.

Under DEC-030, investigate prior possible effect before consequential repetition. Status queries need their own authority/data-use checks. Automatic continuation is permitted only under an approved action-specific profile establishing permitted action without duplication or compounding. Otherwise an authorised human determines the permitted next action. That decision cannot reverse an irreversible disclosure or waive controls.

Required settings: reconciliation evidence/source, query permissions, repeat/compensation scope, attempt limits/backoff/timeouts, evidence availability, restart behaviour, manual fallback, accountable handoff deadline/cover and operating capacity. No numerical retry count, service target or recovery interval is adopted here.

Restart rechecks current permissions and preserves suspension and unknown effects. If required recording is unavailable, pause actions dependent on that recording boundary; invoke only an approved alternative evidence/fallback route. Blind replay of resident contact, commitment or expenditure is prohibited by the approved reconciliation direction.

## 9. Data use, explanation and analytical review

**Owners:** AOS-03 with AOS-02/11/12/14/20–25/30; corresponds to P05/P08/P10/P11.

DEC-035 limits demonstration data to establishing repair status, routing accountability and communicating with the resident. The proposed minimum set comprises repair/case linkage, resident-communicated date and communication evidence, relevant completion/dispute evidence, authorised resident contact and applicable channel-agreement references, owner/team contact references, determinations and execution/handoff history.

Need is assessed per audience and operation. Do not copy resident contact information into every event or expose an entire repair history when a restricted projection suffices. This annex supplies no legal basis, consent override, universal retention period or verified legal mapping.

Required organisation settings include processing purposes and permitted operations, applicable approved basis, access/disclosure/inference restrictions, consent dependency and withdrawal handling where applicable, data locations, retention/deletion by record class and restrictions on derived records. Preservation of accountability history must be reconciled with approved retention/deletion obligations rather than treated as unlimited retention.

Explanation follows DEC-027: meaning, authority basis and referral route by default; recorded/reviewed exceptions for the established grounds. Define permissible redaction, exception authority and review evidence. An explanation exception never removes the underlying control.

Analytical profiles distinguish source assertion, validated fact, inference, provisional recommendation and approved human decision. Define uncertainty rubric, materiality review and canonical presentation. The demonstration may use deterministic factual checks; it does not establish GI analytical quality or permission for resident/workforce profiling.

## 10. Synthetic demonstration fixture

**Fixture identity:** FIX-OP-01, proposed for review. All identities and records below are fictitious; no live residents, contractor systems or communications. Numerical settings are deliberately unpopulated pending fixture approval.

| Fixture element | Proposed value or binding |
| --- | --- |
| Organisation / repair / resident | SYN-ORG / SYN-REPAIR-01 / SYN-RESIDENT-01 |
| Promise | Evidence record E-PROMISE-01, resident communication evidenced; date/time value supplied by reviewed fixture |
| Observation | After the fixture-defined promise boundary, with required evidence current under the fixture source profile |
| Contractor assertion | E-COMPLETE-01 claims completion |
| Resident assertion | E-DISPUTE-01 says the problem remains; preserved alongside contractor assertion |
| Human roles | SYN-CASE-OWNER and SYN-REPAIRS-TEAM, plus named authorised accepting actor and tracking/fallback role |
| Permissions/data use | Explicit synthetic approved instrument references; assertions here are not live grants |
| Channel agreement | Synthetic agreement record identifying the resident-agreed channel(s), selection/combination rule and current revision; no live contact |
| Timing/recovery | Explicit fixture settings required before execution; no implicit deadline or retry default |

Planned trace:
1. Admit both completion accounts with provenance; mark dispute without deleting either.
2. Evaluate the overdue trigger using the resident promise and approved fixture comparison. If completion cannot be established, preserve that limitation rather than falsely assert a known incomplete fact.
3. Produce bounded authority/data-use determinations for internal escalation and factual contact.
4. At each relevant effect boundary, validate current controls and record the attempt.
5. Dispatch escalation; delivery evidence leaves human acceptance pending.
6. Record named human acknowledgement and valid owner/team contact provision.
7. If contact effect is unknown, reconcile before repeat; if acknowledgement is overdue, use the approved fallback and keep the case unresolved.
8. An authorised human resolves the dispute or records an explicitly unresolved disposition. No automatic new promise, spending or contested closure occurs.

## 11. Proposed obligations and component allocation

OP-R01–18 are local drafting identifiers, not approved component REQ IDs. All have origin v0.1, 5 October 2026; status **proposed**; release scope **operational profile drafting, bounded implementation unapproved**. Mark is the project baseline approver; operational instruments require the applicable organisational authority. Accountable role appointments remain open. Exact component REQ/VER allocation and source-matrix updates follow this draft.

| ID | Proposed obligation | Derivation / rationale | Responsible component and blocker | Planned case |
| --- | --- | --- | --- | --- |
| OP-R01 | A dependent capability shall require an active compatible profile with all its required settings supplied and approved. | §2–3; DEC-035; prevent placeholder authority | 01/02/03/04/05; activation/configuration | OP-V01 |
| OP-R02 | Conflicting completion assertions shall be preserved as distinct evidence. | §4; DEC-031; preserve contestability | 02/10/13; source profile | OP-V02 |
| OP-R03 | An unresolved completion dispute shall prevent automatic repair-case closure. | §4–6; DEC-031/032 | 13/30; resolution powers | OP-V02 |
| OP-R04 | Pending work materially dependent on corrected evidence shall be reassessed before continuation. | §4; DEC-029; selective reassessment | 02/04/13; dependency map | OP-V03 |
| OP-R05 | Automatic escalation or factual resident notification shall require permission for its exact scope. | §5; DEC-032; bounded delegation | 01/03/04/11/13/14; schedule/channel | OP-V04 |
| OP-R06 | New completion promises, expenditure commitments and contested closure shall require an authorised human decision. | §5; DEC-032; reserved demonstration actions | 01/13/30; decision powers | OP-V04 |
| OP-R07 | The originating workflow shall track a handoff until an authorised named human acknowledges responsibility. | §6; DEC-033; delivery is not acceptance | 13/30; receiver/tracking roles | OP-V05 |
| OP-R08 | An unacknowledged handoff shall follow the configured authorised non-response route while retaining unresolved status. | §6; DEC-034; no false completion | 13/30; deadline/cover/fallback | OP-V06 |
| OP-R09 | Unavailable essential controls shall withhold dependent effects without granting additional powers. | §7; DEC-003/028/034 | 01/03/04/05; dependency/boundary | OP-V07 |
| OP-R10 | A consequential repeat shall require authorised effect reconciliation and permitted continuation. | §8; DEC-030; no blind replay | 04/05/13/14; recovery profile | OP-V08 |
| OP-R11 | Demonstration processing shall remain within the repair-status, accountability-routing and resident-communication purposes. | §9; DEC-035; purpose limitation | 03/11/13; use/retention profiles | OP-V09 |
| OP-R12 | Synthetic profile values shall be distinguishable from operational organisation configuration. | §2/10; DEC-035; no fixture defaults | 02/05/40; isolated fixture environment | OP-V10 |
| OP-R13 | The overdue comparison shall follow the promise’s calendar-date or precise-time meaning in the approved timezone without automatic grace. | §4–6; DEC-036 | 02/10/13; calendar/source mapping | OP-V11 |
| OP-R14 | A revised resident promise shall preserve original promise/breach evidence and require authorised decision and resident communication evidence. | §4–6; DEC-037 | 01/02/11/13/30; amendment evidence | OP-V12 |
| OP-R15 | Completion shall require the approved repair-specific evidence rule and shall not be established by resident silence or a job-closed flag alone. | §4–6; DEC-038 | 02/10/13; evidence sufficiency | OP-V13 |
| OP-R16 | Unknown completion after the promised boundary shall trigger a verification escalation that preserves uncertainty. | §4–6; DEC-039 | 13/30/11; verification route | OP-V14 |
| OP-R17 | Partial completion shall preserve outstanding promised scope and shall not erase the original commitment through job splitting. | §4–6; DEC-040 | 02/10/13/30; scope authority | OP-V15 |
| OP-R18 | Resident communication shall use applicable resident-agreed channel(s) with agreement and selected-channel evidence bound to the action. | §4–6; DEC-041 | 02/03/11/13/14; agreement profile | OP-V16 |

## 12. Planned acceptance cases

All OP-V01–16 are **planned, not executed**. Shared preconditions: fixed source/specification/profile manifest; authorised isolated synthetic environment; approved fixture settings and test identities; no live side effects. Missing prerequisites yield not assessed, not pass. Inspect complete in-scope cases, not an undisclosed sample. AOS-40 will supply executable procedures and test ownership.

| Case | Input / challenge | Expected behaviour and evidence |
| --- | --- | --- |
| OP-V01 | Missing deadline, inactive permission profile or incompatible revision | Dependent capability unavailable; explicit missing/incompatible setting; unrelated permitted functions preserved |
| OP-V02 | Contractor completion and resident disagreement; attempt auto-closure | Both source revisions retained; disputed state; auto-closure withheld; accountable resolution route |
| OP-V03 | Correct a material promise fact with affected and unrelated pending actions | Affected actions reassessed; unrelated authorised actions continue; completed history preserved and significant consequences reviewed |
| OP-V04 | Permitted factual notice; then proposed new date, expenditure or contested closure without human decision | Exact scoped notice permitted only after controls; reserved actions withheld; later valid human decision checked for scope |
| OP-V05 | Delivery confirmed without human acknowledgement; then authorised acceptance | Transfer remains pending after delivery; tracking retained; named scope-bound acceptance evidenced |
| OP-V06 | Acknowledgement deadline passes; receiving actor unavailable | Authorised cover/fallback invoked and tracked; unresolved state persists; no invented recipient or success |
| OP-V07 | Revoke permission or lose essential control immediately before effect | Dependent effect withheld where enforceable; approved race handling and recorded limitations for effects already irreversible |
| OP-V08 | Contact dispatch may have occurred; timeout/restart/repeat requested | Indeterminate outcome persists; permitted status query/reconciliation; no blind replay; human handoff if safe permitted continuation unestablished |
| OP-V09 | Attempt extra resident inference or excessive disclosure/logging | Out-of-purpose processing/disclosure withheld; permitted restricted projection and evidence of decision; retention/deletion behaviour assessed only with approved policy |
| OP-V10 | Attempt to use synthetic role/permission or timing as live configuration | Fixture separated and rejected for live authority; production commissioning gaps visible |
| OP-V11 | Date-only and precise-time promises; attempt to add hidden grace | Evaluate each at its approved boundary; no inferred precision or automatic grace; timezone/clock evidence retained |
| OP-V12 | Internal reschedule; authorised revised promise after breach | Internal target cannot reset promise; authorised amendment records communication on resident-agreed channel(s); original breach and escalation preserved |
| OP-V13 | Job-closed flag alone; resident silence; sufficient approved evidence | First two cannot establish completion; sufficient evidence assessed against repair-specific rule; dispute remains routed if present |
| OP-V14 | Promise boundary passed with completion unknown | Verification escalation and notification preserve uncertainty and appropriate contacts; no assertion of definite incompletion |
| OP-V15 | Some promised work outstanding; split job/redefine scope | Original incomplete commitment remains visible; completed/outstanding parts retained; scope/new promise requires authorised human review and communication |
| OP-V16 | Agreed channel, unagreed substitute, withdrawn agreement, alternative/combined channel sets and outage | Current agreement and selected channels checked; unagreed substitute withheld; permitted agreed alternative follows profile; unresolved contact/human route for unavailable agreement/channels; no false delivery completion |

## 13. Remaining decisions, author review and next step

Approved direction resolves the five questions, not the detailed profiles. Residual prerequisites are:
- Appointed profile/semantic owners and change/compatibility procedure.
- Authoritative source mappings, comparison rules, evidence sufficiency and dispute-resolution powers.
- Approved organisation action schedule, processing/access/retention/location rules and current-control implementation.
- Actual human appointments, deadline/cover/fallback settings, resident channels and valid contacts.
- Approved action-specific reconciliation limits, recording boundary and threat model.
- Explanation/analytical review detail, exact component records, complete source traceability and acceptance procedures.

Author checks cover local identifier uniqueness, obligation-to-case linkage, Markdown structure, preservation of approved boundaries and explicit unresolved parameters. No implementation test, independent review, operational validation or readiness gate is claimed. This is an annex, not completion of the affected component specifications.

**Next:** Review AOS-01 v0.1 general authority semantics and its contrasting scenario cases, then co-draft AOS-02 and AOS-03 against the common contracts. Specifications derive from governing principles/architecture and are subsequently tested against processes; repair-specific rules remain in their relevant profiles. Shared schema adoption, exact source-matrix links, organisational instruments/settings and readiness remain open. Item 6 continues; item 5b research-pilot verification remains open in parallel.

**Approval disposition, 5 October:** Mark approved all five date/evidence recommendations and additionally required resident-agreed communication channel(s), recorded under DEC-036–041. Direction is approved; exact OP-R wording remains proposed and OP-V cases remain planned. Resident agreement and delivery/receipt are distinct evidence. Component adoption, source-matrix update and operational commissioning remain open.

**Scope and drafting-method clarification, 5 October:** Mark confirmed that general specifications are derived from governing principles/architecture and then tested against business processes. Repair-specific completion/promise/action rules remain scoped to the demonstration/profile. AOS-01 v0.1 now supplies the proposed general authority model and contrasting tests; it does not extrapolate a universal requirement for per-action human approval of all expenditure or promises from the repair example. Organisation-specific settings and profile adoption remain open.

