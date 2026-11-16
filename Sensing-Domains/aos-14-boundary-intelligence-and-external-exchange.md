# AOS-14 — Boundary Intelligence and External Exchange

Document: aos-14-boundary-intelligence-and-external-exchange · Source revision or record: v0.9

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**DEC-103 adopted — 29 October 2026:** Current revision 0.9. Decision validity/effective time, attributable evidence/authentication, minutes approval and permission to execute are separate. DEC-087 is partly superseded; [decision/amendment and legal-source record](../Supporting-Specifications/aos-dec-103-decision-validity-evidence-and-minutes-2026-10-29.md). No universal later-minutes or second decision-record approval gate. Exact instruments/evidence policy, KX-06 v0.3 compatibility and ordinary separate review/readiness gates remain required; cases unexecuted. Earlier contrary wording is historical only where explicitly identified.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

| Document control | Current entry |
| --- | --- |
| Identifier / date / applicable quality standard | AOS-14 / 9 October 2026 / AOS-QS v0.1 |
| Project owner / author | Mark Sweeny / Codex at Mark's request |
| Accountable organisational Boundary owner / independent reviewer | Not yet appointed / not assigned |
| Approver / approval record | Mark for project drafting decisions; organisational approving authority must be appointed for affected instruments / no build or operating approval |
| Release scope / gate | Proposed logical functional draft; G1 organised; G2 review submission, not independently determined; G3/G4 not achieved |
| Source baseline | FP v4; RP v6; Governance Intelligence Tests; preserved AOS-00 Source Manifest; AOS-00 DEC-005/018/086 and current common/component versions above |
| Review/change evidence | §§19–21 and Appendix A; author document checks only; source legal applicability not newly researched |

**Historical supplier perspective — 8 October 2026:** AOS-14 v0.5 adds supplier participation, capability/contract mappings, a worked exchange-to-outcome example, exact requirement response rows and proposed REQ-009/planned VER-007 for supplier allocation. Architecture/Map v0.39; DEC-001–091 unchanged; 01–05 v0.8,10 v0.3,11 v0.2,12 v0.2,13 v0.1 and40 v0.5. Shared v0.15/Core v0.6/Register v0.14; Control Coordination v0.2/Protected Reporting and Recovery v0.1/Operational Profiles v0.1; source manifest and quality/template baselines unchanged. Earlier dated baselines are historical. Nine numbered proposed requirements/seven planned cases cover research and supplier adoption only; older Boundary functions/invariants/conformance criteria remain separately identified, with full requirement/source migration still open. No case execution, whole-document approval, build readiness, operating activation or closure of existing design issues is claimed.

**Current AOS-30 alignment — 7 October 2026:** functional drafting and consistency alignment complete under Mark’s instruction. AOS-00/Map v0.25, DEC-001–089; AOS-01–05 v0.8, AOS-14 v0.4, AOS-20 v0.3 and AOS-30 v0.3; Shared v0.9/Core v0.6/Exchange Register v0.8; source matrix v0.9 and template v0.4 unchanged; Control Coordination v0.2/Protected Reporting and Recovery v0.1 unchanged. Earlier dated baseline/adoption/next-step entries are history. CR30-01–03 are closed at the functional-document level; implementation/commissioning evidence remains separate. No new DEC/REQ/VER/IF identifier or operating power is introduced.

**Specification version:** 0.9  
**Status:** Working draft — not approved for build  
**Architecture baseline:** AOS-00 v0.42, DEC-001–096; 9 October 2026  
**Specification Map:** v0.42, 9 October 2026  
**Issues baseline:** Architecture Issues Register, 29 September 2026  
**Research charter:** AOS-14 Boundary Intelligence Research Agent, updated 6 October 2026; pilot operation remains unverified  
**Accountable human owner:** TBD  
**Research custodian:** AOS-14 Boundary Intelligence Research Custodian  
**Approver / approval record:** Not yet approved  
**Change history:** v0.7 adopts approved DEC092–096 into existing requirement/case records and resolves general ISS003–007 direction; Q1 distinguishes financial/resource impacts;  v0.6 full proposed requirement/case/source migration and typed logical mappings; new REQ-010–055/VER-008–034; existing IDs preserved, issue dispositions reconciled;  v0.5 supplier perspective and proposed REQ-009/planned VER-007, preserving prior IDs and status; v0.4 AOS-30 decision-status disclosure alignment; v0.3 common external-research adoption;  v0.1 initial template trial; v0.2 restructured using AOS Standard Component Specification Template v0.2 and adds explicit State Model.

# 1. Purpose and Scope
## 1.1 Purpose
AOS-14 governs the organisation's intelligent interaction across its external boundary. It ensures that information, instructions, commitments and other consequential exchanges entering or leaving the organisation do so under legitimate authority, for an intelligible purpose, subject to applicable obligations, and with sufficient evidence to remain accountable.

## 1.2 Architectural problem
External connectivity creates distinctive uncertainty concerning identity, provenance, authority, purpose, permitted disclosure, external obligations, execution and actual external effect. Technical connectivity alone cannot establish organisational legitimacy.

## 1.3 Intended outcome
For a consequential external exchange, the organisation can establish and subsequently reconstruct **what crossed the boundary, with whom, for what purpose, under what authority, subject to what obligations, and with what known outcome.**

## 1.4 Scope
AOS-14 owns inbound and outbound external exchange; authorised external retrieval; external commitments and contact controls; external source/destination context; exchange obligations; boundary-specific provenance; federated exchange semantics; boundary-pattern sensing; and monitoring for excessive openness or restriction.

## 1.5 Exclusions
AOS-14 does not own constitutional authority (AOS-01); common data semantics and records (AOS-02); organisation-wide identity/access/consent/permitted processing (AOS-03); general agent lifecycle (AOS-04); runtime containment/security/recovery (AOS-05); internal workflow coordination (AOS-13); governance interpretation (AOS-20–25); human Mode 2 judgement; or independent conformance (AOS-40). It applies shared controls to external exchange but does not acquire ownership of them.

# 2. Authority and Sources
The controlling allocation is AOS-00 DEC-005: Governance Intelligence interprets evidence and prepares propositions; Boundary Intelligence governs exchanges across the organisation's external boundary; AOS-01/03/05 shared controls with the AOS-04 agent contract enforce permissions and prohibitions system-wide; authorised humans adjudicate Mode 2 questions.

The source hierarchy is Foundational Principles v4 and Reasoning Principles v6; approved AOS-00 decisions; explanatory architecture in the four Holding the Line books; existing specifications/working notes as proposals requiring reconciliation; and research evidence as challenge/design input. The AOS-14 Research Charter is non-normative and cannot amend this specification.

# 3. Responsibilities

**Responsibility cross-reference (DEC-094; editorial clarification, 29 October 2026):** AOS-14 recognises an exchange-associated obligation and its source/context; the relevant domain steward determines substantive meaning/applicability. AOS-02 owns the common obligation-record semantics and structure/custody. AOS-13 tracks routing, accepted responsibility, fulfilment and unresolved duties. AOS-30 owns the human-workflow meaning of accepted responsibility and supports empowered human disposition/account. These are distinct responsibilities: recognition, record ownership and dispatch do not constitute human acceptance. The existing tracking owner retains the duty until explicit scoped transfer is accepted; failed delivery or exhausted cover does not create an ownerless success. Actual people, cover and response powers remain organisation-appointed prerequisites. No semantic ownership is transferred by this clarification.
AOS-14 recognises governed external exchange; establishes external actor/system/domain/destination; applies external-exchange controls using authoritative shared determinations; assesses inbound admissibility and outbound disclosure; validates authority for external commitments; identifies exchange obligations; preserves boundary provenance; represents uncertainty; supports outcome reconciliation; senses cumulative patterns; supports federated exchange; and escalates exchanges that cannot legitimately proceed autonomously. Its own actions remain subject to shared controls.

### 3.1 Component-owned external research

Under DEC-086, AOS-14 owns the relevance and substantive implications of external research into its own function/specification, inheriting AOS-04 v0.8 §§3.1/5.1/6.6/10.8 (CON-009), AOS-02 v0.8 §6.6 (CON-007) and AOS-01 v0.8 §§6.6/10.8. Shared agents/collection infrastructure may serve distinct profiles; Boundary does not become the substantive research owner for every component. Internal operational monitoring and GI organisational sensing remain separate. Research observes, analyses, challenges and proposes; it cannot amend specifications, expand tools/powers, approve deployment or reopen DEC-018.

| Controlled profile allocation | Component-specific meaning / owner and gate |
| --- | --- |
| Remit/questions/baseline | Does external evidence expose incomplete, incorrect, ambiguous or insufficiently resilient functions, or meaningful improvement? Topics: external exchange, source verification, partner protocols/data-sharing, federation, identity/provenance and delegated external authority, commitments/obligations, dynamic boundaries and boundary-relevant containment incidents. Bind exact assessed specification/dependency revisions, including their draft/approval status. |
| Jurisdiction/status/sources | Prefer official regulator/government/standards texts, partner protocol specifications, primary research and authoritative incident accounts. Applicable jurisdictions, exact source list/admission/currentness criteria and licensing are owned profile settings; distinguish proposals, publication, enactment/adoption and effective dates. Verification is not organisational adoption or professional legal judgement. |
| Assignment/cadence/triggers | Boundary component owner/research custodian with affected shared-control and receiving-domain owners owns remit/review. Assigned agent/service, approved cadence/event triggers, coverage periods and accountable tracker/cover appointments remain commissioning dependencies; no default schedule or separate deployment is mandated. |
| Authority/use/retrieval | Applicable 01/03 permissions and 05 controls govern task/tools/data/locations; 14 governs external retrieval/admission and source verification. Public accessibility is not unrestricted reuse/disclosure; hostile source content is data, never an instruction. |
| Evidence/assessment | Common 02 profile/run/finding/disposition views bind exact sources/assurance, publication/event/access/effective dates or explicit unknown reasons; evidence versus inference; affected CAP/FUN/REQ/CON/decision/source, alternatives, uncertainty, materiality/urgency and cross-component owners. |
| Coverage/quality | Report actual complete/partial/failed/cancelled/not-performed coverage and bounded no-material-finding. Component reviewers with 04/40 approve relevance, evidence-fidelity, false/missed-finding and limitation rubrics before dependent reliance; deterministic enforcement is assessed separately. |
| Review/change | Named permitted recipient/tracker, deadline/cover/escalation and empowered disposition use 13/30 and 01. Acceptance for further work, amendment approval, verification, applied release and outcome closure remain distinct. Live urgent implications use separately authorised response; research supplies no emergency power. |
| Setup gate | Component owner owns missing profile values; 01 powers, 03 use, 05 enforcement, 14 access, 02 schemas and 04/40 evaluation owners supply their evidence. Missing mandatory values withhold dependent activation/reliance and retain an owned coverage exception. Author drafting does not establish operating readiness. |

### 3.2 Supplier participation and architectural fit

Existing technology and software can realise Boundary functions. Relevant offerings include integration platforms, API/event gateways, external data/research services, partner portals, communication services, identity/provenance services and sensor/IoT connectivity. Their existing analytics, workflows and user interfaces may also realise functions in other AOS components. Logical responsibility does not prescribe a separate product, central gateway or replacement of capable supplier software.

| Supplier capability | AOS-14 contribution | Authoritative counterpart / evidence needed |
| --- | --- | --- |
| API, event or file integration; managed connectors | CAP-001–003/FUN-001–003; CON-001/002 | Recognise direction, exact actor/destination and purpose; consume 01/03 determinations and05 enforcement; unsupported identity, meaning or permission remains explicit. A working connection is not an authority grant. |
| External action, partner portal or communication service | CAP-004/FUN-004; CON-001–003 | Exact commitment/message/action and current permission;04 task/effect meaning,05 final checks,13 duty coordination,11 resident channel agreement where applicable. Supplier dispatch or acceptance is not actual service completion. |
| Contract/data-sharing and exchange-obligation support | CAP-005/FUN-005; CON-004 | Preserve approved confidentiality, use, onward-disclosure, retention, reporting and incident obligations with appointed owners;01/02/03/domain meanings and ISS-006 remain authoritative. |
| Exchange receipts, reconciliation and audit tools | CAP-006/FUN-006/007; CON-003 |02 custody and common source/effect standing;04/05 execution evidence,13 reconciliation/human tracking. Keep dispatched, rejected, partial, duplicate and indeterminate outcomes distinct under the approved exchange profile; ISS-005 is not resolved by a product label. |
| Federated identity, partner protocols and provenance | CAP-007/FUN-008; CON-001–004 | Exact agreed counterparty semantics, permitted scope and incident responsibilities;03 identity/use and01 authority. Partner systems need not use AOS internally; ISS-001/007 remain gates. |
| Boundary analytics and operational dashboards | CAP-008/FUN-009; CON-003/004 | Show permitted cumulative exchange/exposure and excessive-restriction patterns, population/coverage/uncertainty and accountable follow-up;25 owns governance oversight. Analytics do not gain unrestricted data access or new powers. |
| External research feeds, retrieval and verification tools | CAP-009/FUN-010; CON-005; REQ-001–008 | Governed retrieval and exact source/status/licensing/coverage evidence; each component owns its specialist interpretation;02 records,04 agent contract,13/30 accepted review and01 amendment remain distinct. |
| Sensor/IoT hardware, edge bridges and cloud platforms | CAP-001–003/006 for governed external exchanges; may also realise10 asset sensing | Preserve device/source identity, physical observation provenance, uncertainty, permitted use and communication failure.10 owns condition/completion meaning;05 runtime security,03 access/use. Connection or supplier analytics is not verified physical condition by itself. |

### 3.3 Deployment arrangements and ownership

**Standalone or manual assistance:** a supplier may produce evidence, analytical findings or an exchange proposal for a permitted human-mediated route. Declare the unautomated steps and actual handoff/evidence arrangements; a manual arrangement cannot claim demonstrated automated enforcement.

**Integrated arrangement:** a supplier connects through declared APIs, events, files or other approved contracts. Exact schema/profile/source revisions, actor and destination identity, permissions, staged acknowledgements and observed effects must remain attributable at both ends.

**Combined platform:** one supplier may realise Boundary exchange plus Asset/Resident/People/Process functions or shared-control services. Declare each logical responsibility, authoritative record and actual control location. Product-internal calls retain the same purpose, authority, human judgement and evidence duties. Conversely, several suppliers may contribute to one Boundary function; name the party responsible for each mapping, reconciliation and unresolved duty.

Hosting, network location or an existing commercial contract alone does not determine the organisational boundary. The approved organisation/exchange profile must describe supplier/agent control, identity, purpose and permitted scope. ISS-007 remains open for the general mixed-control definition. No deployment arrangement settles that issue by implication. A firewall/gateway can contribute to05 enforcement and14 exchange handling; it does not own constitutional authority or certify permissible data use.

Functional fit identifies candidate contributions. Executable integration additionally requires agreed API/schema/security/time/service/lifecycle profiles and actual producer/consumer mapping. Tested conformance requires scoped observed evidence against the requirements and criteria. These are separate claims; an API catalogue, dashboard or supplier assurance statement does not establish all three.

### 3.4 Approved exchange principles — 9 October 2026


## Approved Boundary decision adoption — 9 October 2026

| Approved decision / subject | Direction / rationale | Affected Boundary records | Approval and standing |
| --- | --- | --- | --- | --- |
| AOS-00-DEC-092 — Consequential external exchange | An external exchange is consequential when it can create or change an organisational commitment, disclose protected information, affect rights or service, trigger external action, or create a material obligation or risk. Materiality considers financial exposure and resource impact separately: payments, expenditure, liabilities or contingent exposure; and staff time, workload, capacity, equipment, facilities or other resource commitments and displacement of existing duties. Low monetary cost does not establish low resource impact. Record known quantities with their units/time basis and uncertainty; no invented money-to-time conversion or universal threshold. Apply organisation-approved criteria, including cumulative commitments. Routine public-information retrieval may use a lighter approved route only where its actual purpose, content and effects meet that profile. Uncertain classification goes to an accountable reviewer and cannot silently use the lighter route. | ISS-004; REQ-010–012/020–022/027/051; VER-008/012/016 | Mark;9October2026; Q1 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-093 — Outcome-specific exchange evidence | Define the required outcome and sufficient evidence for each exchange type. Sending, delivery, recipient acceptance and actual fulfilment remain distinct facts. Contractor receipt does not prove completed work. Where the required effect remains unknown, retain that standing and reconcile before retrying. An authorised person may close further investigation under the approved profile only with an explicit unknown outcome and retained owner/status of every outstanding duty; closure cannot become confirmed success. | ISS-005; REQ-029–032/036/053; VER-018/019/021/031/034 | Mark;9October2026; Q2 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-094 — Common external-obligation ownership | Use a common obligation record carrying source, applicability, exchange, responsible human owner, deadline where applicable, fulfilment evidence and current status. Boundary recognises exchange-associated obligations; relevant domain stewards determine substantive meaning and applicability under their authority; AOS-02 owns common record semantics; AOS-13 tracks accepted responsibility and fulfilment; AOS-30 supports accountable human disposition. Preserve financial and resource impacts separately where applicable, including unknown values. Uncertain or conflicting obligations go to an empowered human; automated recognition does not create legal authority or settle substantive meaning. | ISS-006; REQ-033–036; VER-020/021 | Mark;9October2026; Q3 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-095 — Operation-specific organisational boundary | Determine the boundary from organisational authority and control over the particular operation and data use. Hosting location alone is insufficient. A supplier system may carry out a delegated internal function while its onward disclosure or independent action crosses the external boundary. Each arrangement declares controlling parties, authority, operation/data-use scope, actual governed exchange points and independent shared-control enforcement. Ambiguous or missing control allocation remains an owned gap and withholds dependent consequential action. | ISS-007; REQ-010/011/026/047; VER-008/015/027 | Mark;9October2026; Q4 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-096 — Boundary patterns and system oversight | Boundary detects cumulative external-exchange patterns, including repeated disclosures, accumulating commitments, unusual counterparties, excessive restriction and attempts to evade controls by splitting actions. AOS-25 combines permitted Boundary signals with other domains to assess wider drift and emerging/system risks. Shared AOS-01/03/04/05 controls enforce approved limits and accounting; empowered humans decide policy/limit changes. Boundary cannot create a private budget, waive restrictions or adjudicate systemwide governance. | ISS-003; REQ-027/043–046; VER-016/025/026 | Mark;9October2026; Q5 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |

These directions do not appoint organisational officers, select numerical thresholds, convert resource impact into money or certify external obligations legally. Shared owners retain their meanings and independent enforcement. Proposed component requirements and planned cases retain stable identities; an approved direction is distinct from G3/build or operating approval. The organisation-specific profile must state criteria and aggregation windows for financial and resource materiality; exchange-type expected effect/evidence and authorised unresolved closure; obligation field types/cardinalities/lifecycle and owners; operation/data-use authority and control points; and Boundary-versus25 pattern routing/triggers. Missing or invalid mandatory settings withhold dependent effects/reliance and retain an owned gap. No deferred federation activation or new source-status promotion is implied.

# 4. Capabilities and Functions
## AOS-14-CAP-001 — External Exchange Recognition
**AOS-14-FUN-001 — Classify External Exchange:** determine whether an exchange crosses the governed external boundary; direction; counterparty/domain; type; purpose; consequentiality where defined; and applicable contract. Boundary ambiguity remains explicit.

## AOS-14-CAP-002 — Inbound Admissibility
**AOS-14-FUN-002 — Assess Inbound Admissibility:** consume identity, provenance, permitted-use, authority, security, currency and receiving-domain evidence. Return **admit / admit with conditions / quarantine / reject / escalate / unresolved**. Admission does not establish substantive truth.

## AOS-14-CAP-003 — Outbound Disclosure Control
**AOS-14-FUN-003 — Assess Outbound Disclosure:** assess recipient, purpose, authority, permitted use, disclosure restrictions, obligations and context. Return **permit / constrain / deny / escalate / unresolved**.

## AOS-14-CAP-004 — External Commitment Control
**AOS-14-FUN-004 — Validate External Commitment:** obtain the applicable authority determination from shared controls. Where authority is denied, unresolved, unavailable, expired or revoked, dependent execution must not proceed. AOS-14 cannot manufacture substitute authority.

## AOS-14-CAP-005 — External Obligation Recognition
**AOS-14-FUN-005 — Identify Exchange Obligations:** identify use restrictions, confidentiality, retention/deletion, notification/reporting, reciprocity, acknowledgement, expiry, review and other consequential obligations; pass them through governed contracts to responsible owners.

## AOS-14-CAP-006 — External Provenance and Outcome Evidence
**AOS-14-FUN-006 — Record External Exchange Evidence:** record required exchange evidence using AOS-02 semantics.  
**AOS-14-FUN-007 — Reconcile External Outcome:** where authorised dispatch does not establish actual effect, preserve outcome as **confirmed / rejected / failed / partial / duplicate / indeterminate / other defined state**. Status: proposed clarification; see ISS-005.

## AOS-14-CAP-007 — Federated Exchange
**AOS-14-FUN-008 — Apply Federated Exchange Contract:** apply agreed semantics for identity, authority, provenance, obligations, exchange status and incident duties without assuming the external organisation uses AOS internally.

## AOS-14-CAP-008 — Boundary Pattern Sensing
**AOS-14-FUN-009 — Sense Boundary Patterns:** support detection of repeated disclosures/commitments, unusual destinations, cumulative authority use, changing exchange volumes/types, repeated indeterminate outcomes, systematic excessive restriction and changing external capability/exposure; route material findings to appropriate oversight.

## AOS-14-CAP-009 — Component external research and shared retrieval

**AOS-14-FUN-010:** research Boundary adequacy under its approved remit and provide governed retrieval/source-verification evidence for other assigned component profiles without acquiring their substantive ownership.

### 4.4 External-research adoption requirements

New AOS-14-REQ-001–008 originate in v0.3, 6 October 2026; proposed logical component wording, accountable semantic/component owner per §3.1, project approver Mark, organisational instruments/appointments open. No prior REQ is retired or promoted.

| REQ | Proposed independently verifiable obligation | Derivation / function / contract | Planned VER |
| --- | --- | --- | --- |
| 001 | The component shall bind its external-research task to a controlled component-specific profile inheriting AOS-04-CON-009 and the exact assessed baseline/status. | DEC-086; AOS-14-CAP-009/FUN-010/CON-005; common 04/02/01 inheritance | 001 |
| 002 | Research retrieval, processing and disclosure shall use AOS-14-governed access with current applicable AOS-01/03 determinations and independently enforced AOS-05 controls. | DEC-086; AOS-14-CAP-009/FUN-010/CON-005; common 04/02/01 inheritance | 002 |
| 003 | The component shall produce and consume AOS-02 §6.6 profile/run/finding/disposition views with linked evidence, assurance, legal/standards applicability/status and explicit coverage limitations. | DEC-086; AOS-14-CAP-009/FUN-010/CON-005; common 04/02/01 inheritance | 003 |
| 004 | Shared retrieval, duplicate coalescing and source/baseline correction shall retain each affected component’s assessment, accountable review duty and recorded reassessment. | DEC-086; AOS-14-CAP-009/FUN-010/CON-005; common 04/02/01 inheritance | 004 |
| 005 | Research review shall retain an accountable handoff and empowered exact-revision disposition, with separately authorised urgent handling and no implied amendment or release approval. | DEC-086; AOS-14-CAP-009/FUN-010/CON-005; common 04/02/01 inheritance | 005 |
| 006 | Dependent research reliance shall require accepted component relevance/evidence-fidelity and false/missed-finding evaluation criteria, assessed separately from deterministic control enforcement. | DEC-086; AOS-14-CAP-009/FUN-010/CON-005; common 04/02/01 inheritance | 006 |
| 007 | Missing mandatory profile settings, denied access, failed coverage or delivery shall remain owned exceptions rather than favourable coverage, substituted permissions or completed review. | DEC-086; AOS-14-CAP-009/FUN-010/CON-005; common 04/02/01 inheritance | 001 |
| 008 | Boundary shall supply external retrieval/admission/source-verification evidence to assigned component profiles without deciding their substantive findings or assuming systemwide enforcement ownership. | DEC-086; AOS-14-CAP-009/FUN-010/CON-005; common 04/02/01 inheritance | 004 |

### 4.5 Supplier allocation requirement

| REQ | Proposed independently verifiable obligation | Derivation / function / contract | Planned VER |
| --- | --- | --- | --- |
| 009 | Each supplier implementation scope shall maintain an exact versioned capability-to-AOS requirement/function/contract allocation, with authoritative ownership, scoped conformance evidence or an owned gap/dependency and resolution gate for each applicable obligation. | Mark's 8 October supplier direction; CAP-001–009/FUN-001–010/CON-001–005;01–05 shared ownership; QS-11/12/21/26 | 007 |

REQ-009 governs implementation allocation; it creates no exchange authority, product certification or new shared schema. Existing REQ-001–008 and all prior functions, invariants and criteria are retained; issue statuses now reflect the9October approved dispositions.

### 4.6 Complete proposed requirement records

The following attributes apply unambiguously to every REQ-001–055, including the unchanged statements in §§4.4–4.5. **Level:** component requirement, except REQ-003/015/017/028/033/035/050/053 (interface requirement) and047 (design constraint). **Category:** research001–008; supplier009/054; authority020–027/047/055; privacy018/019/038–042; evidence013–017/028–036/050–053; sensing/quality037/043–049; exchange010–012. **Owner:** accountable Boundary component owner (appointment unresolved), with01/02/03/04/05/domain owners retaining their semantics. **Approver:** Mark for the proposed project baseline; organisational instrument/operating approval remains with the appointed authority. **Status/release:** proposed v0.7 logical draft; none approved for build. **Change:**001–008 retained fromv0.3;009 retained fromv0.5;010–055 introduced9October by Codex under Mark's completion instruction as explicit interpretations/engineering derivations of the original cited functions. DEC092–096, approved9October, now additionally derive the affected existing requirements; no new REQ identity is asserted. **Rationale:** prevent the specific failure named by each row's subject/obligation;001–008 prevent ungoverned specialist research,009 prevents unallocated supplier duties. **Verification:** inspection/walkthrough plus isolated implemented integration/failure injection; exact pass conditions in the linked planned VER, none executed. **Dependencies:** current01–05,02 custody and shared IF-001; exact approved exchange/source/quality/supplier profiles and compatible schema manifest; relevant issue in the row, and appointment/evidence gaps in§17. Missing dependencies withhold affected execution/reliance. Source contributions are interpretations, not verbatim source adoption; exact FP/RP/GT reverse links and residuals are in Appendix A. Each row's FUN refers to the retained§4 function, CON to§6; those locators and DEC-005 are the immediate derivation, with shared responsibilities per§2. REQ-001–008 additionally derive from DEC-086/AOS-04§6.6/AOS-02§6.6/AOS-01§10.8;009 from Mark's8October instruction/§20.

| REQ ID / subject | Proposed normative statement | Exact derivation / logical contract / unresolved dependency | Planned VER |
| --- | --- | --- | --- |
| AOS-14-REQ-010 — Declared control perimeter | AOS-14 shall bind each governed exchange to an approved versioned organisation/exchange profile defining its control perimeter, parties, purpose and permitted scope. | DEC-005; §4 FUN-001; §6 CON-001; ISS-007 | AOS-14-VER-008 |
| AOS-14-REQ-011 — Exchange recognition | AOS-14 shall classify every observed request in the declared perimeter by direction, operation, counterparty and applicable exchange contract before dependent execution. | DEC-005; §4 FUN-001; §6 CON-001; ISS-004/007 | AOS-14-VER-008/AOS-14-VER-034 |
| AOS-14-REQ-012 — Consequentiality uncertainty | AOS-14 shall withhold dependent consequential execution when required approved classification is absent, contradictory or unresolved, recording the classification gap for its named reviewer. | DEC-005; §4 FUN-001; §6 CON-001; ISS-004 | AOS-14-VER-008 |
| AOS-14-REQ-013 — External identity standing | AOS-14 shall preserve the assessed external source/destination identity and acting-principal assurance, including unresolved claims, rather than treating transport connectivity as identity proof. | DEC-005; §4 FUN-001; §6 CON-001; §17 commissioned-profile/appointment gate | AOS-14-VER-009 |
| AOS-14-REQ-014 — Source standing | AOS-14 shall preserve material source origin, observation/effective time, version, correction status and verification limitations when admitting or forwarding external content. | DEC-005; §4 FUN-002; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-009 |
| AOS-14-REQ-015 — Typed determination | AOS-14 shall issue a CON-002 determination retaining the exact request, direction, operation, relevant current control revisions and disposition meaning defined in §6.1. | DEC-005; §4 FUN-002; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-010 |
| AOS-14-REQ-016 — Constrained execution | AOS-14 shall withhold an exchange until every applicable condition in its current constrained determination is satisfied and evidenced at the effect boundary. | DEC-005; §4 FUN-003; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-010 |
| AOS-14-REQ-017 — Admission is not truth | AOS-14 shall retain boundary admission, AOS-02 evidence admission, source truth/authority standing and recipient permitted use as distinct determinations. | DEC-005; §4 FUN-002; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-010/AOS-14-VER-034 |
| AOS-14-REQ-018 — Exact disclosure scope | AOS-14 shall evaluate each outbound release against the exact approved audience, payload, purpose and AOS-03 permitted-use determination before release. | DEC-005; §4 FUN-003; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-011 |
| AOS-14-REQ-019 — Recipient channel | AOS-14 shall use the current approved recipient/channel agreement for resident or other governed communications, recording delivery failure as an owned duty rather than substituting an unapproved channel. | DEC-005; §4 FUN-003; §6 CON-001; §17 commissioned-profile/appointment gate | AOS-14-VER-011/AOS-14-VER-034 |
| AOS-14-REQ-020 — Exact commitment authority | AOS-14 shall require current AOS-01 authority for the exact external commitment or unsolicited contact; a model proposal, prior relationship or technical capability shall not supply that authority. | DEC-005; §4 FUN-004; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-012/AOS-14-VER-034 |
| AOS-14-REQ-021 — No permissive fallback | AOS-14 shall withhold dependent effects when required authority or permitted-use determination is denied, unresolved, unavailable, expired or revoked. | DEC-005; §4 FUN-004; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-012 |
| AOS-14-REQ-022 — Final current check | AOS-14 shall require evidenced current applicable checks at the enforceable boundary before each consequential attempt, including previously authorised queued attempts. | DEC-005; §4 FUN-004; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-012 |
| AOS-14-REQ-023 — Untrusted instructions | AOS-14 shall treat instructions embedded in external material as untrusted content rather than authority to alter tools, purpose, profile or permissions. | DEC-005; §4 FUN-002; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-013 |
| AOS-14-REQ-024 — Selective change reassessment | AOS-14 shall reassess affected pending exchanges when a material authority, use, recipient, source or profile change arrives before execution. | DEC-005; §4 FUN-004; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-014 |
| AOS-14-REQ-025 — Late control events | AOS-14 shall resolve late or out-of-order control events against authoritative current revision/standing before permitting a dependent effect. | DEC-005; §4 FUN-004; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-014 |
| AOS-14-REQ-026 — Bypass resistance | AOS-14 shall subject alternative routes and combined-product internal flows that cross the declared boundary to the same applicable exchange controls. | DEC-005; §4 FUN-001; §6 CON-001; §17 commissioned-profile/appointment gate | AOS-14-VER-015 |
| AOS-14-REQ-027 — Shared cumulative account | AOS-14 shall consume the shared current cumulative account/reservation determination for governed actions rather than splitting exchanges or creating a private permissive budget. | DEC-005; §4 FUN-004; §6 CON-002; ISS-003 | AOS-14-VER-016 |
| AOS-14-REQ-028 — Attempt identity | AOS-14 shall preserve stable request and distinct attempt/event identities with declared duplicate/ordering treatment so repeated delivery cannot silently become a second authorised effect. | DEC-005; §4 FUN-006; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-017 |
| AOS-14-REQ-029 — Outcome evidence scope | AOS-14 shall assign an outcome class only against the exact approved exchange profile defining the effect, observation evidence and sufficiency rule for that class. | DEC-005; §4 FUN-007; §6 CON-003; ISS-005 | AOS-14-VER-018/AOS-14-VER-034 |
| AOS-14-REQ-030 — Unknown actual effect | AOS-14 shall retain partial, disputed or indeterminate effect standing and residual duties when evidence does not establish the profile-defined successful outcome. | DEC-005; §4 FUN-007; §6 CON-003; ISS-005 | AOS-14-VER-018/AOS-14-VER-034 |
| AOS-14-REQ-031 — Retry after reconciliation | AOS-14 shall require authorised reconciliation of an uncertain prior effect before any repetition, with fresh checks for the new attempt. | DEC-005; §4 FUN-007; §6 CON-003; ISS-005 | AOS-14-VER-019 |
| AOS-14-REQ-032 — Separate compensation authority | AOS-14 shall require separate current authority for a compensating external action, preserving the original attempt and effect history. | DEC-005; §4 FUN-007; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-019 |
| AOS-14-REQ-033 — Obligation standing | AOS-14 shall preserve each recognised exchange obligation with its source, applicability, authorised basis, current status and controlling profile under the common obligation model approved by DEC-094; exact schema/lifecycle profiles remain commissioned dependencies. | DEC-005; §4 FUN-005; §6 CON-004; ISS-006 | AOS-14-VER-020 |
| AOS-14-REQ-034 — Accepted obligation owner | AOS-14 shall refer each actionable exchange obligation to a named empowered owner through a tracked acceptance route with an appointed tracker for unaccepted duties. | DEC-005; §4 FUN-005; §6 CON-004; ISS-006 | AOS-14-VER-020 |
| AOS-14-REQ-035 — Staged acknowledgement | AOS-14 shall preserve receipt, validation, application and human responsibility acceptance as distinct stages with profile-defined response windows, cover and breach escalation. | DEC-005; §4 FUN-005; §6 CON-004; §17 commissioned-profile/appointment gate | AOS-14-VER-021/AOS-14-VER-034 |
| AOS-14-REQ-036 — Closure with residual duty | AOS-14 shall record the authorised closure basis, outcome standing and owner of any residual obligation without converting administrative closure into confirmed external success. | DEC-005; §4 FUN-007; §6 CON-003; ISS-005/006 | AOS-14-VER-021/AOS-14-VER-034 |
| AOS-14-REQ-037 — Internal referral distinction | AOS-14 shall distinguish independently permitted internal referral to a reviewer from external unsolicited contact or commitment requiring its separate authority. | DEC-005; §4 FUN-009; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-022/AOS-14-VER-034 |
| AOS-14-REQ-038 — Protected reporting route | AOS-14 shall preserve the common required-audience and permitted alternative reporting route when an instruction attempts suppression or the ordinary recipient is implicated. | DEC-005; §4 FUN-009; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-022 |
| AOS-14-REQ-039 — Purpose-limited exchange | AOS-14 shall enforce the AOS-03 authorised processing/disclosure purpose for raw and derived boundary data, including exclusion of unapproved behavioural inference. | DEC-005; §4 FUN-003; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-023 |
| AOS-14-REQ-040 — Data lifecycle propagation | AOS-14 shall apply current shared correction, restriction, retention, deletion and licensing treatment to affected raw/derived exchange and research records and queued uses. | DEC-005; §4 FUN-006; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-023 |
| AOS-14-REQ-041 — Restore current standing | AOS-14 shall reconcile current controls, data-lifecycle changes and prior effect standing before restoring a dependent exchange after interruption or recovery. | DEC-005; §4 FUN-007; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-024 |
| AOS-14-REQ-042 — Incident communication authority | AOS-14 shall use only the separately permitted minimum incident communication route during failure, recording any unavailable mandatory route as an owned incident. | DEC-005; §4 FUN-003; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-024 |
| AOS-14-REQ-043 — Intrinsic boundary risk | AOS-14 shall produce boundary-specific risk/constraint evidence with its source, uncertainty and affected exchange scope rather than deferring all risk to a separate domain. | DEC-005; §4 FUN-009; §6 CON-003; ISS-003 | AOS-14-VER-025 |
| AOS-14-REQ-044 — Declared coverage | AOS-14 shall disclose its assessed population, coverage gaps, failed/unperformed checks and limits so a quiet or incomplete feed cannot represent absence of boundary risk. | DEC-005; §4 FUN-009; §6 CON-003; ISS-003 | AOS-14-VER-025 |
| AOS-14-REQ-045 — Excessive restriction | AOS-14 shall refer evidence of excessive exchange restriction and resulting service/exclusion burden to an empowered reviewer without waiving the existing restriction. | DEC-005; §4 FUN-009; §6 CON-003; ISS-003 | AOS-14-VER-025 |
| AOS-14-REQ-046 — Oversight feedback | AOS-14 shall supply permitted boundary pattern/actual-outcome evidence to the assigned AOS-25 oversight and AOS-30 human route, retaining the accepted follow-up and received disposition. | DEC-005; §4 FUN-009; §6 CON-003; ISS-003 | AOS-14-VER-026 |
| AOS-14-REQ-047 — Federation deferred | AOS-14 shall withhold uncommissioned federated-exchange behaviour requiring the deferred OQ-012 model while permitting only separately approved bounded external exchange. | DEC-005; §4 FUN-008; §6 CON-001; ISS-001 | AOS-14-VER-027 |
| AOS-14-REQ-048 — Probabilistic quality evaluation | AOS-14 shall require human-approved scoped relevance, identity/source-fidelity and false/missed-result evaluation criteria before relying on probabilistic boundary assessment. | DEC-005; §4 FUN-009; §6 CON-003; ISS-008 | AOS-14-VER-028 |
| AOS-14-REQ-049 — Model/configuration change | AOS-14 shall reassess dependent evaluation and control evidence for a changed model, provider, supplier configuration or material exchange profile before dependent reliance. | DEC-005; §4 FUN-009; §6 CON-003; ISS-008 | AOS-14-VER-028 |
| AOS-14-REQ-050 — Common view compatibility | AOS-14 shall validate each logical contract instance against its approved compatible manifest, withholding dependent use of invalid identifiers, units, time origins, cardinalities or disposition values. | DEC-005; §4 FUN-006; §6 CON-003; ISS-008 | AOS-14-VER-029 |
| AOS-14-REQ-051 — Reconstructable audit | AOS-14 shall retain permitted evidence sufficient to reconstruct request, current determinations, conditions, attempts, actual outcome and accountable follow-up against the exact applied revisions. | DEC-005; §4 FUN-006; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-030 |
| AOS-14-REQ-052 — Meaningful explanation | AOS-14 shall provide the permitted recipient an intelligible determination basis, material uncertainty and challenge route while preserving authorised disclosure restrictions. | DEC-005; §4 FUN-002; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-030 |
| AOS-14-REQ-053 — Domain and human status fidelity | AOS-14 shall preserve authoritative domain and human decision standing when exchanging building information, service promises, completion evidence or chair/board status; delivery shall not upgrade it. | DEC-005; §4 FUN-006; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-031/AOS-14-VER-034 |
| AOS-14-REQ-054 — Supplier exit portability | AOS-14 shall support authorised export/revocation/exit under the agreed supplier profile without broadening data purpose, audience or continuing exchange authority. | DEC-005; §4 FUN-006; §6 CON-003; §17 commissioned-profile/appointment gate | AOS-14-VER-032 |
| AOS-14-REQ-055 — Governed manual continuity | AOS-14 shall preserve applicable checks, evidence and accountable residual duties in the approved manual continuity route rather than treating failure as permission to bypass them. | DEC-005; §4 FUN-004; §6 CON-002; §17 commissioned-profile/appointment gate | AOS-14-VER-033 |

### 4.7 Approved-direction interpretation of retained requirements

The statements and records in§4.6 are interpreted under§3.4/DEC092–096. REQ010/011 bind operation/data-use authority and actual organisational control rather than hosting. REQ012 includes both financial and resource materiality with the ambiguity rule. REQ029/030/036 retain the separately approved sending/delivery/acceptance/fulfilment and unresolved-closure meanings. REQ033/034 adopt the common record/ownership model; REQ043–046 adopt local Boundary sensing versus25 system oversight. All are proposed requirement wording in v0.7, with Mark's9October direction as additional precise derivation and change record; all existing verification links remain. Financial quantities require currency/period/basis; resource quantities require kind/unit/period/capacity context and applicable competing duty; unknown is not zero. Independently governed authority, privacy, cumulative and resource-allocation criteria remain controls even when another materiality criterion is satisfied. Exact thresholds and mixed-impact conflict adjudication belong to the organisation's approved profile, not to supplier discretion.

# 5. State Model
Canonical lifecycle: **Proposed → Assessed → Authorised/Constrained/Denied/Unresolved → Pending Execution → Dispatched → Outcome Pending → Confirmed/Failed/Partial/Indeterminate → Closed**. Not every exchange traverses every state.

**Proposed:** exchange requested/identified; no authority implied.  
**Assessed:** relevant purpose, authority, data-use and boundary conditions evaluated.  
**Authorised:** current requirements satisfied; remains conditional on authority/context remaining valid.  
**Constrained:** may proceed only under explicit conditions.  
**Denied:** may not proceed under current conditions.  
**Unresolved:** required determination cannot be established; dependent execution withheld.  
**Pending Execution:** authorised but not yet crossed boundary; applicable change may trigger reassessment.  
**Dispatched:** crossed controlled boundary; dispatch does not establish external effect.  
**Outcome Pending:** consequence expected but not established.  
**Confirmed:** evidence establishes defined external outcome.  
**Failed:** intended exchange/effect did not occur.  
**Partial:** only part occurred.  
**Indeterminate:** evidence cannot establish effect to required standard; must not be silently converted to success.  
**Closed:** no further action required or authorised process has formally closed unresolved outcome; provenance and obligations remain.

# 6. Semantic Contracts and Interfaces
**AOS-14-CON-001 — External Exchange Request:** actor, external party/destination, direction, purpose, proposed content/action, authority context, identity context, timing and consequentiality where known. Detailed schema jointly defined with AOS-01/02/03/04.

**AOS-14-CON-002 — Exchange Determination:** **Permit / Constrain / Deny / Quarantine / Escalate / Unresolved**, identifying evidence, authority, policy version and conditions.

**AOS-14-CON-003 — External Exchange Evidence:** what occurred at the boundary and known external outcome; common semantics belong to AOS-02.

**AOS-14-CON-004 — External Obligation:** obligation governing or arising from exchange; ownership/lifecycle require joint definition with AOS-01/02/03 and relevant domain owners.

### 6.1 Typed determination and authoritative logical mapping

CON-001–004 are Boundary views of AOS-14-IF-001 in Shared Contracts§4.7, with AOS-02-IF-001 supplying evidence custody, not independent schemas or authority grants. CON-005 adopts the single AOS-02§6.6 / AOS-04-CON-009 RSVIEW-0.1 research pattern. Producer/consumer duties are reciprocal in Exchange Register's9October Boundary addendum. Physical wire schemas remain jointly approved by02 and semantic/control owners before dependent build; logical adoption does not select a transport or data type.

| Context / original vocabulary | CON-002 boundary meaning | Required behaviour |
| --- | --- | --- |
| Inbound `admit` | Permit for the declared inbound operation | Allows only that boundary entry; no assertion of truth, organisational authority,02 evidence acceptance or recipient use |
| Inbound `admit with conditions` | Constrain | No dependent entry/use until its exact applicable conditions are satisfied; restricted storage may be separately authorised |
| Inbound `quarantine` | Quarantine: restricted evidence custody state | Retain under approved restricted custody; no executable permission or automatic release |
| Inbound `reject`; outbound `deny` | Deny | Withhold the assessed operation; preserve reasons and permitted challenge route |
| Outbound `permit` / `constrain` | Permit / Constrain for exact disclosure/contact/commitment | Apply exact audience/payload/purpose and final current shared checks |
| Either direction `escalate` | Escalate: accountable review routing state | Escalation is not permission; dependent operation remains withheld absent a separate current grant |
| Either direction `unresolved` | Unresolved | Withhold the dependent operation; report the missing/conflicting determination |
| Shared02 `accepted`, `accepted with restrictions`, `rejected`, `unresolved` | Separate evidence-admission axis | A Boundary admission may feed02 assessment; no automatic coercion between the axes |
| Unknown label, missing direction/operation or incompatible revision | Invalid instance; unresolved dependent determination | Reject dependent use, retain diagnostic/owner; no permissive default |

The typed logical object retains its context and original disposition. Implementation may encode the mapped terms only under an approved explicit enum/version mapping; the table does not approve a wire enum. Quarantine and escalation do not silently become Authorised state. Assessments, source standing, technical receipt, semantic application, responsibility acceptance and actual effect remain separate axes.

### 6.2 Minimum contract duties and commissioning completeness

| View | Producer → permitted consumer / owner | Minimum content and preconditions | Failure, timing and lifecycle |
| --- | --- | --- | --- |
| CON-001 request | Domain/13/04 or permitted external intake →14;14 owns exchange meaning,02 common record | Stable request/attempt linkage; actor/principal/party/destination; direction/operation; purpose; payload/content reference and source standing; current01/03 context; approved boundary/consequentiality/profile revisions; obligation references | Invalid/unknown scope: owned unresolved assessment, no dependent effect; pre-dispatch cancellation/revocation triggers reassessment; duplicate request does not imply repeat authority |
| CON-002 determination |14 consuming01/03/04/05 authoritative controls → requesting executor/13/02 | Exact CON-001 and control/evidence revisions; typed context/disposition; constraints; valid/current standing and permitted explanation/referral | Missing/stale/conflicting controls withhold; final check at effect boundary; late/out-of-order updates resolve against current master; reassessment recorded |
| CON-003 evidence |14/connector with05/04 observations and counterpart/domain evidence →02/13/permitted domain/25/30/40 | Request and distinct attempts/events; origin/currentness/assurance; applied checks; stage/time; dispatch, transport receipt, semantic acknowledgement, claimed/observed effect, uncertainty; disclosure restrictions; accepted follow-up | Lost response/partial/duplicate/dispute not success; reconcile before retry; permitted audit survives under agreed minimisation/deletion treatment; general outcome-specific rule approved DEC-093; exact exchange-type evidence remains a commissioned profile |
| CON-004 obligation |14 recognised source with01/03/domain legal/semantic steward →02/13/30 appointed duty owner | Source/applicability/basis; exact exchange; obligation identity/current standing; separate financial/resource impacts where applicable; empowered owner/tracker; deadline where applicable, fulfilment evidence; staged acknowledgement/cover and residual duty | DEC-094 settles the common representation/ownership direction; unresolved exact schema or substantive applicability still gates dependent commitments; no timeout implies acceptance; closure/recovery retains real outstanding duty |
| CON-005 research | Assigned component agents and14 shared retrieval →02 custody/component reviewers/13/30;04 behaviour,component relevance | Single02§6.6 profile/run/finding/disposition views; exact component/remit/source/baseline/evidence/coverage; shared source identity but distinct substantive owners and duties | Common correction/revocation/duplicate/lifecycle semantics; failed/unperformed versus bounded no-finding distinguished; acceptance-for-work not amendment or release |

Every approved compatible manifest must define mandatory versus optional fields, identifier references and allowed cardinalities; enum/range validation; units (or explicit no-numeric-field judgement); timestamp origin/time zone/precision and currentness; payload limits; ordering/duplicate/retry protocol; stage acknowledgement and human response windows; invalid/missing/expired/revoked behaviour; authoritative owners/control locations; profile validation, revision and approval. Values are not supplied here. Time windows are measured from the manifest-defined observed event, never from an invented local clock assumption. Absent invalid or expired mandatory manifest/profile means no dependent effect or reliance and an owned gap. Purpose, licensing, access, retention, correction, deletion and restoration cover both raw and derived records; evidence retention does not imply permanent unrestricted storage. Profile completeness and shared owners' acceptance are build gates, not optional configuration choices.

### 6.6 Common research adoption

**AOS-14-CON-005** references AOS-04 v0.8 §§3.1/5.1/6.6/10.8 (CON-009), AOS-02 v0.8 §6.6 (CON-007) and AOS-01 v0.8 §§6.6/10.8. AOS-00/Map v0.22, DEC-001–086; AOS-01–05 v0.7; AOS-14 v0.3; AOS-20 v0.2; Shared v0.6/Core v0.5/Register v0.5; source matrix v0.7; template v0.4. No new approved IF/REC identifier is created. AOS-02 §6.6 is the single proposed logical view definition; this component supplies the remit/finding semantics, 04 behaviour, 14 access/admission evidence, 03 permitted-use decisions, 05 observed enforcement, 13 tracked handoff and 30/01 empowered disposition/change. Profiles/agents → permitted 02 custody/component reviewers; decisions → exact finding/change follow-up. Register v0.5 §13 records exact producer/consumer adoption and logical supporting-view revision RSVIEW-0.1. Wire types/cardinalities/units, mappings and approved compatible schema manifests remain gated shared-schema work, not inferred from logical adoption.

Profile/run/finding/disposition states inherit AOS-04 §5.1; neither run completion, source verification nor proposal acceptance establishes approval/application/compliance. Existing staged acknowledgement, current checks, correction/revocation, recovery, privacy/licensing and source-lifecycle duties apply to raw and derived research. AOS-14’s own research and its shared retrieval service use distinct assignments/owners; its broad pilot horizon routes shared-control implications to their owners.

# 7. Authority and Decision Boundaries
AOS-14 may, where authorised, assess, constrain, deny according to established policy, quarantine, withhold dependent execution, request evidence, escalate and record. It may not create or expand authority; amend telos; waive constitutional constraints; decide Mode 2 questions; grant itself capabilities; suppress mandatory escalation; or amend its own specification. Technical executability is not authority.

# 8. Reasoning Principles Applied
**Telos:** exchange remains connected to legitimate purpose.  
**Integral Ethics:** an authorised exchange may still require ethical challenge; ethics does not replace independently enforced authority.  
**Epistemic Brakes:** material uncertainty in identity, provenance, authority, obligation or outcome remains visible.  
**Radical Transparency:** consequential exchange remains reconstructable.  
**Human Mode 2:** AOS-14 cannot autonomously resolve incommensurable values, constitutional interpretation or other reserved human questions.

# 9. Data, Privacy and Disclosure
AOS-14 consumes AOS-03 determinations concerning legitimate access, permitted processing, consent and disclosure. Possession does not imply permission to disclose. External material remains subject to provenance, purpose, receiving-domain controls, retention, confidentiality, correction, onward-disclosure constraints and externally imposed obligations. Radical Transparency does not mean unrestricted visibility.

# 10. Behaviour and Workflows
**Inbound:** external source → exchange recognised → source/context assessed → admissibility determination → admit/condition/quarantine/reject/escalate → governed record → receiving-domain use. Admission is not truth.

**Outbound:** proposed disclosure → recipient/purpose → authority/permitted-use check → assessment → permit/constrain/deny/escalate → execution → evidence/outcome.

**Commitment:** proposed commitment → authority determination → boundary assessment → authorised execution or withholding → external effect → obligation/outcome record.

**Authority change while pending:** pending exchange → authority/policy change → invalidate prior determination where applicable → reassess → execute/withhold/escalate.

**Outcome reconciliation:** dispatch → external evidence awaited → confirmation/failure/partial/duplicate/indeterminate → authorised follow-up → closure.

**Pattern review:** exchange evidence → cumulative observation → material pattern → oversight signal → review → disposition.

### 10.4 External-research workflow and exceptions

Approved profile/exact draft and governing baseline → permitted AOS-14 retrieval → source/admission/assurance/status evidence → specialist component relevance assessment → common run and finding/coverage record → permitted tracked review through 13/30 → empowered disposition → separately controlled change under 01 → required evaluation/compatible application and outcome follow-up. Shared retrieval retains each component’s assessment, owner, deadlines and disposition. A stale baseline or corrected/restricted source prompts recorded reassessment; preserve the original historical assessment, and propagate material impact under existing CHG/lifecycle rules.

Blocked access, missing baseline, partial/failed coverage, unavailable reviewer or failed delivery produces an explicit owned exception. No silent substitution of sources, route, processing basis or reviewer is permitted. Ordinary quiet reporting cannot conceal missing coverage records; if the platform cannot retain a run record, expose that operational gap. Urgent operational/legal/safety concerns follow the separately authorised protected route without waiting for amendment; receipt is not human acceptance or completion.

# 11. Failure, Escalation and Recovery
If authority is unavailable/unresolved, withhold dependent consequential exchange and use authorised escalation. If external identity is insufficient, constrain/quarantine/reject/escalate. Destination unavailable: preserve pending/failed state; do not infer success. Outcome uncertain: record indeterminate and reconcile where required. Duplicate/replay: prevent or reconcile unintended duplicate consequence through responsible execution controls and evidence. Policy changes while pending: reassess where applicable. Attempted bypass must not convert prohibited/uncontrolled action into legitimate exchange; enforcement belongs jointly to AOS-01/03/04/05. If AOS-14 is unavailable where mandatory, absence must not create an uncontrolled external route.

# 12. Evidence, Provenance and Audit
Where applicable reconstruct **actor → external party → purpose → authority → evidence → constraints → determination → exchange → external effect → obligations → escalation → outcome**. Evidence includes actor, party/destination, direction, purpose, authority/version, policy/contract, material exchanged, timestamp, obligations, determination, execution state, known outcome, uncertainty, exceptions and escalation. Common record semantics belong to AOS-02.

# 13. Security and Operational Requirements
AOS-14 operates within AOS-05 controls. Additional constraints arise where integrations create trust boundaries; credentials/secrets are required; delayed/duplicate/out-of-order exchange alters consequence; external availability affects state; policy changes affect queued exchanges; outcome requires reconciliation; or boundary controls could be bypassed. AOS-14 prescribes no network topology, gateway product, protocol or cloud platform.

# 14. Invariants
**AOS-14-INV-001:** Technical ability to exchange does not establish organisational authority.  
**AOS-14-INV-002:** AOS-14 cannot create authority absent from the organisational authority framework.  
**AOS-14-INV-003:** Where required authority is unresolved, dependent consequential execution must not proceed.  
**AOS-14-INV-004:** Admission of external information does not establish truth or authority.  
**AOS-14-INV-005:** Consequential exchange must leave sufficient evidence for required reconstruction.  
**AOS-14-INV-006:** AOS-14 remains subject to AOS-01/03/04/05 controls.  
**AOS-14-INV-007:** AOS-14 must not silently assume systemwide authority enforcement, internal permission control or agent containment.  
**AOS-14-INV-008:** Unknown external outcome must not be represented as confirmed success. Status dependent on ISS-005.

# 15. Conformance and Acceptance
**AOS-14-CR-001:** Defined consequential external exchange is recognised and subjected to applicable AOS-14 contract.  
**CR-002:** Exchange lacking required authority does not execute.  
**CR-003:** Admitted external information remains distinguishable from verified/authoritative evidence.  
**CR-004:** Outbound disclosure is evaluated against recipient, purpose, authority and permitted use before release.  
**CR-005:** Model/agent proposal alone cannot authorise consequential external commitment.  
**CR-006:** Consequential external exchange can be reconstructed from required evidence.  
**CR-007:** Pending exchange affected by changed/revoked authority is reassessed before execution.  
**CR-008:** Where dispatch does not establish effect, successful completion is not falsely recorded. Status dependent on ISS-005.  
**CR-009:** Alternative execution route cannot silently legitimise an exchange subject to mandatory AOS-14 control.  
**CR-010:** AOS-14's own actions remain subject to shared controls.  
Conformance claims follow current AOS-40 v0.5: exact approved scope/baseline, requirement and case coverage, executed evidence, findings and exclusions are recorded. A partial scope cannot claim whole-component conformance or waive inherited controls, residual human duties or blocked dependencies. No partial or full conformance is claimed for this draft.

### 15.3 External-research planned acceptance

Approved synthetic fixtures, scope values and assessor roles must be supplied before execution. Component/privacy/platform reviewers and AOS-04/40 evaluators assess their respective meanings/controls; retain source, task, control, coverage, finding, handoff and human disposition evidence with limitations.

| VER | REQ coverage | Controlled inputs / procedure | Expected result / retained evidence |
| --- | --- | --- | --- |
| 001 | 001/007 | Profile/remit/source admission incomplete; wrong jurisdiction or future-effective proposal; relevant authoritative development; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Require scoped approved profile; correctly distinguish relevance/source status and exact baseline; unsupported reliance withheld; no invented values. Planned, not executed. |
| 002 | 002 | Denied retrieval, hostile page instructions and substituted tools/processing purpose; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Observe independent denial; source cannot change powers/profile; disclose coverage gap without broadening access. Planned, not executed. |
| 003 | 003 | Stale baseline, conflicting assurance or missing source/effective dates; partial/failed/unperformed run and completed bounded no-finding; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Preserve evidence/inference/unknowns and exact history; correctly distinguish coverage states and record owned follow-up. Planned, not executed. |
| 004 | 004/008 | Shared source impacts two components; duplicate finding and later source correction; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Reuse source identity while retaining distinct findings/owners/deadlines; propagate/reassess material correction without dropping duties. Planned, not executed. |
| 005 | 005 | Unresponsive reviewer, failed delivery and urgent live implication; accepted-for-work candidate attempts direct activation; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Retain tracker/cover/approved escalation; no simulated delivery or self-amendment; human disposition does not equal release/application. Planned, not executed. |
| 006 | 006 | Human-approved rubric with relevant, irrelevant, missed and distorted evidence examples; deterministic bypass fixture; exact synthetic profile/dependency revisions, permitted assessor/tool scope | Retain assessed evidence-fidelity/relevance/false-missed findings and limits separately from observed control tests; no self-certified sufficiency. Planned, not executed. |

### 15.4 Supplier allocation planned acceptance

**AOS-14-VER-007 — Supplier responsibility, integration and evidence allocation.** Requirement: AOS-14-REQ-009. Method: author/supplier mapping walkthrough followed by actual scoped integration and control/failure tests; process, domain, identity/use, runtime, data and assurance stewards assess their respective meanings. Walkthrough cannot establish implemented enforcement.

**Inputs and prerequisites:** exact supplier product/service/version/configuration and release scope; approved isolated fixtures/destinations; exact common contracts, source/domain and boundary profiles; permission/control and actual-effect observation arrangements; appointed responsible parties and empowered human cover. Include one combined platform, a split supplier arrangement, unsupported schema/identity, missing owner, denied/revoked permission, lost external-effect response and a supplier feature marked “met” without evidence. Undefined boundary, consequentiality, obligation or outcome rules remain blocked dependencies, not guessed values.

**Procedure:** map every included requirement and older CAP/FUN/CON/INV/CR obligation to supplier contribution, authoritative owner, actual producer/consumer and relevant component/assembled case. Inspect standalone/manual exclusions and combined-platform internal flows. Challenge missing ownership and unsupported claims. For commissioned routes, observe denial at the real effect boundary, permission change while queued, duplicate/unknown effect reconciliation before authorised repetition, preserved source/use restrictions and actual accepted residual duty. Trace evidence back to the exact mapped versions; inject a changed supplier configuration and identify required reassessment.

**Expected result:** no included obligation disappears between products or inside one product. Shared owners retain authority; denied/unresolved effects cannot proceed through an alternative supplier route. Unsupported identity/meaning and partial/indeterminate outcomes remain visible and owned. Claimed conformance is scoped to actual evidence; gaps name a responsible party and affected build/activation gate. Product capability is not permission, delivery is not human acceptance, and partner receipt is not the required service outcome. Excluded capability cannot waive continuing governing duties. No all-product or whole-suite certification is inferred.

**Evidence:** exact allocation/response rows, scope/exclusions, profile/schema/owner manifests, observed exchanges/checks/prevention/effects and reconciliation, accepted human/residual duty records, findings/remedy/retest and configuration-change impacts. Links: §§3.2/3.3/18.1/20; existing VER-001–006 for research;13 v0.1 REQ-021/022/049/055 and VER-015/035/039;40 v0.5 applicable scope/reciprocal/control/recovery cases. Status: planned, not executed.

### 15.5 Core and assembled planned verification

**Common case record (VER-008–034):** status planned, not executed; baseline AOS-14 v0.7 with current manifest in the opening control. Method is requirements/contract inspection plus isolated integration and failure injection at actual enforcement/receipt/effect boundaries. Preconditions for each case are approved synthetic data and safe isolated destinations, exact profiles/schemas/authority/use/rubric revisions, fixture observation clocks and event windows, appointed Boundary and independent shared-control/domain assessors, empowered human owners/cover, consent/licensing restrictions and recorded expected results. Missing approvals/profiles block execution; no test supplies a production default. Keep input/event/control revisions, attempted and observed effects, stage/time evidence, explanation/uncertainty, accepted duties, assessor/results, failures/remedy/retest and limits in permitted02 custody. Pass requires every listed expected result and each linked normative obligation to hold; an attempted prohibited effect must be demonstrably prevented, not merely described. A walkthrough alone cannot pass implemented enforcement.40 owns assembled assurance;30/human assessors determine actual judgement and institutional claims separately.

**AOS-14-VER-008 — Perimeter and classification.**

**v0.7 decision fixtures:** Include a low-price exchange with substantial staff/capacity commitment, high financial exposure with little staff time, cumulative commitments, unknown financial/resource standing, routine public retrieval and a supplier delegated internal operation with onward external disclosure. Apply exact approved organisation criteria independently to each impact; compare operation/data-use control paths. **Additional pass condition:** no monetary-only shortcut, unknown-as-zero or hosting-only boundary; ambiguous classifications stay owned and cannot use the lighter route. Derivation: DEC092/095.

**Requirements:** AOS-14-REQ-010, AOS-14-REQ-011, AOS-14-REQ-012. **Fixtures/preconditions:** approved bounded external route, hosted/combined/manual variants and an unknown control/consequentiality profile, plus the common record above. **Procedure:** classify inbound/outbound operations then omit/contradict the required perimeter/classification. **Expected/pass condition:** valid scope uses its exact contract; unknown scope stays owned and withheld. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-009 — Identity and source standing.**

**Requirements:** AOS-14-REQ-013, AOS-14-REQ-014. **Fixtures/preconditions:** verified, spoofed, uncertain and corrected sources; stale effective times, plus the common record above. **Procedure:** receive each material source and forward only permitted evidence. **Expected/pass condition:** identity assurance/source correction and uncertainty survive; connectivity proves neither identity nor truth. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-010 — Typed admission and constraints.**

**Requirements:** AOS-14-REQ-015, AOS-14-REQ-016, AOS-14-REQ-017. **Fixtures/preconditions:** all §6.1 labels in each valid/invalid context;02 acceptance variants; unmet constraint, plus the common record above. **Procedure:** map dispositions, attempt custody/use/release and later condition satisfaction. **Expected/pass condition:** valid mappings retain axes; quarantine/escalation/invalid labels never permit dependent execution. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-011 — Disclosure and channel.**

**Requirements:** AOS-14-REQ-018, AOS-14-REQ-019. **Fixtures/preconditions:** permitted/denied audience and payload; agreed channel changed or unavailable, plus the common record above. **Procedure:** attempt release, change recipient/channel while queued, observe permitted delivery/failure. **Expected/pass condition:** only current exact scope dispatches; unapproved substitute does not; failed duty remains owned. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-012 — Authority and final check.**

**Requirements:** AOS-14-REQ-020, AOS-14-REQ-021, AOS-14-REQ-022. **Fixtures/preconditions:** valid/expired/revoked/unavailable grants; model proposal; unsolicited contact; queued attempt, plus the common record above. **Procedure:** request commitment then revoke between initial assessment and final effect check. **Expected/pass condition:** no permission from proposal/relationship; invalid grants withhold at actual enforceable boundary. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-013 — Hostile external input.**

**Requirements:** AOS-14-REQ-023. **Fixtures/preconditions:** page/message with embedded instructions to reveal data or change tooling, plus the common record above. **Procedure:** ingest under permitted isolated profile and attempt injected instructions. **Expected/pass condition:** content cannot create authority or change purpose/tools; incident/coverage evidence retained. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-014 — Change and reordering.**

**Requirements:** AOS-14-REQ-024, AOS-14-REQ-025. **Fixtures/preconditions:** two authority/source/profile revisions, cancellation and late stale event, plus the common record above. **Procedure:** queue work then deliver changes in reversed order and attempt execution. **Expected/pass condition:** affected work reassessed; obsolete event cannot restore permission; unaffected work retains exact scope. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-015 — Alternative and combined route.**

**Requirements:** AOS-14-REQ-026. **Fixtures/preconditions:** split connector and one combined platform with alternate route, plus the common record above. **Procedure:** deny the governed exchange then attempt product-internal/alternate dispatch. **Expected/pass condition:** all declared perimeter crossings observe denial; any unenforced route is a blocking finding. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-016 — Cumulative shared controls.**

**Requirements:** AOS-14-REQ-027. **Fixtures/preconditions:** concurrent exchanges with common cumulative account/reservation and exhausted condition, plus the common record above. **Procedure:** split one operation into requests/products and race final checks. **Expected/pass condition:** shared accounting governs attempts; split/private budget cannot create capacity or permission. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-017 — Duplicate attempt identity.**

**Requirements:** AOS-14-REQ-028. **Fixtures/preconditions:** one request, multiple distinct authorised attempts and duplicate/out-of-order receipts, plus the common record above. **Procedure:** redeliver requests/events and inspect effect/reconciliation evidence. **Expected/pass condition:** identities and deduplication retain standing; duplicate delivery does not authorise another effect. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-018 — Actual-effect uncertainty.**

**v0.7 decision fixtures/pass condition:** Profile-specific sending, delivery, acceptance and actual-fulfilment evidence stay distinct; contractor receipt cannot prove repair completion. Unsupported expected effect remains unknown. Derivation DEC093.

**Requirements:** AOS-14-REQ-029, AOS-14-REQ-030. **Fixtures/preconditions:** profile-defined success evidence; lost response, partial effect and disputed completion, plus the common record above. **Procedure:** compare dispatch/receipt/claimed/observed effect and request closure. **Expected/pass condition:** only profile-supported class confirmed; unknown/partial preserved with owner; no HTTP/receipt success proxy. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-019 — Retry and compensation.**

**Requirements:** AOS-14-REQ-031, AOS-14-REQ-032. **Fixtures/preconditions:** uncertain prior effect, observation unavailable, then authorised reconciliation and compensation, plus the common record above. **Procedure:** attempt immediate repetition and compensating action without/with separate current grants. **Expected/pass condition:** repeat waits for authorised reconciliation/fresh checks; compensation has independent authority/history. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-020 — Obligations and accepted owner.**

**v0.7 decision fixtures/pass condition:** Inspect source/applicability/exchange/human owner/deadline-where-applicable/fulfilment evidence/status; retain financial/resource impacts separately with units and uncertainty. Boundary recognition, domain interpretation,02 semantics,13 tracking and30 disposition remain distinct; conflicting substantive obligations reach an empowered human. Derivation DEC094.

**Requirements:** AOS-14-REQ-033, AOS-14-REQ-034. **Fixtures/preconditions:** applicable/uncertain obligation source, empowered and unavailable owner, plus the common record above. **Procedure:** recognise obligation, route for acceptance then reject or fail delivery. **Expected/pass condition:** exact applicability/status and tracker retained; no fabricated schema or presumed ownership. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-021 — Acknowledgement and closure.**

**v0.7 decision fixtures/pass condition:** An empowered person may terminate investigation under the approved profile while retaining explicitly unknown outcome and accepted residual duty; neither administrative closure nor acceptance converts to fulfilled effect. Derivation DEC093/094.

**Requirements:** AOS-14-REQ-035, AOS-14-REQ-036. **Fixtures/preconditions:** separate receipt/validation/application/acceptance; missed window; residual duty, plus the common record above. **Procedure:** advance stages, lose acceptance, invoke cover/escalation and authorised unresolved closure. **Expected/pass condition:** time windows use fixture profile; no timeout acceptance or closure-success coercion; residual duty stays owned. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-022 — Human and protected referral.**

**Requirements:** AOS-14-REQ-037, AOS-14-REQ-038. **Fixtures/preconditions:** permitted internal route, prohibited external contact, required audience and implicated recipient, plus the common record above. **Procedure:** route ordinary/protected findings and inject suppression request. **Expected/pass condition:** internal route not external power; required independently permitted audience/alternative and tracked acceptance preserved. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-023 — Purpose and lifecycle.**

**Requirements:** AOS-14-REQ-039, AOS-14-REQ-040. **Fixtures/preconditions:** raw/derived research and resident data, rejected inference purpose, restriction/deletion/correction, plus the common record above. **Procedure:** attempt changed use/disclosure; propagate lifecycle change to queued/derived uses. **Expected/pass condition:** unapproved purpose withheld; authorised lifecycle treatment persists without deleting required evidence indiscriminately. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-024 — Failure and recovery.**

**Requirements:** AOS-14-REQ-041, AOS-14-REQ-042. **Fixtures/preconditions:** interrupted dispatch, restricted/deleted source, revoked grant and scoped incident route, plus the common record above. **Procedure:** restore old snapshot then attempt continuation/incident communication. **Expected/pass condition:** current standing and prior effects reconciled; only separately permitted minimum incident route used. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-025 — Risk, gaps and overrestriction.**

**v0.7 decision fixtures/pass condition:** Repeated disclosure, accumulating financial/resource commitments, unusual counterparties, excessive restriction and split-action evasion produce bounded Boundary evidence.25 retains combined cross-domain drift/system-risk interpretation; shared controls retain limits/accounting and humans decide changes. Derivation DEC096.

**Requirements:** AOS-14-REQ-043, AOS-14-REQ-044, AOS-14-REQ-045. **Fixtures/preconditions:** intrinsic boundary risk, unobserved population, failed check, unequal restriction burden, plus the common record above. **Procedure:** produce quiet/partial reports and challenge service restriction. **Expected/pass condition:** scope/uncertainty/coverage disclosed; owned risk/restriction review; no self-waiver or quiet=no-risk claim. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-026 — Oversight and feedback.**

**Requirements:** AOS-14-REQ-046. **Fixtures/preconditions:** permitted25/30 pattern inputs, unavailable reviewer and received disposition, plus the common record above. **Procedure:** refer boundary pattern, track acceptance and return actual-outcome evidence. **Expected/pass condition:** 14 supplies bounded evidence;25/humans retain aggregate judgement; no unaccepted duty disappears. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-027 — Federation exclusion.**

**Requirements:** AOS-14-REQ-047. **Fixtures/preconditions:** bounded approved external exchange and proposed uncommissioned federated delegation, plus the common record above. **Procedure:** attempt to infer trust/authority from partner platform or protocol. **Expected/pass condition:** deferred model stays excluded; bounded exchange only under its own complete approved profile. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-028 — Quality and change.**

**Requirements:** AOS-14-REQ-048, AOS-14-REQ-049. **Fixtures/preconditions:** human-approved relevant/irrelevant/missed/distorted cases; provider/configuration change, plus the common record above. **Procedure:** measure fidelity/error criteria separately from deterministic controls then change provider. **Expected/pass condition:** reliance requires accepted rubric/results; changed evidence reassessed; passed model score cannot waive controls. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-029 — Contract compatibility.**

**Requirements:** AOS-14-REQ-050. **Fixtures/preconditions:** valid manifest; bad identifiers/units/time/cardinality/enum/revision, plus the common record above. **Procedure:** produce/consume each view with valid then malformed/stale instances. **Expected/pass condition:** both sides reference same master; invalid dependent use withheld with owned diagnostic. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-030 — Audit and explanation.**

**Requirements:** AOS-14-REQ-051, AOS-14-REQ-052. **Fixtures/preconditions:** normal and denied exchange with restricted evidence and uncertainty, plus the common record above. **Procedure:** independent authorised assessor reconstructs exact revisions/effect/duty and recipient challenge basis. **Expected/pass condition:** retained evidence supports reconstruction; explanation is not private chain-of-thought or an authority grant. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-031 — Domain status fidelity.**

**Requirements:** AOS-14-REQ-053. **Fixtures/preconditions:** asset golden-thread source, promise revision, partial/unverified work and human chair/board records, plus the common record above. **Procedure:** exchange records, inject transport-success and chair endorsement as completion/board approval. **Expected/pass condition:** source/domain and human standing preserved; delivery does not upgrade physical/statutory/board status. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-032 — Supplier exit.**

**Requirements:** AOS-14-REQ-054. **Fixtures/preconditions:** approved supplier exit/export route with restricted data and revoked authority, plus the common record above. **Procedure:** export permitted evidence and revoke connector; attempt ongoing exchange. **Expected/pass condition:** only permitted audience/use export succeeds; exit retains residual duties without continuing revoked effects. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-033 — Manual continuity.**

**Requirements:** AOS-14-REQ-055. **Fixtures/preconditions:** approved manual route, operator competence/evidence requirements and unavailable automated controls, plus the common record above. **Procedure:** switch to manual, attempt unauthorised bypass and record remaining duties. **Expected/pass condition:** manual operation preserves controls/evidence; unsupported scope withheld with owner. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 applicable authority, admission, disclosure, acknowledgement, unknown-effect, recovery and supplier cases selected in the approved scoped case manifest. No institutional GT result inferred.

**AOS-14-VER-034 — Assembled overdue repair.**

**Requirements:** AOS-14-REQ-011, AOS-14-REQ-017, AOS-14-REQ-019, AOS-14-REQ-020, AOS-14-REQ-029, AOS-14-REQ-030, AOS-14-REQ-035, AOS-14-REQ-036, AOS-14-REQ-037, AOS-14-REQ-053. **Fixtures/preconditions:** exact10/11/13/14/30/40 versions; promise/completion fixtures, named owner/team and agreed channel; supplier effect observer, plus the common record above. **Procedure:** carry overdue-unverified repair through accepted human duty, resident contact and contractor exchange; lose response, revoke authority, reconcile, preserve disputed/partial completion. **Expected/pass condition:** domain promise/history, accepted duty and resident channel survive; boundary dispatch neither proves work nor service remedy; retry blocked until authorised reconciliation/fresh checks. **Evidence/assessor:** common record above;14 exchange steward,02 semantics/custody,01/03/04/05 applicable control owners,13/30 accepted-duty stewards and affected domain specialists;40 assessor for assembled coverage. **Integration counterpart:** 40 VER-007–010/020–025/036/038;10/11/13/30 retained domain cases. No institutional GT result inferred.

# 16. Dependencies
AOS-14 depends on AOS-01 authority; AOS-02 semantics/records; AOS-03 identity/access/consent/data use; AOS-04 agent execution; AOS-05 security/enforcement/resilience; AOS-10–13 domain producers/consumers; AOS-20–25 governance interpretation/oversight; AOS-30 accountable human workflows; and AOS-40 assurance/conformance. External dependencies include actors/systems, authority instruments, data-sharing/contractual arrangements, jurisdictional obligations and external identity/provenance mechanisms. Missing activation dependencies must not be replaced by implementation assumptions.

# 17. Issues
## AOS-14-ISS-001 — Federated Exchange
**Type:** design question. **Source:** Architecture Issues Register OQ-012. **Question:** What authority, identity, provenance, obligation and incident information may or must cross independently governed organisations? **Affected:** CAP-007/FUN-008. **Status:** Deferred under OQ-012; the general federated operating model is outside the current bounded draft. **Decision gate:** before dependent federated build/conformance; REQ-047/VER-027 preserve exclusion.

## AOS-14-ISS-002 — Boundary Terminology
**Type:** architectural ambiguity. **Source:** OQ-013. **Question:** Is “Boundary Intelligence” sufficiently unambiguous given the distinction between external exchange and systemwide enforcement? **Affected:** responsibility boundary. **Status:** Working naming resolved in OQ-013 on 3 October 2026. **Disposition:** DEC-005 remains controlling; Boundary owns external exchange and shared controls enforce systemwide. This does not resolve mechanism adequacy or ISS-007.

## AOS-14-ISS-003 — Cumulative External Behaviour
**Type:** responsibility allocation. **Source:** OQ-007. **Question:** Which cumulative external patterns belong to AOS-14 sensing and which to AOS-25 oversight? **Affected:** CAP-008/FUN-009. **Status:** Architectural direction resolved9October2026 by AOS-00-DEC-096; exact scoped implementation/commissioning remains open.

## AOS-14-ISS-004 — External Consequentiality
**Type:** definition dependency. **Source:** OQ-006 and AOS-00 consequential-action work. **Question:** What constitutes a consequential external exchange requiring the full control/evidence path? **Affected:** all capabilities. **Status:** Architectural direction resolved9October2026 by AOS-00-DEC-092; exact scoped implementation/commissioning remains open.

## AOS-14-ISS-005 — Evidential Closure
**Type:** research challenge / clarification candidate. **Source:** AOS-14 research custodian. **Question:** For which consequential exchanges must AOS establish actual external effect rather than authorised dispatch alone? **Affected:** CAP-006/FUN-007/INV-008/CR-008/State Model. **Status:** Architectural direction resolved9October2026 by AOS-00-DEC-093; exact scoped implementation/commissioning remains open. **Disposition:** Clarify candidate; not yet normative.

## AOS-14-ISS-006 — External Obligations
**Type:** semantic ownership. **Question:** What is the authoritative representation, owner and lifecycle of obligations acquired through external exchange? **Affected:** CAP-005/FUN-005/CON-004. **Status:** Architectural direction resolved9October2026 by AOS-00-DEC-094; exact scoped implementation/commissioning remains open.

## AOS-14-ISS-007 — Dynamic Organisational Boundary
**Type:** architectural definition. **Question:** How is the external boundary determined where suppliers, hosted services, agents and federated platforms operate under mixed organisational control? **Affected:** CAP-001/FUN-001. **Status:** Architectural direction resolved9October2026 by AOS-00-DEC-095; exact scoped implementation/commissioning remains open.

### AOS-14-ISS-008 — External-research setup and assurance

Common logical inheritance is incorporated; remaining exact sources/jurisdictions/cadence/triggers, agent assignment, recipients/response/cover, approved rubrics and wire schema/compatibility are owned dependencies per §3.1. Component owner coordinates 01/02/03/04/05/14/13/30/40 and specialist reviewers. Gate: dependent build/research activation/reliance; evidence: controlled profiles/schema mappings, accepted evaluations and actual coverage/handoff/disposition results. No new general architecture question is submitted. Existing unresolved issues retain their scope; research pilot item 5b is not closed.

### 17.1 Owned resolution and scope gates

Mark is the project decision custodian; the organisational roles below must be appointed rather than presumed filled. No calendar deadline has been authorised: the stated dependent gate is the required resolution point. The five general principles are now expressly settled in§3.4/DEC092–096. Exact scoped parameters/arrangements are not silently supplied by REQ wording or a supplier profile. An approved bounded scope must explicitly determine its affected rules, excluded behaviours and dependencies before build; excluding a capability cannot evade inherited governing duties.

| Issue / standing | Decision owner and required approval | Affected requirements / evidence needed / gate |
| --- | --- | --- |
| ISS-001 deferred federation |01/03 authority/identity and14; Mark/appointed organisational authority |047 plus010/013/020/033; partner trust/mandate/provenance/incident alternatives and approved federation model before dependent build |
| ISS-002 resolved working naming | Mark; DEC-005 retained | No naming gate; inspect responsibility mappings026/047 and boundary010 to prevent conflation |
| ISS-003 direction resolved DEC096; profiles open |14/25 with01/05 cumulative controls; Mark |027/043–046; exact local-versus-system pattern triggers, audience, risk perimeter and follow-up before affected sensing build; shared accounting remains controlling |
| ISS-004 direction resolved DEC092; criteria open |01 constitutional definition with14/domain stewards; Mark/empowered authority |011/012/020–022/029/051; approved scoped classes and ambiguous-case treatment before dependent exchange build |
| ISS-005 direction resolved DEC093; exchange evidence profiles open |14/02/13/domain owner and40; empowered action/outcome authority |029–032/036/053; which exchange classes require which observed effects and evidence, disputed/unknown closure and residual duties before affected build/conformance; no general success rule invented |
| ISS-006 direction resolved DEC094; schemas/applicability open |01/02/03/domain legal/contract steward with13/14; empowered authority |033–036; applicability/representation/ownership/lifecycle/conflict alternatives and approved exact profiles before affected commitments/obligations build |
| ISS-007 direction resolved DEC095; actual arrangements open |14 with01/03/04/05 and supplier/domain owners; Mark/empowered authority |010/011/026/047; approved actual party/control paths and general definition before dependent mixed-control build; hosting not a definition |
| ISS-008 commissioning dependencies open | Appointed14 owner with02/04/13/30/40 specialists |001–009/048–050;§3.1 eight dimensions, approved sources/jurisdictions/cadence/response/cover/rubrics/schema/access and actual evidence before dependent build/research activation/reliance; pilot5b remains open |
| Shared appointment/profile gate | Mark coordinates appointments; respective instrument approvers | All REQs; named accountable owners, valid versioned profiles, compatible wire/schema manifests, control/effect locations and isolated test fixtures before dependent build; no hidden numeric/schema/permission defaults |

# 18. Implementation Guidance — NON-NORMATIVE
Possible patterns include external policy gateways, policy-as-code, verifiable delegation credentials, cryptographic identity/provenance, outbound disclosure controls, action receipts, idempotent exchange, reconciliation workflows, federated trust frameworks, obligation metadata, event provenance and boundary anomaly monitoring. These are possibilities, not requirements. AOS-14 prescribes no model, gateway, firewall, service mesh, API architecture, identity protocol, credential format, database, cloud platform or supplier. AOS-14 is a responsibility boundary, not necessarily a software service.

## 18.1 Worked supplier example — contractor work exchange

An existing repairs platform holds the controlled 10 work/promise evidence and realises 13's workflow. Its connector or integration service contributes14 exchange recognition, request/determination and provenance. An external contractor portal may provide task acceptance, progress and inspection/work evidence. Existing supplier software remains part of the architecture; it need not become a raw-data feed.

1. The service proposes an exact contractor instruction and permitted content.01 supplies current delegated authority;03 identity/use and recipient restrictions;04 bounded task meaning;05 final runtime and applicable cumulative-account checks.14 assesses the external destination, exchange purpose and conditions. The platform's ability to submit an order is not permission to commit expenditure or change a resident promise.
2. The permitted route dispatches under the exact approved profile and records02 exchange evidence. Contractor receipt/acceptance and observed external effect retain their actual standing. If the external action may have occurred but its response is lost,13/14 coordinate authorised observation and reconciliation before a freshly checked retry. An “HTTP success”, “accepted” or “closed” flag alone does not prove completion of physical work. The example does not select HTTP or settle ISS-005's general outcome rule.
3. Contractor work/inspection evidence is admitted with provenance, assurance and uncertainty, then assessed under 10's repair-specific completion rule. Partial or disputed work remains explicit.13 tracks an empowered 30 human owner and residual duties;11 arranges any required resident communication through agreed channels. Contractual/exchange obligations retain approved owners and lifecycle. Supplier commercial convenience cannot change these meanings.
4. Actual permitted work outcome, communication standing, human disposition and residual obligation return to the controlled records and process. Boundary analytics may report repeated indeterminate exchanges or excessive restriction, within approved scope;25/qualified humans review implications. A successful transmission does not close a repair or establish institutional compliance.

The case platform, portal, connector, analytics and resident interface may come from one supplier or several. The implementation allocation identifies source/case masters, control locations and evidence at each handoff. This is an explanatory mapping, not a supplier selection, endorsement or executed conformance result.

# 19. Traceability and Change
Intended chain: **Foundational/Reasoning Principle → AOS-00 decision → AOS-14 capability → function → contract/state/invariant → conformance criterion → AOS-40 acceptance evidence**. The proposed v0.6 chain adds individually numbered REQ and planned VER links in §§4.6/15.5/19.2 and Appendix A. Source sufficiency, exact scoped approvals, unresolved material decisions and independently assessed handover remain required before build. The Research Custodian may **observe → analyse → challenge → propose**, but may not amend or approve this specification. Any change candidate identifies affected element/version, evidence, smallest proposed change, alternatives, cross-AOS implications, risks, confidence and required decision authority.

### 19.1 External-research traceability and current adoption

DEC-086 / AOS-00 REQ-050–054 and VER-023–025 → AOS-14-CAP-009/FUN-010/CON-005 → new REQ-001–008 → VER-001–006; exact row links in §§4.4/15.3. AOS-04 v0.8 §§3.1/5.1/6.6/10.8 (CON-009), AOS-02 v0.8 §6.6 (CON-007) and AOS-01 v0.8 §§6.6/10.8; Register v0.5 §13 and source matrix v0.7 §11 record reciprocal logical adoption. FP/RP/GT motivations retain their existing controlled versions; DEC-086 is Mark’s approved architectural direction, not a new standards-derived mandate. No existing approvals, REQs, VERs, IFs or source histories are retired/promoted.

### 19.2 Retained obligation migration and reciprocal traceability

Original functions/invariants/criteria remain derivation anchors, not competing unnamed requirement sets. Every new REQ is linked forward to exact planned cases;§15.5 lists reverse REQs. Research/supplier links remain001/007→VER001,002→002,003→003,004/008→004,005→005,006→006,009→007. Exact state transitions and data/control meanings are in§§5–6. Source links are all interpretations/contributions with residual scope, not promotion of old matrix statuses.

| Original anchor | Migrated REQ coverage | Observable state/contract / planned VER |
| --- | --- | --- |
| CAP001/FUN001 |010–013/026 | CON001; Proposed/Assessed;008/009/015 |
| CAP002/FUN002 |014–017/023/052 | CON002/003; typed admission;009/010/013/030 |
| CAP003/FUN003 |018/019/039/042 | CON001/002; final permitted scope;011/023/024 |
| CAP004/FUN004 |020–022/024/025/027/055 | CON002; Pending→effect current checks;012/014/016/033 |
| CAP005/FUN005 |033–035 | CON004; accepted duty/stages;020/021 |
| CAP006/FUN006/007 |028–032/036/040/041/050/051/053/054 | CON003; dispatch/effect/closure distinct;017–019/021/023/024/029–032 |
| CAP007/FUN008 |047 with010/013/020/033 | CON001–004; federation excluded pending decision;027 |
| CAP008/FUN009 |037/038/043–049 | CON003/002; bounded risk/referral/evaluation;022/025–028 |
| CAP009/FUN010 |001–008 | CON005/RSVIEW-0.1;001–006 unchanged |
| INV001/002/003; CR002/005 |020–022/026/047 | CON002; withheld invalid authority;012/015/027 |
| INV004; CR003 |014/017 | CON003; admission≠truth;009/010 |
| INV005; CR006 |028/050–052 | CON003; reconstruct exact attempts;017/029/030 |
| INV006/007; CR010 |021/022/026/027/039/041/047/055 | Shared01/03/04/05 remain owners;012/015/016/023/024/027/033 |
| INV008; CR008 |029–032/036 | CON003; unknown not success;018/019/021 |
| CR001 |010–012 | CON001/classification008 |
| CR004 |018/019/022/039 | CON002/outbound;011/012/023 |
| CR007 |024/025 | Pending/reassessment014 |
| CR009 |026/055 | Real effect boundary;015/033 |

### 19.3 Template coverage and controlled baselines

The retained21-section layout is mapped to AOS-QS Appendix A: purpose/context1–3; authority/sources2/8/AppendixA; requirements4/14 and19.2; data/interfaces6/9/12; behaviour5/7/10; qualities8/9/12/13 plusREQ043–052; failure11 andVER008–034; verification15; dependencies/issues16–17; build/handover18/20; review/control19/21. This is a section mapping, not an approved QS tailoring exception. Current opening baseline controls dated historical notes. Exact scoped build manifests must fix compatible revisions; v0.6 does not inherit old approval or assert approval of proposed shared schemas.

# Component Summary
**Purpose:** Govern intelligent exchange across the organisation's external boundary.  
**Owns:** Inbound/outbound external exchange, external commitments, boundary-specific obligations, provenance and exchange-state sensing.  
**Does not own:** Systemwide authority, identity/access, agent lifecycle, runtime containment, internal workflow or human Mode 2 judgement.  
**Receives:** Proposed exchanges, external material, identity/authority determinations, permitted-use conditions, organisational context and execution evidence.  
**Produces:** Exchange determinations, constraints, obligations, provenance, escalation, pattern signals and outcome evidence.  
**Key states:** Proposed → Assessed → Authorised/Constrained/Denied/Unresolved → Pending → Dispatched → Outcome Pending → Confirmed/Failed/Partial/Indeterminate → Closed.  
**Depends upon:** AOS-01/02/03/04/05, relevant sensing/GI components, AOS-30 and AOS-40.  
**Reserved human authority:** Mode 2 judgement, constitutional interpretation, exceptional authority and unresolved legitimate-value conflicts.  
**Conformant when:** Consequential external exchange is governed by legitimate purpose and authority, obligations and uncertainty remain visible, exchange remains reconstructable, and AOS-14 remains subject to shared controls.  
**Open issues:** Deferred federation and exact commissioning remain gated; general cumulative allocation, consequentiality, outcome-specific evidence, common obligations and operation-specific perimeter directions are resolved by DEC092–096. Working Boundary naming is resolved under OQ-013.


**Historical research amendment, 6 October 2026:** AOS-14 v0.3; AOS-00/Map v0.22, DEC-001–086; AOS-01–05 v0.7; AOS-14 v0.3; AOS-20 v0.2; Shared v0.6/Core v0.5/Register v0.5; source matrix v0.7; template v0.4. 8 additional proposed REQs/6 planned VERs. Current totals 8 proposed REQs/6 planned VERs; these count only new research records, not the older Boundary conformance criteria or full template migration. Author document checks only; no live research, delivery, independent review or readiness evidence. Earlier dated counts and next-step notes remain historical; AOS-30 functional work is complete and current next work follows the to-do list.

## AOS-30 decision-status disclosure alignment — 7 October 2026

Under DEC-103 and current AOS-30 §§5/6.2/10.3, decision validity/effective time, record authentication/evidence, minutes approval and permission to execute are distinct. Reliance uses sufficient attributable evidence assessed under the actual organisation’s legal form, instruments and approved evidence policy; a valid decision may precede minutes approval. A Chair-authenticated record or extract may be evidence through an authorised route, but no signature, draft or extract alone creates decision authority or resolves conflicting evidence. No universal second approval of exact decision wording is imposed where applicable arrangements do not require it. Minute-taker drafting and Company Secretary stewardship remain distinct; non-board decisions use their applicable empowered route. Current authority/data-use/conditions and observed effects remain separate. Missing or disputed sufficient evidence blocks affected automated reliance for accountable resolution, not a declaration of legal invalidity. External projections preserve supplied exact approval status and permitted source revision; disclosure permission cannot upgrade a draft or certify a decision. No automation or exchange power is changed.

# 20. Supplier handover and response matrix

Before dependent build/activation, supplier and AOS owners agree exact product/configuration and supported scope; organisation/party/control boundaries; authoritative records and mappings; identity/authority/use and final control locations; view/schema/source versions; units/time/currentness; acknowledgements/ordering/duplicates/retries and effect observation; commitments/obligations; human owner/cover/capacity and permitted channels; access/licensing/correction/deletion/retention/recovery; failure/manual continuity; configuration/provider changes and exit/revocation. Values and mechanisms are commissioned profiles, not defaults supplied by this revision. Existing ISS-001–008 and shared controls retain their standing.

Complete each row with product/version and direct, configured, integrated or outside-scope contribution. Replace “not assessed” only with accepted scoped evidence. Identify gaps, responsible parties and affected build/activation gates. Outside supplier scope requires another named party or authorised release exclusion without waiving governing duties. REQ rows are exact; the older Boundary functional/criterion allocation is separately required below because full migration to numbered requirements is still open.

| Exact requirement | Supplier product/version and contribution | Status | Evidence / gap / responsible party / gate |
| --- | --- | --- | --- |
| AOS-14-REQ-001 — Controlled research profile | Supplier to complete | Not assessed | Supplier/AOS owner to complete before affected build/activation |
| AOS-14-REQ-002 — Current permitted research access | Supplier to complete | Not assessed | Supplier/AOS owner to complete before affected build/activation |
| AOS-14-REQ-003 — Common research records/source standing | Supplier to complete | Not assessed | Supplier/AOS owner to complete before affected build/activation |
| AOS-14-REQ-004 — Shared retrieval and correction duties | Supplier to complete | Not assessed | Supplier/AOS owner to complete before affected build/activation |
| AOS-14-REQ-005 — Accepted review and separate amendment | Supplier to complete | Not assessed | Supplier/AOS owner to complete before affected build/activation |
| AOS-14-REQ-006 — Research evaluation | Supplier to complete | Not assessed | Supplier/AOS owner to complete before affected build/activation |
| AOS-14-REQ-007 — Owned gaps and failed coverage | Supplier to complete | Not assessed | Supplier/AOS owner to complete before affected build/activation |
| AOS-14-REQ-008 — Retrieval versus specialist ownership | Supplier to complete | Not assessed | Supplier/AOS owner to complete before affected build/activation |
| AOS-14-REQ-009 — Supplier allocation and evidence | Supplier to complete | Not assessed | Supplier/AOS owner to complete before affected build/activation |

| Older Boundary obligation allocation | Supplier contribution to declare | Evidence / remaining dependency |
| --- | --- | --- |
| CAP-001/FUN-001/INV-001/007/CR-001/009 | Recognition and declared control perimeter | Exact exchange scope, organisational boundary, actual paths/bypass prevention; ISS-004/007 |
| CAP-002/003/FUN-002/003/CON-001/002/INV-003/004/CR-003/004 | Inbound admission and outbound disclosure | Source/recipient/purpose/permission/uncertainty, observed constraints and receiving-domain meaning |
| CAP-004/FUN-004/INV-002/006/CR-002/005/007/010 | Current commitment controls | Shared authority and final runtime checks; queued changes/denial/bypass evidence |
| CAP-005/FUN-005/CON-004 | Exchange obligations | Exact obligation applicability, owners, records/lifecycle/incident routes; ISS-006 |
| CAP-006/FUN-006/007/CON-003/INV-005/008/CR-006/008 | Provenance and outcome reconciliation | Actual dispatch/effect/unknown/partial/duplicate standing and authorised follow-up; ISS-005 |
| CAP-007/FUN-008 | Federated exchange | Agreed identity/authority/provenance/obligation/incident semantics; ISS-001/007 |
| CAP-008/FUN-009 | Boundary analytics/oversight contribution | Permitted population/coverage/cumulative signals, uncertainty and accepted follow-up; ISS-003/25 boundary |
| CAP-009/FUN-010/CON-005 | Own research and shared collection | Exact REQ-001–008 / VER-001–006 evidence; distinct specialist/reviewer duties |

Apply relevant data/privacy, security, state, failure and evidence duties in §§5–14 across these rows; do not interpret this summary as an exhaustive substitute for the specification. Current v0.6 §§4.6/15.5/19.2 and Appendix A resolve functional migration; substantive source sufficiency and approved scoped profiles remain gates. Supplier evidence supports item 12a's later cross-AOS briefing; it does not close that separate deliverable or authorise procurement.

# 21. Review and findings

## 21.0 Historical supplier revision assessment — 8 October 2026

The supplier additions preserve every prior REQ/VER row, CAP/FUN/CON/INV/CR/ISS identifier and existing issue disposition. Author checks cover exact new requirement/case allocation, table structure, supplier responsibility mappings, deployment arrangements, worked source-to-effect-to-service-outcome example and response rows. No supplier response, execution, research run, independent review, legal validation or operating approval has occurred.

Functional fit is now explained across all five sensing specifications. Next session: author review of AOS-10–14 together for consistent responsibilities, information exchanges, behaviour and source allocation against the common infrastructure. This remains separate from deferred independent project review and from actual commissioned/executed conformance. Full Boundary requirement/template migration and its existing open issues remain visible work; this focused revision does not claim to complete them.


## 20.1 Complete supplier response and stop conditions — 9 October

The supplier response population is all55 requirements, each addressed by its exact ID, statement and linked cases in§§4.4–4.6/15.3–15.5. Each response records product/configuration/route; supported/excluded scope; authoritative record/control/human owner; actual producer/consumer and control location; exact compatible profiles/schema/case revisions; observed evidence or owned gap; remediation/gate and change/exit impact. A group response is acceptable only if it retains each requirement's distinct acceptance condition and status. Older response rows remain historical initial allocations; they cannot omit010–055. Missing material authority/perimeter/effect/obligation or schema decisions stop dependent build and return an owned gap. Suppliers retain implementation discretion over transport/storage/integration mechanism within the approved logical contracts; they cannot choose organisational authority, purpose, evidence sufficiency or human adjudication. Combined/manual arrangements undergo the same scope/control walkthrough.

| Requirement / subject | Supplier implementation and owner | Evidence / standing | Owned gap / gate |
| --- | --- | --- | --- |
| AOS-14-REQ-010 — Declared control perimeter | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 008 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-011 — Exchange recognition | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 008/034 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-012 — Consequentiality uncertainty | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 008 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-013 — External identity standing | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 009 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-014 — Source standing | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 009 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-015 — Typed determination | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 010 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-016 — Constrained execution | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 010 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-017 — Admission is not truth | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 010/034 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-018 — Exact disclosure scope | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 011 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-019 — Recipient channel | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 011/034 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-020 — Exact commitment authority | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 012/034 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-021 — No permissive fallback | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 012 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-022 — Final current check | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 012 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-023 — Untrusted instructions | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 013 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-024 — Selective change reassessment | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 014 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-025 — Late control events | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 014 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-026 — Bypass resistance | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 015 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-027 — Shared cumulative account | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 016 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-028 — Attempt identity | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 017 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-029 — Outcome evidence scope | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 018/034 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-030 — Unknown actual effect | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 018/034 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-031 — Retry after reconciliation | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 019 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-032 — Separate compensation authority | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 019 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-033 — Obligation standing | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 020 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-034 — Accepted obligation owner | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 020 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-035 — Staged acknowledgement | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 021/034 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-036 — Closure with residual duty | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 021/034 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-037 — Internal referral distinction | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 022/034 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-038 — Protected reporting route | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 022 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-039 — Purpose-limited exchange | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 023 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-040 — Data lifecycle propagation | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 023 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-041 — Restore current standing | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 024 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-042 — Incident communication authority | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 024 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-043 — Intrinsic boundary risk | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 025 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-044 — Declared coverage | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 025 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-045 — Excessive restriction | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 025 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-046 — Oversight feedback | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 026 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-047 — Federation deferred | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 027 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-048 — Probabilistic quality evaluation | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 028 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-049 — Model/configuration change | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 028 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-050 — Common view compatibility | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 029 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-051 — Reconstructable audit | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 030 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-052 — Meaningful explanation | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 030 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-053 — Domain and human status fidelity | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 031/034 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-054 — Supplier exit portability | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 032 | Supplier/AOS owner to identify and resolve before affected build/activation |
| AOS-14-REQ-055 — Governed manual continuity | Supplier/AOS owner to complete for exact commissioned scope | Not assessed; planned VER 033 | Supplier/AOS owner to identify and resolve before affected build/activation |

## 21.1 Functional-completion author review — 9 October

**Quality assessment:** author review by Codex against the preserved baseline, requirement/case links, all retained anchors and80 source contributions. Identifier preservation and declared reciprocal coverage checked; all55 REQs have statements, inherited complete attributes or explicit blocking records and planned VER links;34 cases are planned. Original research/supplier statements/cases and8 invariants/10 criteria retained. Typed mapping resolves the local vocabulary ambiguity; working naming corrected from existing OQ-013 disposition. Interfaces now give explicit logical duties and mandatory commissioning fields. Concrete schemas, approved profiles, appointed owners, independent human review and scoped approvals remain visible dependencies, so no unconditional G2/G3 or whole-document conformance assertion is made.

**Design adequacy:** functional responsibility allocation and no-self-authority/uncertainty/actual-duty boundaries are coherent in the author walkthrough. General ISS003–007 decisions and deferred federation cannot be settled by engineering prose; full design adequacy remains not independently assessed. Normal contractor exchange, invalid authority/bypass, recovery and assembled overdue-repair exceptions are planned; none executed. Model relevance/fidelity, protected reporting effectiveness, actual legal applicability, resident burden, board independence and longitudinal outcomes remain unverified. No external standards or legal source was freshly validated for this completion.

**Finding disposition:** SENS-CR-01 core migration and SENS-CR-05 typed logical mapping corrected at functional-document level, subject to substantive review; SENS-CR-02/03 receive Boundary-only adoption/source addenda and remain open for other domains/whole-suite sufficiency; SENS-CR-04 Boundary naming/conformance/current-versus-history corrections complete locally, other components' obsolete passages remain open. Author closure is not independent assurance. The scheduled research pilot remains a separate open operational item.

**Required next review:** Mark and appointed relevant semantic/domain/control owners review the new proposed obligations and retained decisions; an independent competent reviewer checks quality and design separately and walks normal/exception/authority cases from the exact approved package beforeG3. Record reviewer, evidence, findings and approvals; a drafting completion request confers no operating permission.

# Appendix A — Complete source applicability and reverse contribution links

Controlled sources are FP v4, RP v6 and Governance Intelligence Tests as preserved by the source manifest/matrix. FP uses source numbers/titles; RP uses the matrix's domain and opening phrase because the source has no individual principle IDs (row numbers here are local indexes); GT retains exact test titles. RP excerpts already truncated in the controlled matrix remain locators, not substitute principle texts. Full source propositions govern interpretation. All80 are considered below. Each link is a proposed **Boundary contribution/interpretation**, with forward REQ/case records in§§4/15; it does not adopt the entire institutional proposition or promote historical Source Matrix statuses. All GT institutional results remain **not assessed**. Scope/legal fulfilment, humans and outcomes require competent actual evidence.

| FP v4 source locator | Boundary contribution | Residual owner / limit |
| --- | --- | --- |
| 1 Telos/conferred purpose/function | REQ-010/018/039 → VER-008/011/023 | Humans/01/20 confer and adjudicate purpose; exchange profile does not supply telos |
| 2 Permanently human Mode 2 | REQ-020/037/053 → VER-012/022/031/034 | Humans/30 retain genuine Mode2 judgement; technical checks cannot certify it |
| 3 Architectural integrity | REQ-021/022/026/027 → VER-012/015/016 | 01/03/04/05 own independent systemwide enforcement;40 assembled assurance |
| 4 Radical transparency | REQ-051/052 → VER-030 | 02 permitted custody and actual human access/reconstructability; no unrestricted disclosure |
| 5 Bounded rationality/imperfection | REQ-012/030/044/055 → VER-008/018/025/033/034 | Novel perimeter/mixed-control questions remain ISS004/007; real fallback must be demonstrated |
| 6 Epistemic humility | REQ-014/017/030/048 → VER-009/010/018/028/034 | Human challenge and evidence fidelity still evaluated; admission cannot establish truth |
| 7 No-exit obligation | REQ-019/038/045/055 → VER-011/022/025/033/034 | 11/30 actual resident/worker burden and accessible alternatives; no proxy legitimacy |
| 8 Constitutional mediator | REQ-020/037/046 → VER-012/022/026/034 | 01/20/30 constitutional mediation and legitimate conflict resolution remain human |
| 9 Compliance as consequence | REQ-033/043/053 → VER-020/025/031/034 | Competent jurisdiction/contract/legal owners assess real applicability; no legal conformance claim |
| 10 Complexity/emergence | REQ-027/043/044/046 → VER-016/025/026 | 25/40 cross-system and longitudinal assessment; locally assured parts do not establish whole |

| RP local row / v6 domain and opening locator | Boundary contribution | Residual owner / limit |
| --- | --- | --- |
| 1: Architecture and Completeness: Every governance process must close its feedback loop. | REQ-029/030/036/046 → VER-018/021/026/034 | 13/30 real outcome and accepted feedback, not dispatch |
| 2: Architecture and Completeness: Every human accountability layer must be explicitly named, sequenced, and time - bounded before any process is consid... | REQ-034/035/037 → VER-020/021/022/034 | 13/30 appointed people/windows/capacity must be demonstrated |
| 3: Architecture and Completeness: Every option set must include the option that cannot be made to work. | REQ-030/045/046 → VER-018/025/026/034 | 22/30 complete real option set; Boundary preserves constraint evidence only |
| 4: Architecture and Completeness: The ‘AI said so’ test must be passable at every decision point. | REQ-020/053 → VER-012/031/034 | 30 human rationale and judgement; model output/signature insufficient |
| 5: The Mode 1 / Mode 2 Boundary: Mode 2 is permanently human. | REQ-020/037/053 → VER-012/022/031/034 | Permanent human Mode2 judgement |
| 6: The Mode 1 / Mode 2 Boundary: Every Mode 1 boundary is a governance instrument, not a technical setting. | REQ-010/012/020 → VER-008/012/034 | 01/30 approved board governance instrument; no thresholds invented |
| 7: The Mode 1 / Mode 2 Boundary: The boardroom is a Mode 2 deliberative space. | REQ-039/053 → VER-023/031/034 | 30 protected deliberation; no boardroom capture or automatic decision |
| 8: The Mode 1 / Mode 2 Boundary: The Mode 1/Mode 2 boundary is under continuous pressure from AI capability growth. | REQ-001/005/049 → VER-001/005/028 | 25/30 capability pressure review; research cannot reclassify Mode2 |
| 9: The 1+5 Architecture: Every proposed governance mechanism must be tested against the 1+5 structure to confirm which layer it belongs to and... | REQ-010/026/047 → VER-008/015/027 | DEC005/01–05/20–25 retain layered responsibilities |
| 10: The 1+5 Architecture: Risk is intrinsic to each intelligence layer, not a separate domain. | REQ-043/044 → VER-025 | ISS003 exact pattern allocation remains open;25 aggregate risk |
| 11: The 1+5 Architecture: Every intelligence layer boundary where welfare - adjacent or safety - adjacent signals may arise must have an explic... | REQ-034/037/038 → VER-020/022/034 | 13/30 independent permitted welfare/safety audience and cover |
| 12: The 1+5 Architecture: The Golden Thread obligation under the Building Safety Act 2022 is not a technical data management requirement. | REQ-014/051/053 → VER-009/030/031/034 | 10/02 custody, statutory dutyholders and board accountability are distinct; legal scope not verified |
| 13: Options and Decisions: Options generated by the architecture must be grounded in the organisation’s actual state — actual covenant condition... | REQ-014/030/043 → VER-009/018/025/034 | 22/30 actual options and constraints, not Boundary optimisation |
| 14: Options and Decisions: Every consequential decision must feed back into the Unified Data Layer as a structured record — not only the decisio... | REQ-036/046/053 → VER-021/026/031/034 | 02/30 exact human-provided decision context; no inferred deliberation |
| 15: Options and Decisions: Revealed preferences from real decisions take precedence over stated preferences in policy documents when the archite... | REQ-046/053 → VER-026/031/034 | 25/30 descriptive preference is not calibration authority; DEC018 retained |
| 16: Blind Spots and Honesty: The architecture must name what it cannot see. | REQ-044/052 → VER-025/030 | 25/board unknown perimeter and blind spots beyond declared coverage |
| 17: Blind Spots and Honesty: The dynamic risk perimeter question must be asked at board level as a standing agenda item: not only ‘what are our ri... | REQ-043/044/046 → VER-025/026 | 25/30 board standing-agenda and actual challenge not software case |
| 18: Blind Spots and Honesty: The interaction of intelligence layers produces system - level behaviours that no individual layer would produce alone. | REQ-027/046 → VER-016/026 | 25/40 longitudinal compound effects and human judgement |
| 19: Ethics and Telos: Every process must demonstrate a traceable relationship to the organisation’s ethical commitments and social purpose. | REQ-010/018/039 → VER-008/011/023 | 01/20 purpose/ethics adjudication independent of procedural authority |
| 20: Ethics and Telos: The architecture must be capable of detecting purpose drift — the condition where operational processes have graduall... | REQ-043/046 → VER-025/026 | 25/humans assess purpose drift from actual consequences |
| 21: Ethics and Telos: Diversity, inclusion, and equitable outcomes are not separate compliance obligations. | REQ-019/045/055 → VER-011/025/033/034 | 11/12/30 real equitable experience and remedy, not notification metrics |
| 22: Ethics and Telos: Where the organisation’s welfare obligation to residents and its consent architecture pull in opposing directions, th... | REQ-020/021/037/039 → VER-012/022/023/034 | 01/03/11/30 legitimate welfare-consent conflict resolution; no emergency power invented |
| 23: Ethics and Telos: AI systems have function, not telos. | REQ-010/020/046 → VER-008/012/026/034 | Humans confer telos; component has assigned function |
| 24: Ethics and Telos: Where the organisation's purpose is interpreted through an accumulating body of AI-mediated rulings rather than appli... | REQ-020/046/053 → VER-012/026/031/034 | 01/20/25/30 no precedent or purpose amendment from exchange memory |
| 25: Ethics and Telos: Every AI system deployed by the organisation carries an embedded constitutional framework established by its developer. | REQ-009/048/049 → VER-007/028 | 25/shared owners assess developer constitutional framework; supplier statement insufficient |
| 26: Ethics and Telos: The no - exit condition is a constitutive feature of the organisation’s moral architecture, not background context. | REQ-019/045/055 → VER-011/025/033/034 | 11/12/30 actual no-exit burden and legitimacy over time |
| 27: Ethics and Telos: Compliance is the output of sound governance design, not its objective. | REQ-033/043/053 → VER-020/025/031/034 | Purpose-led governance and competent legal/practice evidence |
| 28: Radical Transparency: If you cannot audit it and be held accountable for it, it cannot be done. | REQ-051 → VER-030 | Actual reconstructability by permitted assessor; no private chain-of-thought demanded |
| 29: Radical Transparency: The architecture must be more transparent than the document - based governance it replaces, not less. | REQ-051/052 → VER-030 | Comparison to prior document governance must be empirically assessed |
| 30: Radical Transparency: Transparency obligations extend to the architecture’s uncertainty. | REQ-014/030/044 → VER-009/018/025/034 | Recipient comprehension and fidelity require actual assessment |
| 31: Agentic Delegation: Agents operate under explicitly delegated authority, not implied authority. | REQ-020/021/022 → VER-012/034 | 01 delegated instrument and05 enforcement retain authority |
| 32: Agentic Delegation: Agent authority is domain - specific, context - specific, and condition - specific simultaneously. | REQ-015/018/020/022 → VER-010/011/012/034 | 01/03/04/05 current exact-operation controls remain independent |
| 33: Agentic Delegation: Agents cannot commit the organisation to external obligations, initiate unsolicited contact with external parties, or... | REQ-020/021/022 → VER-012/034 | 01 exact authority for external commitments/unsolicited contact; no model grant |
| 34: Agentic Delegation: Internal escalation — routing a signal within the architecture to a human reviewer or to a receiving intelligence lay... | REQ-037/038 → VER-022/034 | Permitted internal referral has separate authority from external contact |
| 35: Agentic Delegation: The agentic delegation framework is a governance document reviewed by the board, not a technical configuration manage... | REQ-010/020/047 → VER-008/012/027/034 | Board/01/30 delegation instrument review is substantive human duty |
| 36: Agentic Delegation: Every agent action must satisfy the ethics and telos test and the radical transparency test independently of the proc... | REQ-010/020/051 → VER-008/012/030/034 | 01/20/30 separate ethics/telos and transparency tests not replaced by procedural permission |
| 37: Agentic Delegation: Certain classes of finding must reach their required audience regardless of any instruction to suppress or delay them. | REQ-038 → VER-022 | Common protected-reporting independent audience and actual delivery evidence |
| 38: Data and Sensing Boundaries: Sensing must not exceed its declared purpose. | REQ-039/040 → VER-023 | 03 owns data purpose, inference, use and restriction |
| 39: Data and Sensing Boundaries: The boundary between observing an asset and monitoring a behaviour is an absolute architectural boundary, not a matte... | REQ-039/053 → VER-023/031/034 | 10/11 absolute physical-observation/behavioural-monitoring boundary remains |
| 40: Data and Sensing Boundaries: Where behavioural inference from sensing data is genuinely necessary to serve the resident’s interests — energy pover... | REQ-021/037/039 → VER-012/022/023/034 | Any separate behavioural-inference proposal requires necessity, express governed scope/consent/review; none activated here |
| 41: Data and Sensing Boundaries: The purpose limitation principle applies across all intelligence layers, not only to resident - facing sensing. | REQ-018/039/040 → VER-011/023 | 03 purpose limits across all layers/products and derived uses |

| GT controlled test | Boundary supporting contribution | Institutional result / residual assessment |
| --- | --- | --- |
| M1.1 Strategic Coherence | REQ-010/043/046 → VER-008/025/026 | Not assessed — Actual strategy and conferred purpose coherence |
| M1.2 Sensing Architecture | REQ-011/014/044 → VER-008/009/025/034 | Not assessed — Whole declared sensing perimeter and actual blind spots |
| M1.3 Risk Intelligence | REQ-033/043/045 → VER-020/025 | Not assessed — Risk culture, human ownership and changing perimeter |
| M1.4 Composition and Capability | REQ-034/035/048/055 → VER-020/021/028/033/034 | Not assessed — Board/staff competence, composition and actual capacity |
| M1.5 Performance Legibility | REQ-029/030/036/053 → VER-018/021/031/034 | Not assessed — Actual service/physical outcomes and human comprehension |
| M1.6 Compliance Assurance | REQ-014/033/048 → VER-009/020/028 | Not assessed — Competent legal/standards fulfilment in practice |
| M1.7 Governance Documentation | REQ-040/050/051 → VER-023/029/030 | Not assessed — Usable governed institutional records, not document count |
| M1.8 Accountability Architecture | REQ-034/035/037/038 → VER-020/021/022/034 | Not assessed — Empowered accepted duties and real challenge effectiveness |
| M1.9 Value for Money | REQ-043/045/054 → VER-025/032 | Not assessed — Real costs/burdens/alternatives and social value |
| M1.10 Human-AI Interaction Norms | REQ-020/037/052/055 → VER-012/022/030/033/034 | Not assessed — Substantive human judgement and lived interaction |
| M1.11 Learning Metabolism | REQ-029/036/046 → VER-018/021/026/034 | Not assessed — Real consequences and learning over time |
| M1.12 Continuous Self-Assessment | REQ-001/006/044/048 → VER-001/006/025/028 | Not assessed — Independent ongoing review and false/missed findings |
| M1.13 Emergent System Behaviour | REQ-027/030/046 → VER-016/018/026/034 | Not assessed — Cross-system/longitudinal emergence, not assured parts |
| M1.14 Golden Thread Integrity | REQ-014/051/053 → VER-009/030/031/034 | Not assessed — 10/domain dutyholders and board governance; statutory scope not assessed |
| M2.1 Values Architecture | REQ-010/038/039 → VER-008/022/023 | Not assessed — Human constitutional values and practice |
| M2.2 Coherence Under Pressure | REQ-021/030/038 → VER-012/018/022/034 | Not assessed — Human integrity under actual conflicting pressure |
| M2.3 Incommensurable Trade-off Capacity | REQ-020/037/045 → VER-012/022/025/034 | Not assessed — Human deliberation about incommensurable values |
| M2.4 Epistemic Brake Function | REQ-012/030/044 → VER-008/018/025/034 | Not assessed — Actual willingness and capacity to stop/challenge uncertainty |
| M2.5 Directorial Independence | REQ-038/046/053 → VER-022/026/031/034 | Not assessed — Genuine directorial independence and unfiltered evidence |
| M2.6 Social Legitimacy | REQ-019/045/052/055 → VER-011/025/030/033/034 | Not assessed — Resident/worker legitimacy and actual remedy |
| M2.7 No-Exit Obligation | REQ-019/039/045/055 → VER-011/023/025/033/034 | Not assessed — Constitutive no-exit burden and accessible human alternatives |
| M2.8 Radical Transparency | REQ-014/030/051/052 → VER-009/018/030/034 | Not assessed — Actual permitted accountability and comparative transparency |
| M2.9 Moral Drift Detection | REQ-043/044/046 → VER-025/026 | Not assessed — 25/board purpose/moral drift over time |
| M2.10 Purpose Stability | REQ-010/024/039/049 → VER-008/014/023/028 | Not assessed — 01/humans stable purpose despite capability/configuration change |
| M2.11 Murmuration Capacity | REQ-038/046/053 → VER-022/026/031/034 | Not assessed — Independent human sense-making, not aggregated model assent |
| M2.12 Constitutional Authority | REQ-020/021/047 → VER-012/027/034 | Not assessed — 01/30 empowered constitutional adjudication |
| M2.13 AI Constitutional Framework Governance | REQ-009/048/049 → VER-007/028 | Not assessed — 25/shared owners real developer-framework assessment |
| M2.14 Purpose-Led Design | REQ-009/010/039 → VER-007/008/023 | Not assessed — Human purpose-led design adequacy separate from formal quality |
| M2.15 Telos / Function Distinction | REQ-029/036/043/046 → VER-018/021/025/026/034 | Not assessed — Conferred human telos distinct from operational efficiency |

## 21.2 Approved-direction incorporation review — 9 October 2026


## Approved Boundary decision adoption — 9 October 2026

| Approved decision / subject | Direction / rationale | Affected Boundary records | Approval and standing |
| --- | --- | --- | --- | --- |
| AOS-00-DEC-092 — Consequential external exchange | An external exchange is consequential when it can create or change an organisational commitment, disclose protected information, affect rights or service, trigger external action, or create a material obligation or risk. Materiality considers financial exposure and resource impact separately: payments, expenditure, liabilities or contingent exposure; and staff time, workload, capacity, equipment, facilities or other resource commitments and displacement of existing duties. Low monetary cost does not establish low resource impact. Record known quantities with their units/time basis and uncertainty; no invented money-to-time conversion or universal threshold. Apply organisation-approved criteria, including cumulative commitments. Routine public-information retrieval may use a lighter approved route only where its actual purpose, content and effects meet that profile. Uncertain classification goes to an accountable reviewer and cannot silently use the lighter route. | ISS-004; REQ-010–012/020–022/027/051; VER-008/012/016 | Mark;9October2026; Q1 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-093 — Outcome-specific exchange evidence | Define the required outcome and sufficient evidence for each exchange type. Sending, delivery, recipient acceptance and actual fulfilment remain distinct facts. Contractor receipt does not prove completed work. Where the required effect remains unknown, retain that standing and reconcile before retrying. An authorised person may close further investigation under the approved profile only with an explicit unknown outcome and retained owner/status of every outstanding duty; closure cannot become confirmed success. | ISS-005; REQ-029–032/036/053; VER-018/019/021/031/034 | Mark;9October2026; Q2 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-094 — Common external-obligation ownership | Use a common obligation record carrying source, applicability, exchange, responsible human owner, deadline where applicable, fulfilment evidence and current status. Boundary recognises exchange-associated obligations; relevant domain stewards determine substantive meaning and applicability under their authority; AOS-02 owns common record semantics; AOS-13 tracks accepted responsibility and fulfilment; AOS-30 supports accountable human disposition. Preserve financial and resource impacts separately where applicable, including unknown values. Uncertain or conflicting obligations go to an empowered human; automated recognition does not create legal authority or settle substantive meaning. | ISS-006; REQ-033–036; VER-020/021 | Mark;9October2026; Q3 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-095 — Operation-specific organisational boundary | Determine the boundary from organisational authority and control over the particular operation and data use. Hosting location alone is insufficient. A supplier system may carry out a delegated internal function while its onward disclosure or independent action crosses the external boundary. Each arrangement declares controlling parties, authority, operation/data-use scope, actual governed exchange points and independent shared-control enforcement. Ambiguous or missing control allocation remains an owned gap and withholds dependent consequential action. | ISS-007; REQ-010/011/026/047; VER-008/015/027 | Mark;9October2026; Q4 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-096 — Boundary patterns and system oversight | Boundary detects cumulative external-exchange patterns, including repeated disclosures, accumulating commitments, unusual counterparties, excessive restriction and attempts to evade controls by splitting actions. AOS-25 combines permitted Boundary signals with other domains to assess wider drift and emerging/system risks. Shared AOS-01/03/04/05 controls enforce approved limits and accounting; empowered humans decide policy/limit changes. Boundary cannot create a private budget, waive restrictions or adjudicate systemwide governance. | ISS-003; REQ-027/043–046; VER-016/025/026 | Mark;9October2026; Q5 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |

These directions do not appoint organisational officers, select numerical thresholds, convert resource impact into money or certify external obligations legally. Shared owners retain their meanings and independent enforcement. Proposed component requirements and planned cases retain stable identities; an approved direction is distinct from G3/build or operating approval. The organisation-specific profile must state criteria and aggregation windows for financial and resource materiality; exchange-type expected effect/evidence and authorised unresolved closure; obligation field types/cardinalities/lifecycle and owners; operation/data-use authority and control points; and Boundary-versus25 pattern routing/triggers. Missing or invalid mandatory settings withhold dependent effects/reliance and retain an owned gap. No deferred federation activation or new source-status promotion is implied.

Author check: all55 REQ and34 VER identities/links retained; new five decision records map to affected existing records/cases; no old DEC changed. Current proposed requirement wording includes the financial/resource distinction and each approved principle. ISS003–007 no longer represent unanswered general design questions. Exact scoped schemas/parameters/appointments, implementation evidence and independent human quality/design assessment remain separate; no G3/G4 or operating approval. The earlierv0.6 self-review records its historical unresolved baseline.

## Current reciprocal adoption and precise source allocation — 9 October2026

This revision corrects current control/status and adoption/traceability references only. Every original normative requirement statement, case acceptance condition, invariant and identity retains its prior meaning. Existing source versions, approved architectural directions and human/private boundaries are unchanged. Local§6 is the authoritative domain view; Registerv0.17 SENSING-ADOPTION-2026-10-09 supplies the current reciprocal common mapping; Matrixv0.18 SENSING-SOURCES-2026-10-09 supplies every FP/RP/GT source locator, exact contribution chain and owned residual/gate. The following reverse view rows are projections of that single adoption manifest, not new dictionaries or wire schemas.

| Exact component/view revision | Authoritative common master | Retained producer → consumer / domain meaning | Local requirement → planned case | Exact40 supporting cases / residual gate |
| --- | --- | --- | --- | --- |
| AOS-14-CON-001 / documentv0.8 | KX-23/02/03/09/11/12;14-IF-001 request | Domain/04/13 or permitted external intake →14/requesting executor; organisation/party/direction/operation/purpose/profile and current authority/use | AOS-14-REQ-010, AOS-14-REQ-011, AOS-14-REQ-012, AOS-14-REQ-013, AOS-14-REQ-019, AOS-14-REQ-026, AOS-14-REQ-047 → AOS-14-VER-008, AOS-14-VER-009, AOS-14-VER-011, AOS-14-VER-015, AOS-14-VER-027, AOS-14-VER-034 | AOS-40-VER-024, AOS-40-VER-025; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-14-CON-002 / documentv0.8 | KX-23/02/03/11/14/24/25;14-IF-001 typed determination; CHECK | 14 consuming01/03/04/05 → executor/13/02; exact operation-bound Permit/Constrain/Deny/Quarantine/Escalate/Unresolved | AOS-14-REQ-015, AOS-14-REQ-016, AOS-14-REQ-018, AOS-14-REQ-020, AOS-14-REQ-021, AOS-14-REQ-022, AOS-14-REQ-024, AOS-14-REQ-025, AOS-14-REQ-027, AOS-14-REQ-037, AOS-14-REQ-039, AOS-14-REQ-042, AOS-14-REQ-052, AOS-14-REQ-055 → AOS-14-VER-010, AOS-14-VER-011, AOS-14-VER-012, AOS-14-VER-014, AOS-14-VER-016, AOS-14-VER-022, AOS-14-VER-023, AOS-14-VER-024, AOS-14-VER-030, AOS-14-VER-033, AOS-14-VER-034 | AOS-40-VER-014, AOS-40-VER-015, AOS-40-VER-020; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-14-CON-003 / documentv0.8 | KX-23/01/04/08/13/15/21;14-IF-001 evidence; REC-E/Q/X | 14/connector/04/05 and attributed domain/counterparty effect →02/permitted10–13/25/30/40; attempt/stages/outcome/uncertainty | AOS-14-REQ-014, AOS-14-REQ-017, AOS-14-REQ-023, AOS-14-REQ-028, AOS-14-REQ-029, AOS-14-REQ-030, AOS-14-REQ-031, AOS-14-REQ-032, AOS-14-REQ-036, AOS-14-REQ-038, AOS-14-REQ-040, AOS-14-REQ-041, AOS-14-REQ-043, AOS-14-REQ-044, AOS-14-REQ-045, AOS-14-REQ-046, AOS-14-REQ-048, AOS-14-REQ-049, AOS-14-REQ-050, AOS-14-REQ-051, AOS-14-REQ-053, AOS-14-REQ-054 → AOS-14-VER-009, AOS-14-VER-010, AOS-14-VER-013, AOS-14-VER-017, AOS-14-VER-018, AOS-14-VER-019, AOS-14-VER-021, AOS-14-VER-022, AOS-14-VER-023, AOS-14-VER-024, AOS-14-VER-025, AOS-14-VER-026, AOS-14-VER-028, AOS-14-VER-029, AOS-14-VER-030, AOS-14-VER-031, AOS-14-VER-032, AOS-14-VER-034 | AOS-40-VER-022, AOS-40-VER-023, AOS-40-VER-025, AOS-40-VER-036, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-14-CON-004 / documentv0.8 | KX-23/07/06/21/26;14-IF-001 obligation;13 tracking/02 common record | 14 recognised source with01/03/domain steward →02/13/30/empowered duty owner; common obligation and actual fulfilment | AOS-14-REQ-033, AOS-14-REQ-034, AOS-14-REQ-035 → AOS-14-VER-020, AOS-14-VER-021, AOS-14-VER-034 | AOS-40-VER-009, AOS-40-VER-021, AOS-40-VER-022, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-14-CON-005 / documentv0.8 | RSVIEW-0.1;02§6.6/04-CON-009; KX-23/07/06/05/13/17/21 | Assigned component research/14 retrieval →02/component reviewers/13/30/01; distinct specialist relevance and common research states | AOS-14-REQ-001, AOS-14-REQ-002, AOS-14-REQ-003, AOS-14-REQ-004, AOS-14-REQ-005, AOS-14-REQ-006, AOS-14-REQ-007, AOS-14-REQ-008 → AOS-14-VER-001, AOS-14-VER-002, AOS-14-VER-003, AOS-14-VER-004, AOS-14-VER-005, AOS-14-VER-006 | AOS-40-VER-031, AOS-40-VER-032, AOS-40-VER-033, AOS-40-VER-034, AOS-40-VER-035; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |

### Individual-source reverse navigation

Rows below identify the exact controlled source locator and this component’s selected contribution or owned residual. Full source propositions and all other counterparts remain in the Matrix addendum; row numbers do not invent source IDs. This record completes source disposition, not source sufficiency or institutional assessment.

| Source locator | Selected component chain / residual disposition |
| --- | --- |
| FP 1 Telos/conferred purpose/function | AOS-14-REQ-010, AOS-14-REQ-018, AOS-14-REQ-039 → AOS-14-VER-008, AOS-14-VER-011, AOS-14-VER-023; Matrix source row retains owned residual and gate |
| FP 2 Permanently human Mode 2 | AOS-14-REQ-020, AOS-14-REQ-037, AOS-14-REQ-053 → AOS-14-VER-012, AOS-14-VER-022, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| FP 3 Architectural integrity | AOS-14-REQ-021, AOS-14-REQ-022, AOS-14-REQ-026, AOS-14-REQ-027 → AOS-14-VER-012, AOS-14-VER-015, AOS-14-VER-016; Matrix source row retains owned residual and gate |
| FP 4 Radical transparency | AOS-14-REQ-051, AOS-14-REQ-052 → AOS-14-VER-030; Matrix source row retains owned residual and gate |
| FP 5 Bounded rationality/imperfection | AOS-14-REQ-012, AOS-14-REQ-030, AOS-14-REQ-044, AOS-14-REQ-055 → AOS-14-VER-008, AOS-14-VER-018, AOS-14-VER-025, AOS-14-VER-033, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| FP 6 Epistemic humility | AOS-14-REQ-014, AOS-14-REQ-017, AOS-14-REQ-030, AOS-14-REQ-048 → AOS-14-VER-009, AOS-14-VER-010, AOS-14-VER-018, AOS-14-VER-028, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| FP 7 No-exit obligation | AOS-14-REQ-019, AOS-14-REQ-038, AOS-14-REQ-045, AOS-14-REQ-055 → AOS-14-VER-011, AOS-14-VER-022, AOS-14-VER-025, AOS-14-VER-033, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| FP 8 Constitutional mediator | AOS-14-REQ-020, AOS-14-REQ-037, AOS-14-REQ-046 → AOS-14-VER-012, AOS-14-VER-022, AOS-14-VER-026, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| FP 9 Compliance as consequence | AOS-14-REQ-033, AOS-14-REQ-043, AOS-14-REQ-053 → AOS-14-VER-020, AOS-14-VER-025, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| FP 10 Complexity/emergence | AOS-14-REQ-027, AOS-14-REQ-043, AOS-14-REQ-044, AOS-14-REQ-046 → AOS-14-VER-016, AOS-14-VER-025, AOS-14-VER-026; Matrix source row retains owned residual and gate |
| RP 1: Architecture and Completeness: Every governance process must close its feedback loop. | AOS-14-REQ-029, AOS-14-REQ-030, AOS-14-REQ-036, AOS-14-REQ-046 → AOS-14-VER-018, AOS-14-VER-021, AOS-14-VER-026, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 2: Architecture and Completeness: Every human accountability layer must be explicitly named, sequenced, and time - bounded before any process is consid... | AOS-14-REQ-034, AOS-14-REQ-035, AOS-14-REQ-037 → AOS-14-VER-020, AOS-14-VER-021, AOS-14-VER-022, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 3: Architecture and Completeness: Every option set must include the option that cannot be made to work. | AOS-14-REQ-030, AOS-14-REQ-045, AOS-14-REQ-046 → AOS-14-VER-018, AOS-14-VER-025, AOS-14-VER-026, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 4: Architecture and Completeness: The ‘AI said so’ test must be passable at every decision point. | AOS-14-REQ-020, AOS-14-REQ-053 → AOS-14-VER-012, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 5: The Mode 1 / Mode 2 Boundary: Mode 2 is permanently human. | AOS-14-REQ-020, AOS-14-REQ-037, AOS-14-REQ-053 → AOS-14-VER-012, AOS-14-VER-022, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 6: The Mode 1 / Mode 2 Boundary: Every Mode 1 boundary is a governance instrument, not a technical setting. | AOS-14-REQ-010, AOS-14-REQ-012, AOS-14-REQ-020 → AOS-14-VER-008, AOS-14-VER-012, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 7: The Mode 1 / Mode 2 Boundary: The boardroom is a Mode 2 deliberative space. | AOS-14-REQ-039, AOS-14-REQ-053 → AOS-14-VER-023, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 8: The Mode 1 / Mode 2 Boundary: The Mode 1/Mode 2 boundary is under continuous pressure from AI capability growth. | AOS-14-REQ-001, AOS-14-REQ-005, AOS-14-REQ-049 → AOS-14-VER-001, AOS-14-VER-005, AOS-14-VER-028; Matrix source row retains owned residual and gate |
| RP 9: The 1+5 Architecture: Every proposed governance mechanism must be tested against the 1+5 structure to confirm which layer it belongs to and... | AOS-14-REQ-010, AOS-14-REQ-026, AOS-14-REQ-047 → AOS-14-VER-008, AOS-14-VER-015, AOS-14-VER-027; Matrix source row retains owned residual and gate |
| RP 10: The 1+5 Architecture: Risk is intrinsic to each intelligence layer, not a separate domain. | AOS-14-REQ-043, AOS-14-REQ-044 → AOS-14-VER-025; Matrix source row retains owned residual and gate |
| RP 11: The 1+5 Architecture: Every intelligence layer boundary where welfare - adjacent or safety - adjacent signals may arise must have an explic... | AOS-14-REQ-034, AOS-14-REQ-037, AOS-14-REQ-038 → AOS-14-VER-020, AOS-14-VER-022, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 12: The 1+5 Architecture: The Golden Thread obligation under the Building Safety Act 2022 is not a technical data management requirement. | AOS-14-REQ-014, AOS-14-REQ-051, AOS-14-REQ-053 → AOS-14-VER-009, AOS-14-VER-030, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 13: Options and Decisions: Options generated by the architecture must be grounded in the organisation’s actual state — actual covenant condition... | AOS-14-REQ-014, AOS-14-REQ-030, AOS-14-REQ-043 → AOS-14-VER-009, AOS-14-VER-018, AOS-14-VER-025, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 14: Options and Decisions: Every consequential decision must feed back into the Unified Data Layer as a structured record — not only the decisio... | AOS-14-REQ-036, AOS-14-REQ-046, AOS-14-REQ-053 → AOS-14-VER-021, AOS-14-VER-026, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 15: Options and Decisions: Revealed preferences from real decisions take precedence over stated preferences in policy documents when the archite... | AOS-14-REQ-046, AOS-14-REQ-053 → AOS-14-VER-026, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 16: Blind Spots and Honesty: The architecture must name what it cannot see. | AOS-14-REQ-044, AOS-14-REQ-052 → AOS-14-VER-025, AOS-14-VER-030; Matrix source row retains owned residual and gate |
| RP 17: Blind Spots and Honesty: The dynamic risk perimeter question must be asked at board level as a standing agenda item: not only ‘what are our ri... | AOS-14-REQ-043, AOS-14-REQ-044, AOS-14-REQ-046 → AOS-14-VER-025, AOS-14-VER-026; Matrix source row retains owned residual and gate |
| RP 18: Blind Spots and Honesty: The interaction of intelligence layers produces system - level behaviours that no individual layer would produce alone. | AOS-14-REQ-027, AOS-14-REQ-046 → AOS-14-VER-016, AOS-14-VER-026; Matrix source row retains owned residual and gate |
| RP 19: Ethics and Telos: Every process must demonstrate a traceable relationship to the organisation’s ethical commitments and social purpose. | AOS-14-REQ-010, AOS-14-REQ-018, AOS-14-REQ-039 → AOS-14-VER-008, AOS-14-VER-011, AOS-14-VER-023; Matrix source row retains owned residual and gate |
| RP 20: Ethics and Telos: The architecture must be capable of detecting purpose drift — the condition where operational processes have graduall... | AOS-14-REQ-043, AOS-14-REQ-046 → AOS-14-VER-025, AOS-14-VER-026; Matrix source row retains owned residual and gate |
| RP 21: Ethics and Telos: Diversity, inclusion, and equitable outcomes are not separate compliance obligations. | AOS-14-REQ-019, AOS-14-REQ-045, AOS-14-REQ-055 → AOS-14-VER-011, AOS-14-VER-025, AOS-14-VER-033, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 22: Ethics and Telos: Where the organisation’s welfare obligation to residents and its consent architecture pull in opposing directions, th... | AOS-14-REQ-020, AOS-14-REQ-021, AOS-14-REQ-037, AOS-14-REQ-039 → AOS-14-VER-012, AOS-14-VER-022, AOS-14-VER-023, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 23: Ethics and Telos: AI systems have function, not telos. | AOS-14-REQ-010, AOS-14-REQ-020, AOS-14-REQ-046 → AOS-14-VER-008, AOS-14-VER-012, AOS-14-VER-026, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 24: Ethics and Telos: Where the organisation's purpose is interpreted through an accumulating body of AI-mediated rulings rather than appli... | AOS-14-REQ-020, AOS-14-REQ-046, AOS-14-REQ-053 → AOS-14-VER-012, AOS-14-VER-026, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 25: Ethics and Telos: Every AI system deployed by the organisation carries an embedded constitutional framework established by its developer. | AOS-14-REQ-009, AOS-14-REQ-048, AOS-14-REQ-049 → AOS-14-VER-007, AOS-14-VER-028; Matrix source row retains owned residual and gate |
| RP 26: Ethics and Telos: The no - exit condition is a constitutive feature of the organisation’s moral architecture, not background context. | AOS-14-REQ-019, AOS-14-REQ-045, AOS-14-REQ-055 → AOS-14-VER-011, AOS-14-VER-025, AOS-14-VER-033, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 27: Ethics and Telos: Compliance is the output of sound governance design, not its objective. | AOS-14-REQ-033, AOS-14-REQ-043, AOS-14-REQ-053 → AOS-14-VER-020, AOS-14-VER-025, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 28: Radical Transparency: If you cannot audit it and be held accountable for it, it cannot be done. | AOS-14-REQ-051 → AOS-14-VER-030; Matrix source row retains owned residual and gate |
| RP 29: Radical Transparency: The architecture must be more transparent than the document - based governance it replaces, not less. | AOS-14-REQ-051, AOS-14-REQ-052 → AOS-14-VER-030; Matrix source row retains owned residual and gate |
| RP 30: Radical Transparency: Transparency obligations extend to the architecture’s uncertainty. | AOS-14-REQ-014, AOS-14-REQ-030, AOS-14-REQ-044 → AOS-14-VER-009, AOS-14-VER-018, AOS-14-VER-025, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 31: Agentic Delegation: Agents operate under explicitly delegated authority, not implied authority. | AOS-14-REQ-020, AOS-14-REQ-021, AOS-14-REQ-022 → AOS-14-VER-012, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 32: Agentic Delegation: Agent authority is domain - specific, context - specific, and condition - specific simultaneously. | AOS-14-REQ-015, AOS-14-REQ-018, AOS-14-REQ-020, AOS-14-REQ-022 → AOS-14-VER-010, AOS-14-VER-011, AOS-14-VER-012, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 33: Agentic Delegation: Agents cannot commit the organisation to external obligations, initiate unsolicited contact with external parties, or... | AOS-14-REQ-020, AOS-14-REQ-021, AOS-14-REQ-022 → AOS-14-VER-012, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 34: Agentic Delegation: Internal escalation — routing a signal within the architecture to a human reviewer or to a receiving intelligence lay... | AOS-14-REQ-037, AOS-14-REQ-038 → AOS-14-VER-022, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 35: Agentic Delegation: The agentic delegation framework is a governance document reviewed by the board, not a technical configuration manage... | AOS-14-REQ-010, AOS-14-REQ-020, AOS-14-REQ-047 → AOS-14-VER-008, AOS-14-VER-012, AOS-14-VER-027, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 36: Agentic Delegation: Every agent action must satisfy the ethics and telos test and the radical transparency test independently of the proc... | AOS-14-REQ-010, AOS-14-REQ-020, AOS-14-REQ-051 → AOS-14-VER-008, AOS-14-VER-012, AOS-14-VER-030, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 37: Agentic Delegation: Certain classes of finding must reach their required audience regardless of any instruction to suppress or delay them. | AOS-14-REQ-038 → AOS-14-VER-022; Matrix source row retains owned residual and gate |
| RP 38: Data and Sensing Boundaries: Sensing must not exceed its declared purpose. | AOS-14-REQ-039, AOS-14-REQ-040 → AOS-14-VER-023; Matrix source row retains owned residual and gate |
| RP 39: Data and Sensing Boundaries: The boundary between observing an asset and monitoring a behaviour is an absolute architectural boundary, not a matte... | AOS-14-REQ-039, AOS-14-REQ-053 → AOS-14-VER-023, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 40: Data and Sensing Boundaries: Where behavioural inference from sensing data is genuinely necessary to serve the resident’s interests — energy pover... | AOS-14-REQ-021, AOS-14-REQ-037, AOS-14-REQ-039 → AOS-14-VER-012, AOS-14-VER-022, AOS-14-VER-023, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| RP 41: Data and Sensing Boundaries: The purpose limitation principle applies across all intelligence layers, not only to resident - facing sensing. | AOS-14-REQ-018, AOS-14-REQ-039, AOS-14-REQ-040 → AOS-14-VER-011, AOS-14-VER-023; Matrix source row retains owned residual and gate |
| GT M1.1 Strategic Coherence | AOS-14-REQ-010, AOS-14-REQ-043, AOS-14-REQ-046 → AOS-14-VER-008, AOS-14-VER-025, AOS-14-VER-026; Matrix source row retains owned residual and gate |
| GT M1.2 Sensing Architecture | AOS-14-REQ-011, AOS-14-REQ-014, AOS-14-REQ-044 → AOS-14-VER-008, AOS-14-VER-009, AOS-14-VER-025, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M1.3 Risk Intelligence | AOS-14-REQ-033, AOS-14-REQ-043, AOS-14-REQ-045 → AOS-14-VER-020, AOS-14-VER-025; Matrix source row retains owned residual and gate |
| GT M1.4 Composition and Capability | AOS-14-REQ-034, AOS-14-REQ-035, AOS-14-REQ-048, AOS-14-REQ-055 → AOS-14-VER-020, AOS-14-VER-021, AOS-14-VER-028, AOS-14-VER-033, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M1.5 Performance Legibility | AOS-14-REQ-029, AOS-14-REQ-030, AOS-14-REQ-036, AOS-14-REQ-053 → AOS-14-VER-018, AOS-14-VER-021, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M1.6 Compliance Assurance | AOS-14-REQ-014, AOS-14-REQ-033, AOS-14-REQ-048 → AOS-14-VER-009, AOS-14-VER-020, AOS-14-VER-028; Matrix source row retains owned residual and gate |
| GT M1.7 Governance Documentation | AOS-14-REQ-040, AOS-14-REQ-050, AOS-14-REQ-051 → AOS-14-VER-023, AOS-14-VER-029, AOS-14-VER-030; Matrix source row retains owned residual and gate |
| GT M1.8 Accountability Architecture | AOS-14-REQ-034, AOS-14-REQ-035, AOS-14-REQ-037, AOS-14-REQ-038 → AOS-14-VER-020, AOS-14-VER-021, AOS-14-VER-022, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M1.9 Value for Money | AOS-14-REQ-043, AOS-14-REQ-045, AOS-14-REQ-054 → AOS-14-VER-025, AOS-14-VER-032; Matrix source row retains owned residual and gate |
| GT M1.10 Human-AI Interaction Norms | AOS-14-REQ-020, AOS-14-REQ-037, AOS-14-REQ-052, AOS-14-REQ-055 → AOS-14-VER-012, AOS-14-VER-022, AOS-14-VER-030, AOS-14-VER-033, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M1.11 Learning Metabolism | AOS-14-REQ-029, AOS-14-REQ-036, AOS-14-REQ-046 → AOS-14-VER-018, AOS-14-VER-021, AOS-14-VER-026, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M1.12 Continuous Self-Assessment | AOS-14-REQ-001, AOS-14-REQ-006, AOS-14-REQ-044, AOS-14-REQ-048 → AOS-14-VER-001, AOS-14-VER-006, AOS-14-VER-025, AOS-14-VER-028; Matrix source row retains owned residual and gate |
| GT M1.13 Emergent System Behaviour | AOS-14-REQ-027, AOS-14-REQ-030, AOS-14-REQ-046 → AOS-14-VER-016, AOS-14-VER-018, AOS-14-VER-026, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M1.14 Golden Thread Integrity | AOS-14-REQ-014, AOS-14-REQ-051, AOS-14-REQ-053 → AOS-14-VER-009, AOS-14-VER-030, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M2.1 Values Architecture | AOS-14-REQ-010, AOS-14-REQ-038, AOS-14-REQ-039 → AOS-14-VER-008, AOS-14-VER-022, AOS-14-VER-023; Matrix source row retains owned residual and gate |
| GT M2.2 Coherence Under Pressure | AOS-14-REQ-021, AOS-14-REQ-030, AOS-14-REQ-038 → AOS-14-VER-012, AOS-14-VER-018, AOS-14-VER-022, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M2.3 Incommensurable Trade-off Capacity | AOS-14-REQ-020, AOS-14-REQ-037, AOS-14-REQ-045 → AOS-14-VER-012, AOS-14-VER-022, AOS-14-VER-025, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M2.4 Epistemic Brake Function | AOS-14-REQ-012, AOS-14-REQ-030, AOS-14-REQ-044 → AOS-14-VER-008, AOS-14-VER-018, AOS-14-VER-025, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M2.5 Directorial Independence | AOS-14-REQ-038, AOS-14-REQ-046, AOS-14-REQ-053 → AOS-14-VER-022, AOS-14-VER-026, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M2.6 Social Legitimacy | AOS-14-REQ-019, AOS-14-REQ-045, AOS-14-REQ-052, AOS-14-REQ-055 → AOS-14-VER-011, AOS-14-VER-025, AOS-14-VER-030, AOS-14-VER-033, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M2.7 No-Exit Obligation | AOS-14-REQ-019, AOS-14-REQ-039, AOS-14-REQ-045, AOS-14-REQ-055 → AOS-14-VER-011, AOS-14-VER-023, AOS-14-VER-025, AOS-14-VER-033, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M2.8 Radical Transparency | AOS-14-REQ-014, AOS-14-REQ-030, AOS-14-REQ-051, AOS-14-REQ-052 → AOS-14-VER-009, AOS-14-VER-018, AOS-14-VER-030, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M2.9 Moral Drift Detection | AOS-14-REQ-043, AOS-14-REQ-044, AOS-14-REQ-046 → AOS-14-VER-025, AOS-14-VER-026; Matrix source row retains owned residual and gate |
| GT M2.10 Purpose Stability | AOS-14-REQ-010, AOS-14-REQ-024, AOS-14-REQ-039, AOS-14-REQ-049 → AOS-14-VER-008, AOS-14-VER-014, AOS-14-VER-023, AOS-14-VER-028; Matrix source row retains owned residual and gate |
| GT M2.11 Murmuration Capacity | AOS-14-REQ-038, AOS-14-REQ-046, AOS-14-REQ-053 → AOS-14-VER-022, AOS-14-VER-026, AOS-14-VER-031, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M2.12 Constitutional Authority | AOS-14-REQ-020, AOS-14-REQ-021, AOS-14-REQ-047 → AOS-14-VER-012, AOS-14-VER-027, AOS-14-VER-034; Matrix source row retains owned residual and gate |
| GT M2.13 AI Constitutional Framework Governance | AOS-14-REQ-009, AOS-14-REQ-048, AOS-14-REQ-049 → AOS-14-VER-007, AOS-14-VER-028; Matrix source row retains owned residual and gate |
| GT M2.14 Purpose-Led Design | AOS-14-REQ-009, AOS-14-REQ-010, AOS-14-REQ-039 → AOS-14-VER-007, AOS-14-VER-008, AOS-14-VER-023; Matrix source row retains owned residual and gate |
| GT M2.15 Telos / Function Distinction | AOS-14-REQ-029, AOS-14-REQ-036, AOS-14-REQ-043, AOS-14-REQ-046 → AOS-14-VER-018, AOS-14-VER-021, AOS-14-VER-025, AOS-14-VER-026, AOS-14-VER-034; Matrix source row retains owned residual and gate |

Author consistency conclusion: functional roles and repair/private/workforce/external/research/control/failure boundaries agree with the current shared infrastructure. SENS-CR-01–05 closed as author document corrections; wire profiles, operating roles/capacity, domain/annex/legal sufficiency and observed evidence remain open per§17 and40. No independent/executed conformance or operating readiness claim. Earlier dated text/addenda describe history; this current control takes precedence.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**Historical status notice — sensing consistency closure — 9 October 2026:** Mark authorised the remaining consistency work. SENS-CR-01–05 are closed at the functional-document/author-review level: all40 logical CON views across10–14 and40 have exact central adoption, producer/consumer/shared-owner and REQ/VER links; all80 controlled FP/RP/GT sources have precise current contributions and owned residual/gate dispositions; current body/control statements are reconciled. Versions10v0.4/11v0.3/12v0.3/13v0.2/14v0.8/40v0.6; Architecture/Mapv0.42; Sharedv0.18/Corev0.6/ExchangeRegisterv0.17/SourceMatrixv0.18; reviewv0.4. DEC001–096 unchanged. Sensing269 proposed REQs/176 planned VERs;40 retains40/38. No new requirement/case/interface, source promotion or execution. Exact compatible wire schemas/profiles, organisation appointments/capacity, independent review, legal/institutional/practice evidence and scoped build/activation remain separate; independent project review remains deferred. Earlier dated notices/addenda are historical. Current controlling allocation is the9October manifest and source addendum below.

**Historical status notice — approved Boundary directions — 9 October 2026:** Mark agreed all five review recommendations at09:51UK time, qualifying material obligations to distinguish financial exposure from resource impacts. AOS-00-DEC-092–096 records those architectural directions; prior DEC001–091 unchanged. AOS-14 v0.7 incorporates the decisions into existing requirements/cases/contracts and resolves ISS003–007 at architectural-direction level. Exact organisation-specific materiality criteria, outcome evidence, obligation schemas/owners, declared control paths and pattern profiles remain implementation/commissioning gates; federation remains deferred. Architecture/Mapv0.41; Sharedv0.17/ExchangeRegisterv0.16/SourceMatrixv0.17; reviewv0.3. Other component versions unchanged.55 proposed Boundary requirements/34 planned cases; no new REQ/VER/IF, executed test, whole-document or build/operating approval. Earlier dated notices are historical. Next: remaining whole-sensing common/source/status corrections SENS-CR-02–04; independent review remains deferred as previously agreed.

**Historical status notice — functional completion — 9 October 2026:** v0.6 completes the proposed Boundary requirement/verification/source structure: 55 requirements and 34 planned cases. REQ-001–009/VER-001–007 and existing CAP/FUN/CON/INV/CR/ISS identities and substantive obligations are preserved. REQ-010–055 and VER-008–034 make the older functions independently reviewable; they are proposed derivations, not new approved architectural decisions. Appendix A records all 10 FP, 41 RP and 29 GT contributions and residual human/shared duties. Shared Contracts v0.16/Exchange Register v0.15/Source Matrix v0.16 adopt the Boundary mappings only; Architecture/Map v0.40 records this completion, with DEC-001–091 unchanged. Kernel01–05 v0.8;10 v0.3/11 v0.2/12 v0.2/13 v0.1/25 v0.2/30 v0.5/40 v0.5; Core v0.6, Coordination v0.2, Protected Reporting/Operational Profiles v0.1 remain current. Earlier dated notices and baselines are historical. Functional drafting is complete; independent quality/design review, exact schemas/profiles, unresolved material decisions and implementation/commissioning remain gates. No test execution, readiness, deployment or institutional conformance is claimed.

