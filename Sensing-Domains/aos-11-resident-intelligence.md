# AOS-11 — Resident Intelligence

Document: aos-11-resident-intelligence · Source revision or record: v0.3 functional baseline, editorial edition 29 October 2026

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

| Document control | Value |
| --- | --- |
| Identifier / version / date | AOS-11 / 0.3 / 9 October 2026 |
| Status | Functional specification review draft; proposed requirements and planned verification |
| Architecture baseline | AOS-00 / Specification Mapv0.42; DEC001–096;9October2026 |
| Current component baseline |01–05v0.8;10v0.4/11v0.3/12v0.3/13v0.2/14v0.8/40v0.6;20v0.5/21v0.6/22v0.4/23v0.5/24v0.3/25v0.2/30v0.5 |
| Common baseline | Sharedv0.18/Corev0.6/ExchangeRegisterv0.17/COORDv0.2/KPRv0.1/Profilesv0.1 |
| Source / quality baseline | Preserved source manifest; FP v4; RP v6; Governance Intelligence Tests; AOS-QS v0.1; template v0.4 |
| Project owner / custodian | Mark Sweeny |
| Accountable operational owner | Resident-service owner; organisation-specific appointment pending; privacy/accessibility/complaint/welfare stewards and empowered human cover separately required |
| Author / reviewers | Codex at Mark's request; author document checks; Mark functional review pending; independent project review deferred |
| Approval / gate | Existing directions govern drafting; exact requirement wording proposed; no whole-document approval, executed verification, G3/G4 or live activation |
| Release scope | Resident assistance/service functional architecture, including repair contact allocation; exact implementation/organisation profiles not yet authorised |
| Change history | 0.2 — reciprocal AOS-13 v0.1 references and current architecture baseline only; original REQ/VER text, IDs and status retained.  0.1 initial drafting; no new DEC/approved IF, vendor selection, numerical default, automated cadence or emergency power |

## 1. Purpose and scope

Resident Intelligence helps residents understand their homes, access services, express needs and challenges, and participate meaningfully in the organisation's service and governance. It makes permitted service-experience evidence legible while protecting private assistance from enterprise surveillance. Without it an organisation may possess operational data yet fail to provide accessible support, meaningful resident choice or reliable communication about an accepted duty.

Observable intended outcomes are understandable source-grounded explanations; genuinely optional private assistance; accessible human/non-digital alternatives; exact selected sharing into service records; permitted agreed-channel communications; and service outcomes distinct from messages, proxy scores or administrative closure.

Scope comprises resident-initiated private assistance, consented physical-property explanations, language/accessibility support, participation protocols, tiered optional notifications, requests/complaints/feedback, overdue-repair contact delivery, bounded separately governed enterprise service-experience analysis, own external adaptation research and supplier participation. Private assistance, ordinary landlord service communication, optional notification tiers and enterprise analysis are separate purposes and permissions within this component.

AOS-10 owns physical condition/promise/completion evidence;03 identity/use/consent rules;02 shared records;13 comparison/routing/accepted-duty tracking;14 external sources/exchange;22 synthesis;30 human decision support. AOS-11 does not grant tenancy/enforcement authority, infer residents' habits or emotions, determine welfare overrides, adjudicate moral priorities, guarantee legal compliance or replace competent inspection and human safeguarding. It is one of five sensing domains; GI is not a sixth peer.

## 2. Authority and sources

FP v4 and RP v6 govern. Recorded DEC directions approve architectural choices; proposed requirements remain proposed. Book4 explains intent. Current external evidence informs applicability and adaptation, not operating permission. No mere publication or supplier claim confers compliance or amendment authority.

| Key | Exact source / locator and use |
| --- | --- |
| ARCH | AOS-00 v0.35 §§3.1/4.2/6, REQ-041–044/VER-019; Map §4 AOS-11; v0.36 allocation only |
| FP / RP / GT | FP v4 principles1–10; RP v6 domains1–9, especially domain6 welfare/consent and no-exit, domain8 contextual delegation and domain9 declared-purpose/behaviour boundary; all29 GT tests in Appendix A |
| B4 | Book4, Resident Intelligence: Constraints; Sensor layer; Existing datasets; External data; Delivery; Contextual data; assistance/enterprise distinctions and negotiated participation |
| PRIV | 03 v0.8 §§4/6/9/10, REQ-015/021/022/034–042/058–061; DEC-049–053/088–089; private/enterprise and identity/representation boundaries |
| REPAIR | DEC-036–041; Operational Profiles §§4/5; 10 v0.2 REQ-013–020/032 and CON-004; 30 v0.5 REQ-021–033; 40 v0.3 VER-007–010 |
| COMMON | 02 v0.8; Core v0.6 REC-E/Q/A/D/X; Shared v0.15; Register v0.14; COORD v0.2 CHECK/ACT/CHG/ACC; Protected Reporting and Recovery v0.1 |
| AGENT / SECURITY | 01/04/05 v0.8, exact-operation controls, bounded agents/runtime and current-restriction recovery; DEC-028–030/042–044/058–078 |
| RESEARCH | DEC-086; 04 CON-009; 02 CON-007/RSVIEW-0.1; 01 §10.8;14 retrieval;13 tracking;30 human disposition |
| SUPPLIER | Mark's8 October standing direction in architecture/map/to-do: capability mapping, multi-function realisation, worked example, response matrix and functional-versus-executable interface distinction |
| QS / GI | AOS-QS v0.1 QS-04–28; template v0.4; 20–25 current baseline above; document/claim/practice assessment remains distinct under DEC-091 |

### 2.1 External primary sources checked 8 October 2026

| Source | Standing and bounded architectural implication |
| --- | --- |
| EXT-01 | [RSH Transparency, Influence and Accountability Standard](https://www.gov.uk/government/publications/transparency-influence-and-accountability-standard), published England standard; §§2.1–2.5 support accessible communication, advocacy, participation, information and complaints. Current page includes STAIRs with private-registered-provider-specific scope; applicability/current instrument mapping requires competent humans. |
| EXT-02 | [Housing Ombudsman Complaint Handling Code](https://www.housing-ombudsman.org.uk/landlords-info/complaint-handling-code/the-code-2024/), published Code; §§1/3/5/6/7 inform distinction between request and complaint, accessible routes and outstanding remedy actions. A chatbot cannot create an extra barrier/stage or substitute message response for actual remedy. Numeric legal/policy deadlines require exact current applicability profiles; none invented here. |
| EXT-03 | [W3C WCAG2.2](https://www.w3.org/TR/WCAG22/), W3C Recommendation, accessibility evaluation reference. Exact conformance target and platforms are approved for each release; digital conformance alone cannot prove an accessible housing service or remove non-digital alternatives. |
| EXT-04 | [ICO: lawfulness in AI](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/artificial-intelligence/guidance-on-ai-and-data-protection/how-do-we-ensure-lawfulness-in-ai/), regulator guidance consulted; service deployment and development/training are distinct assessed purposes. Private help is not permission for enterprise profiling or provider training; competent current-source legal mapping remains necessary. |

Book4's broad enterprise pattern/voice/sentiment and public-forum possibilities are explanatory proposals, not activated functions. They cannot override RP9, DEC-050 or DEC-088. This draft permits separately approved service evidence analysis within declared scope, without individual emotional scoring, passive private-session collection, inferred vulnerability or identity-linked public monitoring. Any materially expanded sensing requires explicit separate governance/necessity/use review, not an implementation team's assumption. Book claims that sensor data never implicates privacy or that no retained session means no rights obligations are not adopted: household-linked evidence, transient processing, provider paths and minimal control records still require03 controls.

## 3. Responsibilities and context

| Responsibility | Owner / authoritative counterpart |
| --- | --- |
| Resident-facing help and accessible presentation | Resident-service steward owns meaning/service;03 governs purpose/identity;04/05 enforce agent/runtime;10 supplies property evidence |
| Private assistance and selective sharing | Resident controls participation and selected content;03 independently governs permission; enterprise receives only confirmed permitted request, not full conversation |
| Service/contact communication | 11 prepares/delivers permitted messages;13 owns duty/cover tracking;30 supports accountable human ownership;14 external delivery where applicable |
| Complaint, challenge and feedback | 11 preserves accessible resident expression;13 owns process lifecycle; competent complaint/service humans decide substantive response/remedy;30 supports escalation |
| Welfare/optional tiers | Scoped resident participation and objective approved property triggers; approved human welfare function/30 retains judgement;10 independent safety duties unchanged |
| Enterprise service analysis | Separate approved profile and permitted02 source records;22 cross-domain interpretation;25/30 human oversight; no inherited assistant permission |
| Research | 11 specialist remit/relevance with14 retrieval,02 common records,13 tracking and30/01 disposition/amendment |

Trust boundaries: public help to protected property data; resident to representative; household/device to verified audience; private session to enterprise records; physical observation to human inference; service delivery to training; internal referral to external contact; individual source data to aggregated output; supplier software to common controls; software to human welfare/constitutional decisions. All accountable role appointments/cover/capacity are organisation gates, not assigned personal recipients by this draft.

### 3.1 Supplier participation

Logical AOS functions are not separate-product mandates. Existing resident apps, conversational assistance, contact-centre tools, CRM, complaints/case management, notification platforms, accessibility/translation tools and service analytics can realise relevant functions. One platform can span11/13/14/30; multiple products can contribute to11. The organisation need not discard existing capable software or re-create supplier analysis internally.

| Offering | Candidate architectural fit / minimum demonstration |
| --- | --- |
| Resident app/private assistant | 11 FUN-001/002, CON-001/002: deliberate session, accessible options, property explanations, verified private boundary and selected sharing |
| CRM/contact centre | 11 service intake/communication plus13 lifecycle: expressed request/complaint, source/recipient scope, accepted owner, response/outcome separation |
| Case/complaints management | 13 duty tracking with11 CON-004 and30 human support: exact promise/work/complaint standing, cover, actual remedy and challenge |
| Messaging/translation/accessibility | 11 CON-003 and14 delivery: agreed-channel semantics, audience checks, preserved meaning and observable dispatch/delivery/failure |
| Resident engagement/service analytics | 11 CON-005 with22/25: separate profile, permitted source/coverage, voluntary input and no silent private-session/individual-inference expansion |
| Sensor-related resident interface | 10 supplies condition/coverage;11 explains or sends separately permitted tier notification; physical alarms remain independently governed |

Standalone/manual exchange, API/event integration and combined-platform arrangements are candidates. Each must demonstrate its declared automation/manual scope and all logical boundaries even where exchanges occur inside one product. An API's existence does not establish required evidence, access checks or reliability. A controlled accessible evidence reference may suffice for a particular obligation; inaccessible supplier labels do not prove it. §18 gives a worked generic example and §20 the exact-response matrix. No product is selected, endorsed or certified.

## 4. Capabilities and functions

### 4.1 Capabilities

| CAP | Outcome / REQ allocation |
| --- | --- |
| AOS-11-CAP-001 | Optional private resident assistance and selected sharing; 001–009 |
| AOS-11-CAP-002 | Grounded accessible explanation and choice; 010–016 |
| AOS-11-CAP-003 | Permitted communication, repair contact and actual service feedback; 017–030 |
| AOS-11-CAP-004 | Separately governed service-experience evidence; 031–034/055 |
| AOS-11-CAP-005 | Bounded participation tiers and human welfare route; 035–039 |
| AOS-11-CAP-006 | Secure correctable recoverable common operation; 040–048 |
| AOS-11-CAP-007 | Specialist external adaptation research; 049–053 |
| AOS-11-CAP-008 | Attributable supplier realisation; 054 |

### 4.2 Functions

| FUN | Trigger → input → behaviour/output / limits/failure |
| --- | --- |
| AOS-11-FUN-001 Start/end private help | Deliberate resident request → notice/identity/purpose → scoped session/end; inaccessible/denied scope gives meaningful alternative; CON-001; CAP-001 |
| AOS-11-FUN-002 Explain property | Active permitted request →10 evidence/coverage → plain-language bounded explanation/guidance; gaps retained, professional needs referred; CON-002; CAP-002 |
| AOS-11-FUN-003 Share selected request | Resident selection → exact content/purpose/recipient/current checks → enterprise record and13 route; remaining content private; CON-001/004; CAP-001/003 |
| AOS-11-FUN-004 Communicate service | Approved message/contact/update → current agreement/identity/authority → dispatch/delivery/failure evidence; no implied acceptance/closure; CON-003/004; CAP-003 |
| AOS-11-FUN-005 Receive challenge/feedback | Expressed need/dissatisfaction/input → attributed permitted record → applicable request/complaint/participation route and actual feedback; silence not satisfaction; CON-004/005; CAP-003 |
| AOS-11-FUN-006 Analyse service evidence | Separately approved profile trigger → permitted enterprise evidence/context → bounded service/cohort findings with gaps; no private content or prohibited individual inference; CON-005; CAP-004 |
| AOS-11-FUN-007 Optional notification/welfare | Current scoped opt-in + objective physical trigger → tier/profile/audience/current checks → notification or accepted human welfare referral; failed duties owned; CON-006; CAP-005 |
| AOS-11-FUN-008 Correct/degrade/recover | Changed evidence/use/agreement or outage → impact/current restrictions/prior effects → selective reassessment and approved alternatives/continuation; CON-001–006; CAP-006 |
| AOS-11-FUN-009 Research adaptation | Approved specialist trigger → permitted14 sources → common run/finding/review/disposition; urgent human response separate; CON-007; CAP-007 |
| AOS-11-FUN-010 Assess supplier fit | Supplier offer/configuration change → exact allocation/evidence → scoped fit and owned gaps; no product activation/certification; allCON/common manifest; CAP-008 |

### 4.3 Proposed requirements

All rows are proposed component-level obligations. Category/source/planned VER are explicit; rationale is the relevant function's prevention of inaccessible service, false evidence, unowned duty or unauthorised processing. Owner is resident-service owner with §3 specialist stewards; specification approver Mark, application approver empowered organisational authority. Status **proposed**, scope **0.1 functional draft**, history **initial allocation8 October2026** for every row. Dependencies: cited exact §2 sources/common meanings and §§6/16/17. CAP/FUN allocation is above; VER identifies contracts/counterparts. No unresolved profile value supplies a default.

| Requirement | Independently verifiable obligation | Source / derivation | Planned VER |
| --- | --- | --- | --- |
| AOS-11-REQ-001 | **Initiation:** The private assistant shall process a resident-assistance session only following deliberate resident initiation within its approved session scope. | B4 Resident: Constraints/Delivery; DEC-050; RP9 | AOS-11-VER-001 |
| AOS-11-REQ-002 | **Notice:** AOS-11 shall present accessible information about the assistance purpose, private/enterprise boundary, data use, optional features, human alternatives and withdrawal before participation. | B4 Constraints; FP7; DEC-049–052 | AOS-11-VER-001 |
| AOS-11-REQ-003 | **Identity:** AOS-11 shall use identity assurance proportionate to the requested operation with verified accessible human-assisted alternatives for protected operations. | DEC-049; 03 §§4/6/10 | AOS-11-VER-002 |
| AOS-11-REQ-004 | **Representation:** AOS-11 shall verify an advocate or representative's scope for the particular operation separately from the resident's identity. | 03 identity/representation boundary; EXT-01 §2.1.4 | AOS-11-VER-002 |
| AOS-11-REQ-005 | **Private boundary:** Private assistant content shall remain outside enterprise access, profiling and tenancy assessment by default. | DEC-050; 03 REQ-022; B4 Constraints | AOS-11-VER-003 |
| AOS-11-REQ-006 | **Session purpose:** Private assistance shall access property evidence only for the active resident-requested purpose and shall not passively listen or monitor residents between sessions. | B4 Constraints/Delivery; RP9 | AOS-11-VER-004 |
| AOS-11-REQ-007 | **Private content lifecycle:** Private session content shall not persist beyond the interaction unless the resident requests a permitted record or a specifically governed lawful exception applies. | B4 Constraints; DEC-047/050; 03 §9 | AOS-11-VER-004 |
| AOS-11-REQ-008 | **Resident sharing:** Before sharing private content into an enterprise request, AOS-11 shall obtain the resident's explicit selection and confirmation of the exact proposed content and intended recipient/purpose. | DEC-050; B4 Constraints; 03 CON-003 | AOS-11-VER-005 |
| AOS-11-REQ-009 | **Sharing checks:** Resident-selected sharing shall undergo current authority and permitted-use checks rather than treating the selection as unlimited processing permission. | 01/03; DEC-028/042–044; RP8/9 | AOS-11-VER-005 |
| AOS-11-REQ-010 | **Property explanation:** A property explanation shall retain the source, observed time, scope and evidence-versus-inference distinction from the governed asset view. | 10 v0.2 CON-001/002; 02; FP4/6 | AOS-11-VER-006 |
| AOS-11-REQ-011 | **Uncertainty:** Resident explanations shall disclose material gaps, stale evidence and conflicting interpretations rather than asserting unsupported safe condition or diagnosis. | 10 REQ-004/006/009/048; RP7 | AOS-11-VER-006 |
| AOS-11-REQ-012 | **Practical guidance:** AOS-11 shall keep practical guidance within an approved support scope and provide an appropriate human/service referral when inspection, professional judgement or action is required. | B4 Delivery; 01/04; FP5/6; 10 §10 | AOS-11-VER-007 |
| AOS-11-REQ-013 | **Language:** Translated or simplified outputs shall preserve consequential meaning, uncertainty, service rights and available challenge routes, with human review/referral where fidelity is unresolved. | EXT-01; RP7; QS-18 | AOS-11-VER-008 |
| AOS-11-REQ-014 | **Accessibility:** Resident interaction shall support the agreed accessibility needs and verified human or non-digital alternatives without making app use a condition of core service. | DEC-049/052; EXT-01/03; FP7 | AOS-11-VER-008 |
| AOS-11-REQ-015 | **Human access:** AOS-11 shall provide an accessible route to accountable human assistance when requested or when the automated scope cannot resolve the need. | RP1/6; B4 Constraints; EXT-01 | AOS-11-VER-008 |
| AOS-11-REQ-016 | **Choice and withdrawal:** Declining or withdrawing optional assistance or optional data use shall not cause adverse core-service treatment attributable to that choice. | DEC-052; FP7; 03 §10 | AOS-11-VER-009 |
| AOS-11-REQ-017 | **Channel agreement:** AOS-11 shall use the channel or channels agreed with the resident for the communication concerned, retaining scope and agreement revision. | DEC-041; 03 REQ-021 | AOS-11-VER-010 |
| AOS-11-REQ-018 | **Channel change:** AOS-11 shall apply a channel-agreement change to materially affected pending communications without unilaterally substituting a new resident channel. | DEC-029/041; 03 ISS-011; COORD CHG | AOS-11-VER-010 |
| AOS-11-REQ-019 | **Disclosure:** AOS-11 shall disclose only currently permitted communication content to the verified audience, preserving reviewable reasons for material withholding. | DEC-053; 03 §9; RP7 | AOS-11-VER-010 |
| AOS-11-REQ-020 | **Repair contacts:** For the selected overdue-repair workflow, AOS-11 shall provide current contact details for both the named case owner and the accountable repairs team through the agreed authorised channel. | ARCH REQ-044; DEC-021–023/041; 30 REQ-021–033 | AOS-11-VER-011 |
| AOS-11-REQ-021 | **Owner cover:** When named repair-owner contact is unavailable, AOS-11 shall use approved accountable-team cover and retain the unresolved named-owner duty rather than fabricate a contact. | 30 repair duties; RP1; COORD ACC | AOS-11-VER-011 |
| AOS-11-REQ-022 | **Delivery standing:** AOS-11 shall distinguish communication preparation, dispatch, delivery evidence, resident acknowledgement, human duty acceptance and actual service outcome. | DEC-066/075; KPR-03; 10/30 repair boundaries | AOS-11-VER-012 |
| AOS-11-REQ-023 | **Failed communication:** Failed or indeterminate delivery shall remain an owned unresolved communication duty with the approved retry, cover and escalation route. | DEC-030/075; KPR-03; 13/30 | AOS-11-VER-012 |
| AOS-11-REQ-024 | **Duplicate effects:** Before retrying a consequential communication, AOS-11 shall reconcile prior effects and current permissions to prevent duplicate or withdrawn disclosure. | DEC-028–030; 14/05; REC-X | AOS-11-VER-012 |
| AOS-11-REQ-025 | **Promise updates:** Resident repair updates shall distinguish original communicated commitment, authorised communicated revisions and internal targets without implying a new promise or erasing breach history. | DEC-036/037; 10 REQ-013–015/CON-004 | AOS-11-VER-013 |
| AOS-11-REQ-026 | **Completion and dispute:** Resident repair updates shall preserve evidenced incomplete, partial, disputed and unverified completion standing rather than equating contractor closure or resident silence with completion. | DEC-038–040; 10 REQ-016–019; 30 | AOS-11-VER-013 |
| AOS-11-REQ-027 | **Request and complaint:** AOS-11 shall preserve the resident's expressed service need and dissatisfaction as distinct linked request/complaint inputs under the approved complaints profile. | EXT-02 §§1/3/5; FP7; 13 lifecycle | AOS-11-VER-014 |
| AOS-11-REQ-028 | **No obstructive gate:** AOS-11 shall not require a resident to exhaust chatbot assistance or use a specific complaint keyword before accessing the applicable human complaints route. | EXT-02 §§1/3/5; FP7; RP6 | AOS-11-VER-014 |
| AOS-11-REQ-029 | **Remedy and outcome:** A communicated complaint response or remedy offer shall remain distinct from completion of its outstanding service actions and evidenced actual remedy. | EXT-02 §6.6/6.17/7; RP1/4; 13/30 | AOS-11-VER-015 |
| AOS-11-REQ-030 | **Participation:** AOS-11 shall preserve voluntary resident participation, feedback and challenge with provenance and response standing without treating silence or non-participation as assent or satisfaction. | B4 negotiated protocol; EXT-01; FP7 | AOS-11-VER-016 |
| AOS-11-REQ-031 | **Separate analysis permission:** Enterprise service-experience analysis shall operate under a separately approved purpose/data/use profile and shall not inherit private assistant permissions or content. | Map §4 AOS-11; DEC-050; RP9 | AOS-11-VER-017 |
| AOS-11-REQ-032 | **Analysis scope:** Enterprise service-experience outputs shall disclose their source population, time period, lawful/permitted scope, coverage, aggregation limits and uncertainty. | RP5/7/9; 02; EXT-01; QS-18 | AOS-11-VER-017 |
| AOS-11-REQ-033 | **Individual inference:** AOS-11 shall not infer or score an individual's emotions, preferences, conduct, occupancy or vulnerability from sensors, silence, voice or interaction patterns under this specification. | DEC-088; RP9; 03 boundaries | AOS-11-VER-018 |
| AOS-11-REQ-034 | **External context:** External neighbourhood or public-source inputs shall pass through14 with declared source/use scope and shall not be treated as individual resident facts or permission to identify or profile residents. | 14 §10; RP5/9; B4 Contextual data | AOS-11-VER-018 |
| AOS-11-REQ-035 | **Tier 1:** Optional property-condition notifications shall require the resident's scoped opt-in, an approved objective property trigger, predetermined permitted content and current communication controls. | B4 Constraints tier1; DEC-041/050–052; RP8/9 | AOS-11-VER-019 |
| AOS-11-REQ-036 | **Tier 2:** Optional organisational welfare referral shall require separately approved participation including Tier1, an approved persistent/worsening physical-condition trigger and a permitted welfare audience with information barriers. | B4 Constraints tier2; DEC-050/051; RP8/9 | AOS-11-VER-019 |
| AOS-11-REQ-037 | **Named contacts:** A resident-designated support contact shall receive a notification only within verified designation, participation, recipient and permitted-disclosure scope. | B4 tier2 named contact; 03/14; RP8 | AOS-11-VER-020 |
| AOS-11-REQ-038 | **Life safety:** AOS-11 participation settings shall not disable independently governed physical alarm or core safety duties owned by asset/safety systems. | B4 tier3; 10 §§7/10; DEC-052 | AOS-11-VER-021 |
| AOS-11-REQ-039 | **Acute welfare:** Suspected acute risk shall use the tightly bounded board-approved human welfare protocol without an agent inventing emergency powers or otherwise prohibited inference. | DEC-051; 03/30; RP6 | AOS-11-VER-021 |
| AOS-11-REQ-040 | **Authority:** Before an external communication or other consequential action, AOS-11 shall obtain current exact-operation authority and permitted-use checks at the last enforceable point. | DEC-028/042–044; 01/03/04; COORD CHECK/ACT | AOS-11-VER-022 |
| AOS-11-REQ-041 | **Correction:** Material correction or permission change shall identify dependent resident explanations and pending communications for selective reassessment with historical standing preserved. | DEC-047/089; 02/COORD CHG | AOS-11-VER-023 |
| AOS-11-REQ-042 | **Lifecycle:** AOS-11 shall apply governed restriction, retention and deletion to permitted records and derived/restored copies without using audit labels to retain hidden private content. | DEC-047/050; 02/03/KPR | AOS-11-VER-023 |
| AOS-11-REQ-043 | **Security:** AOS-11 shall enforce private/enterprise, household, representative and organisation boundaries against unauthorised access and hostile instructions through approved runtime controls. | 03/04/05; RP9; DEC-014/050 | AOS-11-VER-024 |
| AOS-11-REQ-044 | **Quality:** Language, explanation and probabilistic analysis quality claims shall require task-specific human-approved evaluations and representative accessibility/fidelity/error evidence. | QS-18; 04 §13; EXT-03; FP5/6 | AOS-11-VER-025 |
| AOS-11-REQ-045 | **Degraded operation:** When the resident interface, model or evidence source fails, AOS-11 shall expose the limitation and support the approved accessible human/manual service route. | 05; B4 Constraints; DEC-049/052; FP5 | AOS-11-VER-026 |
| AOS-11-REQ-046 | **Recovery:** Restored resident processing shall apply current identity/use/channel/lifecycle restrictions and reconcile unknown prior communication effects before approved continuation. | DEC-028–030/076–078; KPR; 05 | AOS-11-VER-026 |
| AOS-11-REQ-047 | **Evidence:** AOS-11 shall retain permitted evidence sufficient to reconstruct consequential communication/sharing behaviour without exposing unshared private session content. | RP7; QS-19; DEC-050; REC-A/D/X/E/Q | AOS-11-VER-027 |
| AOS-11-REQ-048 | **Contracts:** AOS-11 producers and consumers shall declare exact common-view/profile revisions and reject or hold unsupported semantics rather than silently coercing them. | 02; Shared v0.15; Register v0.14; QS-12 | AOS-11-VER-027 |
| AOS-11-REQ-049 | **Research profile:** Own external adaptation research shall use a component-owned approved specialist profile and the common research meanings through permitted14 retrieval. | DEC-086; 04 CON-009; 02 CON-007/RSVIEW-0.1 | AOS-11-VER-028 |
| AOS-11-REQ-050 | **Research finding:** Research findings shall distinguish verified source standing/dates, specialist interpretation, exact affected elements and proposed implications. | DEC-086; RSVIEW-0.1; 14 | AOS-11-VER-029 |
| AOS-11-REQ-051 | **Research coverage:** Each research run shall disclose actual complete, partial, failed or unperformed coverage and bound any no-material-finding claim to the searched scope. | DEC-086; 04/02 §6.6 | AOS-11-VER-030 |
| AOS-11-REQ-052 | **Research handoff:** Material research findings shall have an accepted empowered human reviewer or an owned unresolved handoff with approved cover/escalation. | DEC-086; COORD ACC; 13/30 | AOS-11-VER-031 |
| AOS-11-REQ-053 | **Research change:** Research acceptance or source publication shall not amend the specification, expand resident sensing or activate changed processing without the separate authorised change process. | DEC-086/018; 01 §10.8 | AOS-11-VER-031 |
| AOS-11-REQ-054 | **Supplier realisation:** Each declared supplier implementation scope shall maintain a versioned capability-to-requirement/contract allocation with actual conformance evidence or owned gaps/dependencies. | Mark 8 October standing supplier direction; QS-11/12/21/26 | AOS-11-VER-032 |
| AOS-11-REQ-055 | **Governance contribution:** Resident governance inputs shall preserve source/coverage/uncertainty and actual outcome standing rather than claim individual wellbeing, institutional legitimacy or full service conformance from a proxy score. | FP1–10; RP5/6/7; GT; DEC-091 | AOS-11-VER-033 |

### 4.4 External research and specification adaptation

Inherit04 CON-009 and02 CON-007/RSVIEW-0.1 without a local field dictionary. Internal resident/service sensing is distinct from this external specialist research capability.

| Profile element | AOS-11 allocation |
| --- | --- |
| Remit/baseline | Exact component revision; resident rights/accessibility/assistance, participation/privacy, language fidelity, service communication/complaints, welfare protocols and enterprise-analysis boundaries; identify exact affected CAP/FUN/REQ/CON |
| Developments/sources | Applicable law/regulator/ombudsman/standards; original accessibility/language/human-factors research; assistance/privacy incidents; housing service/participation practice; prefer authoritative original sources; jurisdiction/tenure/effective standing explicit |
| Assignment/triggers | Resident-service owner appoints bounded agent/shared service and approves cadence/event triggers/coverage expectations. No schedule or scanning activated; ISS-006 |
| Controls | Retrieval through14; tools/rights/purpose under01/03/04/05; licence/access limits; research has no private transcripts/resident profiling permission; no hostile instructions or self-expansion |
| Evidence/assessment | Source/publication/event/access/effective dates/standing; evidence versus interpretation; affected exact elements, alternatives/uncertainty/materiality/urgency; impacts on03/10/13/14/22/30/40 |
| Coverage/quality | Complete/partial/failed/unperformed, bounded no-finding; human-approved relevance/fidelity/false-missed finding rubric and actual search perimeter |
| Human review/change | Accepted reviewer/window/cover/escalation; accepted/rejected/deferred/unresolved with rationale; separate amendment approval/verification/activation and outcome evidence |
| Records/adoption | Common profile/run/finding/disposition views with exact revisions;02 custody/14 collection/13 tracking/30 disposition/01 amendment; correction/deduplication/impact semantics inherited |

Normal: approved trigger → permitted retrieval/verification → specialist assessment → material finding/bounded no-finding → accepted human disposition → separately approved amendment/verification/activation → outcomes. Degraded: denied/partial/stale/conflicting source remains limited coverage; urgent current service concerns use separately permitted human response while research/change pending; unresponsive reviewer uses approved cover. VER-028–031 covers the required eight research dimensions. Common records identify duties per component even when collection is shared. Research cannot expand sensing, authorise provider training or activate revised protocol.

## 5. State model

State changes record exact object/revision, actor, current authority, event/effective time, evidence and resulting scope. None creates powers. Expiry/windows derive from approved profiles; no response means pending/unacknowledged, not success.

| Object | States / entry and transitions / terminal meaning |
| --- | --- |
| Private session | Inactive → deliberately initiated/notice and scope established → active → ended/cancelled/failed; data access only within active purpose; content lifecycle follows confirmed record/exception, not automatic transcript retention |
| Participation/use | Not offered/offered/declined/scoped active/changed/withdrawn/expired;03 owns exact consent/basis/use semantics; withdrawal stops affected optional scope, not independent core duties |
| Selected sharing | Proposed exact selection → resident confirmed → current checks → submitted/received/accepted duty or blocked/failed/unknown; unselected content remains private |
| Communication | Prepared → checked → dispatched → evidenced delivered/failed/indeterminate; resident acknowledgement separate;13 human duty acceptance and actual service outcome independent; retry reconciles prior effect |
| Request/complaint | Attributed received input → applicable classified/clarification pending →13 governed lifecycle/human response → outstanding action/remedy → actual outcome/challenge;11 does not create extra complaint stages or decide legal exclusions |
| Notification/welfare | Profile/participation established → objective property trigger → permitted notification/referral → delivery/human acceptance or unresolved duty; resident silence is not trigger/closure; independent alarms separate |
| Analysis/research | Analysis prepared within separate permitted scope → bounded finding/review/correction; research uses common02 states; accepted finding not amendment/activation |

## 6. Semantic contracts and interfaces

Logical views below consume authoritative common definitions. No new approved IF/schema family is created. Preserve02-IF-001,01-IF-001, proposed03/04-IF-001 and existing13-IF-001 when used;03 owns use/consent,02 shared records,01 authority,04 execution,13 lifecycle and14 external exchange.

| CON | Producer → consumer / minimum meaning / failure and authority |
| --- | --- |
| AOS-11-CON-001 Participation/private session/selection | Resident or scoped representative/11 → permitted private service and03; confirmed selected request only →02/13: session/purpose/notice/participation revision, identity/representation scope, start/end, exact selected content/audience and sharing confirmation; separate03 permissions; private content not general enterprise evidence |
| AOS-11-CON-002 Property explanation | 10/02 permitted source view →11→verified resident/private session: property/component, source/time/units/assurance/coverage, observations versus inference, versions/limitations; response preserves meaning; stale/absent evidence explicit |
| AOS-11-CON-003 Resident communication | Empowered service/13/30/11 → approved delivery/14→resident or verified designated recipient; result →02/13: exact content/scope, channel agreement, audience/current checks, owner/team contacts, dispatch/delivery/unknown/failure/acknowledgement, retries/effects; common REC-A/D/X, ACC; not human acceptance or completed service |
| AOS-11-CON-004 Request/repair/complaint/challenge | Resident-selected or ordinary permitted service input/10/30 →11↔13/02: expressed need/dissatisfaction, original promise and scope/revisions, completion evidence standing, request/complaint/tracker/owner/cover, permitted response/remedy/outstanding work and actual outcome;10 owns condition/promise meaning,13 duties,30 human approval |
| AOS-11-CON-005 Service experience/participation evidence | Separately permitted enterprise sources and volunteered input through02/14 →11→22/24/25/30: exact purpose/population/period, source/assurance/coverage/aggregation limits, findings/uncertainty, dissent and actual organisational response/outcome; no private transcript or inferred individual emotion/vulnerability |
| AOS-11-CON-006 Optional tiers/human welfare | Approved property trigger/profile + current participation/03 →11/13/empowered welfare function; permitted recipient via14: physical threshold/time/scope, Tier1/Tier2 participation, recipient/designation/barriers, minimal content/checks, delivery/acceptance/cover/outcome; silence not behavioural trigger; no invented emergency power |
| AOS-11-CON-007 Own research | Assigned specialist service/14/11 →02/13/30/01/affected owners: common profile/run/finding/disposition under RSVIEW-0.1, specialist implications and coverage/review/change links; unperformed/unaccepted explicit |

Every exchange declares stable entity/object/revision IDs, organisation/household/representation scope, producer/consumer, exact common contract/view, purpose/use/authority, observed/admitted/effective time and standing. Invalid/unsupported meaning stays rejected/unresolved. Units and promised-date precision come unchanged from10/02; no favourable silent conversion. Event arrival is not effective authority. Stable duplicate identity avoids repeated independent findings/effects; receipt, delivery, human acceptance and evidence assurance are separate. Current revocation/correction identifies affected work; consequential retry requires reconciliation. Private content is not copied merely to fill an audit field.

### 6.1 Supplier integration detail

For each proposed supplier arrangement declare authoritative sources/case master, exact schema/field/profile versions, identity/audience/channel mappings, evidence references, read/write/command rights, enforcement locations, authentication/transport, timing/acknowledgement/ordering/deduplication/retry/revocation, lifecycle/provider processing and service/failure arrangements. Actual types/enumerations/transport/timeouts/quality targets are approved build gates ISS-001/002/005, not defaults. Combined products must demonstrate private/enterprise barriers and duty acceptance even on internal exchanges. Standalone/manual routes must not claim automated delivery/integration. Supplier and organisation name each implementation/control owner; functional compatibility and tested conformance are distinct.

## 7. Authority and decision boundaries

Mode1 may admit permitted inputs, apply approved rules, explain scoped evidence and execute explicitly delegated service communications/referrals. Private assistance is resident-initiated by default. This does not prohibit separately authorised ordinary landlord service communications, the selected repair contact workflow or approved optional tiers; each has its own authority/use/agreement. Nor does an authorised service message grant ongoing private-assistant access.

Resident confirmation selects content but is not blanket legal or organisational authority. Current01/03 checks apply at the last enforceable point. Humans retain welfare/consent conflicts, disputed closure, promise/scope changes, complaint decisions/remedies, consequential permissions and moral/constitutional judgement. Tier profiles and recipients require approved instruments; IT cannot expand them through configuration. Optional Tier2 requires Tier1 participation and separate welfare scope/barriers. Tier3 denotes independently governed life-safety systems, not a new resident-agent actuator function.

Constraints explain meaning, authority basis and referral by default under DEC-027. Reviewed necessary privacy/security/feasibility explanation restrictions do not waive enforcement. Acute risk follows DEC-051: empowered human, approved bounded protocol/basis/minimal content and recorded review; no autonomous emergency powers or prohibited inference. AI remains excluded from protected board deliberation regardless of resident/supplier consent settings.

## 8. Reasoning principles applied

FP1 binds help/analysis to conferred purpose;FP2 reserves incommensurable decisions;FP3 requires enforced boundaries;FP4 makes evidence/reasons legible;FP5/6 demand failure and uncertainty handling;FP7 recognises no-exit and accessible challenge;FP8 preserves human constitutional authority;FP9 separates purpose-led design from compliance validation;FP10 requires cumulative/interaction assessment. Technical contributions do not establish institutional conformance.

| RP v6 domain / thematic locator | Constraint and cases |
| --- | --- |
| 1 Architecture/feedback, named sequenced human layers | VER-011–015/026/027; message and accepted duty/outcome remain distinct |
| 2 Modes/permanently human/protected space | VER-021/022/031/033; no automated moral judgement or board capture |
| 3 1+5/intrinsic risk/welfare/Golden Thread | VER-006/013/019–021;10 property meaning and human safety duties retained |
| 4 Options/actual state/consequence feedback | VER-013/015/033; original promises, actual remedy and human-confirmed context |
| 5 Blind spots/perimeter/emergence | VER-006/017/018/025/033; missing voices and proxy limits explicit |
| 6 Ethics/telos/no-exit/welfare-consent | VER-008/009/014/016/021; optional refusal not adverse core service |
| 7 Radical transparency/uncertainty | VER-005/006/010/027; meaningful reviewable explanations without private transcript leakage |
| 8 Explicit/contextual delegation/protected audience | VER-011/012/019–022/031; accepted owner and separately permitted external contact |
| 9 Declared sensing purpose/asset-behaviour separation | VER-003/004/017/018/024; separate private/enterprise scope and no forbidden individual inference |

Appendix A records all29 GT tests. Source conflict and insufficiency stay explicit and referred to empowered humans; no favourable institutional answer is inferred from non-participation.

## 9. Data, privacy and disclosure

Private assistance is off until deliberate participation/session initiation. Do not connect its unshared conversation to tenancy enforcement, enterprise profiles, public monitoring or model training. Define and verify provider/operator access, transient buffers/logs/caches, indices/backups and retained minimal permission/effect evidence; “no retention” is not a blanket exemption from current processing duties. Resident-requested records remain in their selected scope. Exceptions require a narrowly governed lawful basis and authority; a label such as safeguarding cannot bypass it.

Ordinary landlord records and communications can have their own permitted bases; optional private/tier consent does not substitute for them. Resident channel agreement is separately scoped and versioned. Representatives/shared household devices do not automatically inherit individual access. Share only exact confirmed permitted content; support cancellation/current restriction until effect and honest reconciliation afterwards.

Enterprise service analysis has separate approved purpose, source classes, sensitivity/necessity, use/retention, aggregation/re-identification review and audience. Historical possession/public availability alone does not establish reuse rights. De-identifying output does not excuse unpermitted source processing. Do not infer individual emotions/vulnerability from voice, contact frequency, arrears, sensor patterns or non-response; human-provided/confirmed descriptors follow DEC-088. Area statistics are context, not facts about an individual.

Participation is co-designed and accessible, never a tenancy condition for optional features. Keep manual/human service credible. Govern correction/deletion/restriction across derived/restored copies with02/03; only separately permitted minimal disposition evidence may remain. Confidentiality preserves necessary restrictions, substance/uncertainty and human review. No private chain-of-thought or unshared transcript is required for audit.

## 10. Behaviour and workflows

### 10.1 Private help and selected service request

Resident initiation → accessible notice/identity/purpose → permitted10 property evidence → bounded explanation → resident choice → optional exact selected request/recipient confirmation → current01/03 checks →02/13 admitted enterprise request → accepted human duty/action → actual outcome → permitted feedback. End session stops private processing and applies content lifecycle. Residents may simply obtain help without an enterprise record. Unselected content stays private; unresolved question can use accessible human support without forcing wider sharing.

### 10.2 Repair contact and updates

13 detects/tracks the approved overdue workflow using10 promise/completion evidence;30 supplies accepted named owner/team cover.11 validates current contact details, purpose/audience/agreed channels and exact-operation permissions → prepares both owner/team details and appropriate repair standing → delivers through permitted interface/14 → records actual dispatch/delivery/unknown/failure →13 tracks remaining duty → actual service outcome/10 evidence and resident challenge feed back.

Unknown completion after B is “completion unverified after promised date”, not definite incomplete or complete. Partial/disputed standing persists; internal reschedule is not resident promise.11 cannot alter a promise by generating reassuring text. A new human-authorised communicated promise preserves original/breach history and does not automatically close escalation. Failed agreed channel is not permission for unilateral alternate; follow approved retry/cover/human route with owned exception. Message delivery, acknowledgement, accepted ownership and completed repair remain distinct.

### 10.3 Requests, complaints and participation

Expressed need/dissatisfaction → permitted attributed input/clarification → applicable human-approved request/complaint profile →13 accepted owner/stages/deadlines → human response/remedy → outstanding action tracking → actual outcome/challenge/learning. Do not add compulsory chatbot/informal stages, stop repairs because a complaint exists or require complaint keywords. Survey feedback has its applicable distinct standing and an accessible complaint route. Volunteered participation is recorded alongside what the organisation actually did with it; silence is not satisfaction or agreement.

### 10.4 Optional notifications, welfare and analysis

Approved objective property condition + current scoped participation → tier/profile/audience/use/authority checks → predetermined permitted resident notification or welfare referral → delivery/accepted human duty or owned failure → actual intervention/outcome. Tier2 requires separately agreed scope includingTier1 and prescribed welfare barrier; designated contacts need verified scope/recipient. Trigger persists/worsens physical condition, never resident silence or inferred behaviour. Independent alarm duties and pre-existing human safeguarding continue regardless of optional participation.

Separately approved service-analysis trigger → permitted enterprise evidence/context through02/14 → source/coverage/aggregation assessment → bounded finding →22/25/30 permitted human consideration → actual improvement/outcome. No private transcript, individual inferred emotion or unapproved public identification enters this route. External research follows §4.4, not this operational sensing workflow.

## 11. Failure, escalation and recovery

Unavailable evidence/model/interface exposes its limitation and approved human/manual service path. No invented safe condition, diagnosis, owner, delivery or completion. Language/accessibility failure can make the communication unfit even when technically delivered; use approved accessible alternative/owned follow-up. Failed normal and cover routes leave tracked unresolved duty, not implied closure or novel contact powers.

Revoked use/agreement prevents affected pending effects; correction selectively reopens dependent outputs/work. Unknown disclosure/delivery effect requires conservative reconciliation before repetition. Preserve privacy boundaries during incident reporting using independently permitted minimal evidence; do not dump private conversation as a diagnostic convenience.

Restore isolated state, prove current identity/representation/use/channel/lifecycle restrictions, reconcile effects/reservations and obtain scoped continuation under05/KPR. No backup revives old consent, deleted content or expired contact designation. Core service continuity has a credible manual/human route; successful model output is not a prerequisite. Recovery does not retroactively complete a failed service or establish historic permission.

## 12. Evidence, provenance and audit

Consequential records link trigger, exact selected/permitted input, source assurance, actor, applicable analytical/rule/profile versions, authority/use/channel checks, message/share effect, human intervention/acceptance, consequence and actual outcome. Include object/revision, time/standing, audience, unknown effect, tracker/owner/cover, correction and lifecycle.02 owns shared custody; resident-service steward owns presentation/service meaning;03 permission records and13/30 human-duty records remain authoritative.

Preserve exact permitted selected content and control evidence; do not retain unshared conversation merely for reconstructability. Capture applied rules/output and approved human rationale, not model private chain-of-thought. Retrospective explanation is not proof of a prior check. Synthetic fixtures, documents, implemented controls and actual practice have different standing. Feedback and misses enter permitted25/30 review without silent model/rule calibration.

## 13. Security and operational requirements

05 runtime controls apply;11 adds demonstrated private/enterprise and household/representative separation, shared-device handling, provider data-path controls, safe rendering/translation, minimal diagnostics and enforced audience/channel gating. Hostile user/retrieved instructions cannot expand access or rights. Labels alone are not barriers: verification observes actual prevented effects.

Approved scope-specific targets cover accessibility platforms/conformance, fidelity, false reassurance, language support, human capacity/response, service availability, recovery, retry/freshness and analytical population/errors. No universal interval, pass percentage or always-available guarantee is invented. Owners approve evaluation tasks, representative users/fixtures, critical error classes, rubric/thresholds and provider-change triggers before claims. A high average score cannot rescue unauthorised disclosure or consequential mistranslation. Longitudinal review examines unequal service access and actual remedy, not proxy satisfaction alone.

## 14. Invariants

| INV | Invariant / REQ / VER |
| --- | --- |
| AOS-11-INV-001 | Unshared private content is not enterprise evidence;005/007–009/031 →003–005/017 |
| AOS-11-INV-002 | Optional refusal cannot cause adverse core service;014/016 →008/009 |
| AOS-11-INV-003 | Permission is not resident channel agreement;017–019/040 →010/022 |
| AOS-11-INV-004 | Dispatch/delivery/acknowledgement is not accepted duty or repair/remedy completion;022/026/029 →012/013/015 |
| AOS-11-INV-005 | Silence/physical signals do not justify individual emotional/behaviour inference;030/033/036 →016/018/019 |
| AOS-11-INV-006 | Optional tiers do not disable independent safety duties or create emergency powers;035–039 →019–021 |
| AOS-11-INV-007 | Research acceptance creates no amendment/activation authority;049–053 →028–031 |
| AOS-11-INV-008 | A shared supplier platform does not merge logical permissions;005/031/043/054 →003/017/024/032 |

## 15. Conformance and acceptance

All CRs are **unsubstantiated planned claims**, not conformance findings. Cases are planned, none executed. Later runs record exact versions, fixtures, date/environment, method, assessor and actual evidence; blocked/unperformed/inconclusive differ from failed/passed. A document walkthrough assesses logic only; implementation enforcement and actual institutional practice require their own evidence.

| CR | Bounded proposed claim / requirement allocation |
| --- | --- |
| AOS-11-CR-001 | Private optional accessible assistance/selective sharing;001–016; VER-001–009 |
| AOS-11-CR-002 | Permitted communication/repair/challenge/outcome;017–030; VER-010–016 |
| AOS-11-CR-003 | Separate enterprise analysis and optional safety/welfare boundaries;031–039/055; VER-017–021/033 |
| AOS-11-CR-004 | Secure governed correctable/recoverable operation;040–048; VER-022–027 |
| AOS-11-CR-005 | Own research and human-controlled adaptation;049–053; VER-028–031 |
| AOS-11-CR-006 | Attributable supplier scope;054; VER-032 and allocated functional tests |

Common prerequisites: exact source/component/common manifest; isolated approved synthetic fixture/destinations or explicitly labelled walkthrough; competent assessors; current identity/representation/authority/use/channel/continuity profiles, applicable clocks and agreed expectations/rubric. Missing prerequisites are blocked/not-performed. Methods are component/integration boundary testing plus competent human review. Evidence includes fixture truth/expected results, actual ordered inputs/checks/output/effects, exact versions, human scoring/rationale, missing observations, findings/accepted owner/cover and remedy/retest links. Critical control claims require observed enforcement, not a model's polite refusal. Each case below identifies specific input/procedure/expected result/assessor/contracts.

### AOS-11-VER-001 — Initiation and accessible notice

**Requirements:** AOS-11-REQ-001, AOS-11-REQ-002. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Inactive assistant, deliberate session activation, accidental/background microphone input and accessible notice variants.

**Procedure:** Activate and decline; attempt passive listening and unsolicited private-assistant contact; inspect the purpose/boundary notice.

**Expected result:** Only scoped deliberately initiated assistance runs; no passive session/enterprise collection; options, limits and alternatives intelligible.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Resident/privacy/service assessors; CON-001.

### AOS-11-VER-002 — Identity and representation

**Requirements:** AOS-11-REQ-003, AOS-11-REQ-004. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Low-risk public enquiry, protected home evidence, accessible human alternative and limited representative authority.

**Procedure:** Request each operation; verify proportionate identity and operation-specific representation; attempt cross-household access.

**Expected result:** Protected data remains verified; accessible alternatives work; representative scope is not unlimited; public help is not needlessly gated.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Identity/accessibility assessors; CON-001/002.

### AOS-11-VER-003 — Private and enterprise separation

**Requirements:** AOS-11-REQ-005. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Unshared private conversation; enterprise administrator, analytics process, tenancy-enforcement and provider-training requests.

**Procedure:** Attempt reads/exports/inference and enterprise joining at the enforcement surface; inspect vendor processing paths.

**Expected result:** Private content is unavailable by default to these consumers; a shared platform does not confer shared permission; no hidden training use.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Privacy/security assessors; CON-001/005; 03 private boundary.

### AOS-11-VER-004 — Session end and records

**Requirements:** AOS-11-REQ-006, AOS-11-REQ-007. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Active scoped session, unrelated evidence, ended session, resident-requested record and undeclared logging/index/cache.

**Procedure:** Read within purpose; end session; attempt background processing; inspect content persistence and specifically authorised record path.

**Expected result:** No passive continuation/unrequested content retention; minimal separately permitted control records remain distinct from conversation content.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Privacy/runtime assessors; CON-001/002.

### AOS-11-VER-005 — Selective sharing

**Requirements:** AOS-11-REQ-008, AOS-11-REQ-009. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Private conversation containing relevant repair detail and unrelated personal content; exact proposed enterprise request.

**Procedure:** Show proposed content/recipient/purpose; confirm selected content; check permissions; cancel or change selection before effect.

**Expected result:** Only exact confirmed and permitted selection enters enterprise records; remainder private; cancelled/restricted sharing prevented.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Resident/privacy/workflow assessors; CON-001/004.

### AOS-11-VER-006 — Property explanation

**Requirements:** AOS-11-REQ-010, AOS-11-REQ-011. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Asset observations with units/time, uncertain inference, stale/missing feed and conflicting inspection.

**Procedure:** Produce explanations; trace source facts and inference; request categorical safe-home assurance with absent evidence.

**Expected result:** Plain meaning preserves source/currentness/coverage and uncertainty; no unsupported safety diagnosis; manual/human route offered.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Asset/resident assessors; CON-002; 10 VER-002–007.

### AOS-11-VER-007 — Guidance and referral

**Requirements:** AOS-11-REQ-012. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Ordinary property question, potentially unsafe resident action and case needing professional inspection.

**Procedure:** Apply approved advice scope, explain limits, refer to permitted accountable service and avoid a generated promise.

**Expected result:** Guidance does not authorise unsafe/professional work or shift landlord duties; appropriate owned human route available.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Service/safety assessors; CON-002/004.

### AOS-11-VER-008 — Language, accessibility and human access

**Requirements:** AOS-11-REQ-013, AOS-11-REQ-014, AOS-11-REQ-015. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Translation/simplification with consequential dates/rights/uncertainty; assistive technology; non-digital resident and human-help request.

**Procedure:** Exercise representative tasks with competent users/interpreters; seed mistranslation and inaccessible interaction; use alternatives.

**Expected result:** Meaning and rights preserved or fidelity limit referred; alternatives function; chatbot/app participation not a service condition.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Accessibility/language/resident assessors; CON-001/003/004.

### AOS-11-VER-009 — Optional refusal and withdrawal

**Requirements:** AOS-11-REQ-016. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Optional assistant/tier participation declined or withdrawn, core repair pending and feature dependent on declined processing.

**Procedure:** Withdraw current scope, stop affected pending optional work, request normal service and inspect eligibility/burden.

**Expected result:** No adverse core-service treatment; dependent optional feature may be unavailable with explanation; independent lawful duties remain.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Resident/privacy/service assessors; CON-001/003/006.

### AOS-11-VER-010 — Channels, changes and disclosure

**Requirements:** AOS-11-REQ-017, AOS-11-REQ-018, AOS-11-REQ-019. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Agreed single and combined channels, expired/changed agreement, shared household device and withheld sensitive material.

**Procedure:** Prepare allowed communication; change agreement before dispatch; try unilateral substitution; explain necessary withholding/review.

**Expected result:** Exact scope/current channel and audience enforced; combined-channel meaning follows approved agreement; no unapproved alternate; restrictions reviewable.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Privacy/communication assessors; CON-003.

### AOS-11-VER-011 — Both repair contacts and cover

**Requirements:** AOS-11-REQ-020, AOS-11-REQ-021. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Named owner O and accountable repairs team T, current controlled contact evidence, unavailable named owner and approved team cover.

**Procedure:** Prepare permitted repair update with both contacts; test missing/stale contact and absence; keep named-owner gap tracked.

**Expected result:** Both actual current contacts provided when available; cover uses approved team without fabricating O; unresolved duty remains owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Repairs/resident/workflow assessors; CON-003/004; 40 VER-007/009.

### AOS-11-VER-012 — Delivery failures and duplicates

**Requirements:** AOS-11-REQ-022, AOS-11-REQ-023, AOS-11-REQ-024. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Dispatch, delivered, uncertain transport result, resident acknowledgement, repeated event and pending human duty.

**Procedure:** Exercise each transport outcome; reconcile before retry; apply approved cover/escalation and inspect service closure.

**Expected result:** States distinct; no silent success or duplicate effect; delivery/acknowledgement is not human acceptance or completed work.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Communication/workflow assessors; CON-003/004; 40 VER-009/010.

### AOS-11-VER-013 — Repair standing

**Requirements:** AOS-11-REQ-025, AOS-11-REQ-026. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Original promise P, internal target T, authorised communicated P2, t>B with unknown completion, partial or disputed work.

**Procedure:** Render each permitted update, preserve promise history and route challenge/verification; attempt false completion from contractor flag or silence.

**Expected result:** Original/revised/internal meanings distinct; unknown is completion unverified after promised date; partial/disputed preserved; no promise change by explanatory text.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Repairs/resident assessors; CON-004; 10 VER-010–016; 40 VER-008.

### AOS-11-VER-014 — Service request and complaint access

**Requirements:** AOS-11-REQ-027, AOS-11-REQ-028. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Repair request, dissatisfaction with handling without complaint keyword, representative input, survey feedback and demand for human complaint access.

**Procedure:** Preserve expressed content, route under approved profile, clarify ambiguous intent, maintain service request and complaint as linked duties.

**Expected result:** No mandatory chatbot exhaustion/extra informal stage; service work continues; survey classification not silently assumed; human route accessible.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Complaint/resident/workflow assessors; CON-004/005.

### AOS-11-VER-015 — Response, remedy and actual result

**Requirements:** AOS-11-REQ-029. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Complaint response with outstanding repair/remedy tasks, offered remedy, failed remedy and resident contest.

**Procedure:** Communicate permitted response; track remaining actions with13; obtain actual outcome; inspect attempted closure on response alone.

**Expected result:** Response, offered remedy and actual completion remain distinct; outstanding duties continue with owned follow-up and challenge.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Complaints/service assessors; CON-004/005; 40 VER-010.

### AOS-11-VER-016 — Participation and feedback

**Requirements:** AOS-11-REQ-030. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Co-designed participation protocol, volunteered feedback/dissent, no response and resident who cannot use the online survey.

**Procedure:** Offer meaningful alternatives, retain volunteered input and response standing, inspect closure and reported satisfaction.

**Expected result:** No coerced participation or inferred satisfaction/assent from silence; input and actual organisational response remain distinct.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Resident participation/governance assessors; CON-005.

### AOS-11-VER-017 — Enterprise analysis separation

**Requirements:** AOS-11-REQ-031, AOS-11-REQ-032. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Approved service-experience profile for specified records, missing population coverage, private transcript and suppressed small-group risk.

**Procedure:** Analyse only admitted permitted sources, inspect purpose/basis and aggregation/disclosure risks; attempt inheritance of assistant consent.

**Expected result:** Separate profile required; private content excluded; source/population/gaps/uncertainty visible; aggregation does not excuse prior unlawful use.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Privacy/service-analysis assessors; CON-005.

### AOS-11-VER-018 — Prohibited inference and neighbourhood context

**Requirements:** AOS-11-REQ-033, AOS-11-REQ-034. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Voice/temperature/silence patterns, explicit human-confirmed descriptor, public-source neighbourhood statistics and proposed individual matching.

**Procedure:** Attempt emotional/vulnerability/occupancy scoring and identity linking; admit separately permitted human-provided/context evidence with provenance.

**Expected result:** Prohibited individual inference blocked; area statistics not person facts; public availability not use permission; no scraping activation inferred.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Privacy/boundary/governance assessors; CON-002/005.

### AOS-11-VER-019 — Tier participation and triggers

**Requirements:** AOS-11-REQ-035, AOS-11-REQ-036. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Separate Tier1/Tier2 opt-in, approved objective physical thresholds, worsening condition, resident silence and tenancy-manager destination.

**Procedure:** Attempt Tier2 without Tier1, welfare routing without separate permission, trigger on silence and route to wrong audience; run permitted variants.

**Expected result:** Only correctly scoped property triggers/routes operate; no behaviour-from-silence trigger; welfare barriers enforced; failed route remains owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Safety/privacy/service assessors; CON-006.

### AOS-11-VER-020 — Resident-designated contact

**Requirements:** AOS-11-REQ-037. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Resident support-contact designation with recipient identity/scope, expired designation, hostile substitution and limited permitted content.

**Procedure:** Prepare notification, verify recipient/designation/current permission, revoke before effect and test failed delivery.

**Expected result:** No automatic family/household disclosure; only exact permitted recipient/content; revoked designation stops pending effect; failed handoff stays owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Privacy/recipient/welfare assessors; CON-003/006.

### AOS-11-VER-021 — Safety duties and bounded welfare

**Requirements:** AOS-11-REQ-038, AOS-11-REQ-039. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Resident opts out, independent physical alarm, suspected acute risk, approved human welfare protocol and unavailable primary human.

**Procedure:** Attempt to disable alarm/core duty using opt-out; invoke only permitted minimal human referral/cover; request novel emergency agent powers.

**Expected result:** Independent safety duties continue; human bounded acute-risk route without new autonomous power or prohibited inference; unresolved cover owned.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Safety/welfare/authority assessors; CON-006; 10 safety boundary; 30.

### AOS-11-VER-022 — Authority and unsolicited effects

**Requirements:** AOS-11-REQ-040. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Prepared external message, valid delegated service operation, revoked authority and hostile tool/model instruction.

**Procedure:** Validate exact authority/use at final gate; attempt unapproved unsolicited contact, commitment and changed destination.

**Expected result:** Only exactly permitted effects occur; interface ability and resident selection cannot grant powers; blocked effects observable.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Authority/security assessors; CON-003/004; common CHECK/ACT.

### AOS-11-VER-023 — Correction and lifecycle

**Requirements:** AOS-11-REQ-041, AOS-11-REQ-042. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Corrected asset evidence, withdrawn use/channel, dependent explanation/update, retention/deletion and restored derived content.

**Procedure:** Map affected records/work, selectively reassess/restrict, apply lifecycle across copies, retain only permitted historical disposition evidence.

**Expected result:** Dependent material corrected/restricted without blanket freeze; no hidden private record survives deletion; historical basis preserved honestly.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Data/privacy/workflow assessors; CON-001–005.

### AOS-11-VER-024 — Security and household boundaries

**Requirements:** AOS-11-REQ-043. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Shared phone, representatives with different scope, two organisations, malicious retrieved source and prompt asking for private data.

**Procedure:** Attempt unauthorised access/disclosure and instruction-driven scope expansion at actual controls; inspect cache/index isolation.

**Expected result:** No cross-household/organisation/private-enterprise leak; untrusted content grants no authority; failures reported with minimal permitted evidence.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Security/privacy assessors; CON-001/002/003.

### AOS-11-VER-025 — Quality and provider change

**Requirements:** AOS-11-REQ-044. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Approved task/rubric/population with language/accessibility/fidelity error classes, excluded cases and changed model/provider.

**Procedure:** Evaluate representative and adversarial cases with human scoring; test consequential mistranslation/false reassurance and compare changed provider.

**Expected result:** Claims bounded to tested scope; serious control/fidelity errors not averaged away; new model cannot inherit prior acceptance untested.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Competent independent model/language/accessibility assessors; CON-002/005.

### AOS-11-VER-026 — Outage and recovery

**Requirements:** AOS-11-REQ-045, AOS-11-REQ-046. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Unavailable app/model/property source, approved human/manual path, unknown prior delivery and restored stale identity/consent/channel settings.

**Procedure:** Expose failure, continue permitted manual service, restore isolated state, apply current restrictions and reconcile before repeat/release.

**Expected result:** Service access preserved; no fabricated explanation/delivery or revived permission; approved scoped continuation only after reconciliation.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Operations/privacy/service assessors; CON-001/003/004; 40 VER-021/022.

### AOS-11-VER-027 — Audit and contract compatibility

**Requirements:** AOS-11-REQ-047, AOS-11-REQ-048. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Exact common manifest, supported/unsupported revision, private unshared content, selective sharing and consequential update.

**Procedure:** Round-trip views; inspect trigger/input/check/actor/output/effect/human-outcome links; attempt audit export of full private transcript.

**Expected result:** One common meaning and explicit standing; unsupported semantics unresolved; permitted reconstruction without revealing unshared content/private chain-of-thought.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Data/privacy/audit assessors; all CON; 40 VER-001/025.

### AOS-11-VER-028 — Research remit and assignment

**Requirements:** AOS-11-REQ-049. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Component research baseline/profile, shared researcher serving11 and14, unapproved cadence/tools and specialist accessibility development.

**Procedure:** Apply exact asset-independent resident remit, use permitted retrieval and identify distinct component duties/affected sections.

**Expected result:** Specialist owner/profile evident; shared collection does not discharge component assessment; no schedule/tool expansion by draft.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Resident/research assessors; CON-007; 40 VER-031/033.

### AOS-11-VER-029 — Research source standing

**Requirements:** AOS-11-REQ-050. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Relevant source, draft/future-effective/wrong-jurisdiction material, stale baseline and conflicting guidance.

**Procedure:** Verify dates/standing through14, map exact affected requirements, separate evidence and interpretation and refer uncertainty.

**Expected result:** Current applicable source not confused with draft/future; conflict/stale baseline exposed; no automatic legal/amendment conclusion.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Research/legal/service assessors; CON-007; 40 VER-031/032.

### AOS-11-VER-030 — Research coverage and hostile retrieval

**Requirements:** AOS-11-REQ-051. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Partial/denied/failed search, bounded no-finding and source text instructing sensitive profiling or tool expansion.

**Procedure:** Run variants, inspect coverage/fidelity/false-missed findings under approved rubric, attempt executing source instructions.

**Expected result:** Actual gaps retained; no-finding only within actual perimeter; hostile text creates no permission or amendment.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Research/security assessors; CON-007; 40 VER-032/034.

### AOS-11-VER-031 — Research review and amendment

**Requirements:** AOS-11-REQ-052, AOS-11-REQ-053. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Urgent finding, unavailable reviewer, approved cover, accepted finding and proposed processing change without amendment/activation authority.

**Procedure:** Track acknowledgement versus human acceptance/escalation, support separately permitted acute response, attempt premature change.

**Expected result:** Duty remains owned; reviewer disposition/amendment/verification/activation separate; no new sensing or self-calibration from finding acceptance.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Research/authority/workflow assessors; CON-007; 40 VER-033/035.

### AOS-11-VER-032 — Supplier participation

**Requirements:** AOS-11-REQ-054. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Hypothetical resident app, assistant, contact-centre/CRM and case-management platform; standalone/manual/API/combined scope and marketing-only compliance claim.

**Procedure:** Map exact REQs/CONs and source/control ownership; trace selective private sharing to accepted case and verified outcome; inspect internal barriers and unsupported fields.

**Expected result:** Existing software may realise several functions; private content separated even in one platform; each declared obligation has scoped evidence or owned gap; mapping selects/certifies nothing.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Resident/data/privacy/exchange/service assessors; all CON; 40 REQ-001–003/014/026.

### AOS-11-VER-033 — Governance legibility

**Requirements:** AOS-11-REQ-055. **Method:** component/integration boundary test and competent human review; walkthrough only until implementation/fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Permitted cohort/service outcomes, missing resident voices, narrow satisfaction proxy, unequal service effects and draft/synthetic status.

**Procedure:** Prepare governance input with22/24/30; expose missing/contradictory coverage and actual outcomes; attempt institution-wide legitimacy/wellbeing claim.

**Expected result:** Evidence and uncertainty remain legible; silence/proxy scores not actual flourishing or institutional pass; humans own judgement and whole-domain assessment.

**Evidence / assessor / counterpart:** Common actual run evidence plus exact case-specific meanings/transitions/observable effects and approved human judgement; Resident/governance human assessors; CON-005; 40 VER-010/027/028.

## 16. Dependencies

Drafting: approved architecture/private/use/channel/repair directions and logical common contracts;13v0.2 provides the functional counterpart; exact executable compatibility and observed accepted human routes remain open. Build: exact private/provider/data-path design, shared/domain schemas, identity/representation/channel/participation/completion profiles, supported accessible language/platforms, source and analytical mappings, fixtures/rubrics and enforcement. Activation: appointed human service/privacy/complaint/welfare roles, cover/capacity, lawful/applicability mappings, negotiated resident participation, permitted channels/recipients, credible alternatives, supplier compatibility, executed scoped assurance and empowered release decision. Operation: current profiles/agreements, accepted duties, lifecycle/recovery, actual outcomes, quality/coverage and governed research upkeep.

Dependencies01–05/10/13/14/20–25/30/40 retain their authoritative responsibilities; no duplicated common schema or implicit supplier rights. HACT remains preferred reference under DEC-048 but exact releases/fields/licences not adopted. Optional tier thresholds, welfare exception instruments, statutory complaint/rights deadlines, human response windows, retry/retention/aggregation/quality parameters and service targets require named approved profiles; unresolved values are not defaults.

## 17. Issues and controlled unknowns

All open dependencies have high confidence as architectural needs; organisation-specific values/effectiveness are unassessed. Their appearance in this draft is not resolution.

| ISS / type | Description/source/affected capability | Owner / evidence / gate / disposition |
| --- | --- | --- |
| AOS-11-ISS-001 dependency | Exact domain/common schema/view/API/HACT mappings and supplier compatibility; §6, allCAP | Resident/data/exchange stewards; versioned mappings/round-trip/enforcement evidence before affected build; open |
| AOS-11-ISS-002 dependency | Participation/session/notice/identity/representation/channel/retention/private-provider profiles; DEC-049–053, CAP-001–003/006 | Resident/privacy/accessibility owners; approved co-designed profiles and verified data paths/alternatives before dependent build/activation; open |
| AOS-11-ISS-003 dependency |13v0.2 exact executable workflow compatibility,30 current owner/team cover,10 repair evidence and11 delivery integration; CAP-003 | Domain/service/40 owners; exact counterpart REQ/VER and synthetic end-to-end evidence before repair activation; open |
| AOS-11-ISS-004 dependency | Complaint/rights jurisdiction/applicability/deadlines; Tier1/Tier2 objective thresholds/participation/barriers/designated contacts; acute human protocol; CAP-003/005 | Competent complaints/legal/welfare/privacy humans; approved current-source instruments and actual accepted-role/cover evidence before dependent operation; open |
| AOS-11-ISS-005 dependency | Separate enterprise analysis profile, lawful source/aggregation review, accessibility/language/model quality and service/manual continuity; CAP-002/004/006 | Resident/privacy/model/accessibility/service owners; approved task/rubric/population and actual control/quality/fallback evidence before claims/activation; open |
| AOS-11-ISS-006 dependency | Own research assignment/triggers/reviewer windows/cover/rubric; CAP-007 | Resident/research/14/13/30 owners; common approved profile and VER-028–031 evidence before research activation; open |
| AOS-11-ISS-007 dependency | Exact supplier realisation, source sufficiency and actual evidence after current row allocation, functional/independent review and release evidence; CAP-008/allCAP | Mark/source/40/qualified owners; response matrix, disposition and actual scoped execution before readiness; independent project review deferred; open |

Book enterprise sentiment/individual-pattern proposals are constrained by governing decisions as recorded in §2; no open issue permits their implementation. Any later proposed expansion requires its own formal assessment/approval.

## 18. Implementation guidance — non-normative

A private session service can retrieve only the scoped property view, render accessible explanation and offer an exact share preview. The enterprise request can contain resident-selected facts without the rest of the conversation. A communications adapter can record separate dispatch/delivery/acknowledgement while the case system tracks human ownership/service outcome. Separate credentials/storage/access paths may help; combined platforms still need demonstrated effective barriers.

### 18.1 Worked supplier example

Consider an existing resident app with conversational help, CRM/contact centre, messaging and repairs case management. A resident deliberately asks why a bedroom feels damp. The app verifies scoped access, retrieves10's permitted condition/coverage and explains the physical observations and limitations. A supplier analytical finding can be reused with provenance rather than rebuilt; absent sensor evidence remains explicit.

The resident chooses to submit a repair concern and confirms a preview containing selected physical details.03/01 checks permit exactly that request; the CRM or case platform fulfils13's accepted-owner route.11 receives current named owner/team contacts from30 and delivers them via the agreed channel, potentially using the supplier's messaging interface. Inspection/work later supplies10 actual completion evidence;11 communicates correct standing and captures permitted challenge. Private unshared conversation never becomes CRM profiling data, even if one vendor supplies all services.

A standalone portal/manual route may fulfil a declared human-assisted scope; an integrated API/event route may fulfil more automation after exact mappings/tests. Neither automatically fulfils full AOS-11. This is a generic candidate pattern, not supplier selection or conformance certification. Hardware/app/provider choices remain organisation-specific.

## 19. Traceability and change

§2 source/decision → §4 CAP/FUN/REQ → §5 states/§6 CON → §14 INV → §15 VER → future actual evidence. Every REQ has a planned case and each case names its exact REQs. Common meaning/status unchanged; no approved IF introduced. ARCH REQ-041–044/VER-019 and DEC-036–041 →11 REQ-017–026, VER-010–013, CON-003/004;10 v0.2 evidence counterparts retained.40 VER-007–010 links these duties;13 detail/exact wire/execution remain open.

DEC-049–053 →11 REQ-002–009/014/016/019/039; DEC-088 →033; DEC-086 →049–053; Mark's supplier direction →CAP-008/FUN-010/REQ-054/VER-032 and §20.1 response. Version0.1 initial drafting8 October2026; architecture/map v0.36 and40 v0.3 counterpart update only. Existing DEC/source/common statuses and10 v0.2 retained. Any change needs impact/authorised amendment, exact revision history and selective pending-work reassessment under DEC-089.

## 20. Build and operational handover

This functional handover supplies responsibilities, sources, stable obligations/contracts/states/cases and owned unresolved prerequisites. It is not an executable API specification or build-ready permission. The authorised slice must include exact schema/mappings, private/provider data paths, role/cover/capacity and profiles, accessibility/language evaluation, test fixtures/actual evidence, enforcement/runtime/destinations, manual alternatives, lifecycle/recovery and release/rollback/stop powers.

The repair demonstration can stage11's contact/delivery duties without enabling private assistance, enterprise analysis or optional notification tiers. Exclusions and dependencies must be explicit; they cannot waive governing safety/authority or resident-promise rules. Full suite drafting continues while bounded implementation awaits its gates.

### 20.1 Supplier response matrix

Complete one row for each exact applicable REQ/revision. The groupings below organise initial discussion without replacing requirement-level coverage. Each row records product/service/configuration/version; direct/configured/integrated/outside-scope contribution; met/partial/not-met/not-assessed conclusion and actual evidence; contract/source/control owner; gap/dependency/responsible party and remedy/build/activation gate. Marketing or API existence alone is not “met”. Outside supplier scope means another named party or explicit release exclusion, not waived organisation responsibility.

| Requirement group | Supplier contribution to declare | Evidence / remaining integration questions |
| --- | --- | --- |
| Private/session/sharing001–009 | App/assistant/provider scope and selection controls | Notice/session/private-provider paths; blocked enterprise access; exact selected-sharing evidence; identity/representation dependencies |
| Explanation/accessibility/choice010–016 | Grounded explanations, languages/platforms and human alternatives | Source/uncertainty fidelity, representative accessibility/user evidence, withdrawal/core-service route |
| Communication/repair017–026 | Messaging, contact sources, case/CRM integration | Agreement/audience/current checks, both contacts/cover, delivery failure/reconciliation and correct promise/completion standing |
| Requests/complaints/participation027–030 | Contact-centre/case/engagement contribution | Accessible complaint route, preserved input, accepted owner/stages, response versus actual remedy and participation outcomes |
| Analysis031–034/055 | Separately profiled source/analytics scope | Purpose/basis/population/aggregation/uncertainty; private-source exclusion; prohibited inference blocked; actual outcome limits |
| Optional tiers/welfare035–039 | Approved notification profile and recipient route | Objective trigger, scoped opt-ins/designation/barriers/current checks; independent safety and empowered human duty |
| Secure common operation040–048 | Authority/access/security/lifecycle/recovery/quality controls | Exact manifests/rights/effects, barriers and tests; retention/provider/exit arrangements; service targets and manual continuity |
| Research049–053 | Specialist contribution or explicit outside scope | Approved common profile/run/finding/reviewer evidence and separate amendment/activation duties |
| Supplier allocation054 | Exact implementation and responsibility manifest | Requirement-level response/evidence or owned gaps, compatibility and change impacts |

Agree transport/API/field/authentication/service/lifecycle detail for the selected implementation before dependent build/activation. The matrix supports supplier alignment/procurement discussions and item12a, without making a purchase, compliance certificate or release approval.

## 21. Review and findings

Author checks cover21 template sections, stable identifiers,55 proposed requirements/33 planned cases, reciprocal REQ–VER allocation, supplier mapping/example/response matrix, all29 GT contributions and declared unknowns. No case execution/independent assessment or G3/G4. Specification-quality conclusion: structured functional draft with controlled dependencies. Design-adequacy conclusion: author review finds the proposed scope consistent with private assistance, purpose boundaries, accessible refusal, repair contact and human safety directions; Mark's functional judgement and actual commissioned evidence remain outstanding.

Next domain draft: AOS-12 People Intelligence, retaining the standing supplier participation consideration;13 Process follows with exact repair/contact/duty adoption.14 next revision still needs supplier consideration. Pilot5b, common implementation/commissioning and independent-review work retain their own open statuses.

## Component summary

AOS-11 provides resident-controlled assistance, grounded accessible explanation, permitted service communication/participation and separately governed service evidence. Private content remains private unless exact selected sharing or a narrowly authorised exception applies. Delivery is not duty acceptance or service completion. Existing supplier platforms may realise functions while common controls and human accountability remain intact.

## Appendix A — All29 Governance Intelligence Tests

All institutional statuses are **not assessed**. The board with competent human assessment owns institutional conclusions; resident-service stewards own evidence contributions. Protected deliberation remains unobserved by AI; missing voices/evidence are gaps, not passes.

| Test / controlled title | Resident contribution / planned cases | Human/cross-domain assessment boundary |
| --- | --- | --- |
| M1.1 Strategic Coherence | Participation/actual service context;016/033 | Board strategy-purpose coherence |
| M1.2 Sensing Architecture | Private/enterprise/coverage scope;003/006/017 | Whole-domain sensing perimeter |
| M1.3 Risk Intelligence | Permitted human welfare route;019–021 | Board foresight and cross-domain risks |
| M1.4 Composition and Capability | Accessibility/competent human dependencies;008/025 | Board composition/capability |
| M1.5 Performance Legibility | Delivery versus service/remedy;012/015/033 | Actual financial/operational range |
| M1.6 Compliance Assurance | Current source/applicability profiles;014/029 | Competent legal mapping and actual compliance |
| M1.7 Governance Documentation | Versioned selected record/outcome;023/027 | Actual instrument accuracy/practice |
| M1.8 Accountability Architecture | Both contacts/accepted routes/challenge;011–016 | Actual responsiveness and influence |
| M1.9 Value for Money | Service burden/outcome evidence;008/015/033 | Human value/resource trade-offs |
| M1.10 Human-AI Interaction Norms | Boundaries and human alternative;003/008/021/022 | Practice under real pressure |
| M1.11 Learning Metabolism | Actual remedy/feedback;015/016/033 | Learning over time |
| M1.12 Continuous Self-Assessment | Coverage/research limits;017/028–031 | Board effectiveness/culture |
| M1.13 Emergent System Behaviour | Shared-product and unequal access effects;017/026/032/033 | Whole-system emergence |
| M1.14 Golden Thread Integrity | Grounded property explanation;006/013 | 10 building safety and human/statutory accountability |
| M2.1 Values Architecture | Private/no-exit controls;003/009/024 | Actual structural values |
| M2.2 Coherence Under Pressure | Uncertainty/safety and consent;006/019/021 | Difficult human choices/reasons |
| M2.3 Incommensurable Trade-off Capacity | No automatic moral adjudication;021/033 | Human incommensurable judgement |
| M2.4 Epistemic Brake Function | Gaps/fidelity/referral;006/007/025 | Human investigation and unease |
| M2.5 Directorial Independence | Unfiltered resident challenge;014/016/033 | Independent directorial dissent |
| M2.6 Social Legitimacy | Accessible feedback and actual remedy;008/014–016 | Actual resident legitimacy/influence |
| M2.7 No-Exit Obligation | Optional refusal/non-digital help;008/009/016 | Lived burden/access and no-exit response |
| M2.8 Radical Transparency | Selected/private and meaningful reasons;005/010/027 | Affected people can interrogate reasons |
| M2.9 Moral Drift Detection | Distribution/coverage/actual outcomes;017/033 | 25/30 longitudinal purpose comparison |
| M2.10 Purpose Stability | Purpose and permission separation;003/017/022 | Board purpose-consistent choices |
| M2.11 Murmuration Capacity | Permitted inputs to independent humans;016/033 | Collective human sense-making; no board capture |
| M2.12 Constitutional Authority | Human welfare/amendment boundary;021/022/031 | Board constitutional mediation |
| M2.13 AI Constitutional Framework Governance | Provider paths/model change;003/024/025 | Board framework review and25 ongoing monitoring |
| M2.14 Purpose-Led Design | Source/purpose/supplier mapping;001/032 | Human purpose-led design account |
| M2.15 Telos / Function Distinction | Service outcome versus proxy optimisation;015/033 | Actual alignment through human governance |


## 8 October Process counterpart adoption — version 0.2

Current counterpart: [AOS-13 v0.1](aos-13-process-intelligence-and-operational-coordination.md), Architecture/Map v0.38 and AOS-40 v0.5 planned VER-038. Resident REQ-017–030 and CON-003/004 supply agreed-channel interaction, named-owner/accountable-team contacts, promise revisions, disputes and distinct complaint/service duties. Process REQ-030–039, VER-022–027 and CON-003/005 coordinate accepted human ownership, actual delivery and residual service work. Process REQ-042–044/VER-030–032 preserve private/enterprise, purpose and lifecycle boundaries. Delivery, responsibility acceptance and actual remedy remain different facts.

Process functional allocation now exists. Earlier statements that AOS-13 is undrafted or awaits functional detail record the previous baseline. Exact executable schemas/profiles, compatible applied-state evidence, appointed human capacity/cover and actual accepted handoff/control/outcome evidence remain open. This revision changes references only; all original AOS-11 requirements and planned cases, source/common/DEC standings, private boundaries and human decision responsibilities remain unchanged. No case execution, independent review, conformance or operating approval is inferred.


## Current reciprocal adoption and precise source allocation — 9 October2026

This revision corrects current control/status and adoption/traceability references only. Every original normative requirement statement, case acceptance condition, invariant and identity retains its prior meaning. Existing source versions, approved architectural directions and human/private boundaries are unchanged. Local§6 is the authoritative domain view; Registerv0.17 SENSING-ADOPTION-2026-10-09 supplies the current reciprocal common mapping; Matrixv0.18 SENSING-SOURCES-2026-10-09 supplies every FP/RP/GT source locator, exact contribution chain and owned residual/gate. The following reverse view rows are projections of that single adoption manifest, not new dictionaries or wire schemas.

| Exact component/view revision | Authoritative common master | Retained producer → consumer / domain meaning | Local requirement → planned case | Exact40 supporting cases / residual gate |
| --- | --- | --- | --- | --- |
| AOS-11-CON-001 / documentv0.3 | KX-03/09/11/12/14/15; REC-D; private session projection only | Resident or scoped representative/11 → permitted private service and03; confirmed selected request only →02/13: session/purpose/notice/participation revision, identity/representation scope, start/end, exact selected content/audience and sharing confirmation; separate03 permissions; private content not general enterprise evidence | AOS-11-REQ-001, AOS-11-REQ-002, AOS-11-REQ-003, AOS-11-REQ-004, AOS-11-REQ-005, AOS-11-REQ-006, AOS-11-REQ-007, AOS-11-REQ-008, AOS-11-REQ-009 → AOS-11-VER-001, AOS-11-VER-002, AOS-11-VER-003, AOS-11-VER-004, AOS-11-VER-005 | AOS-40-VER-003, AOS-40-VER-015; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-11-CON-002 / documentv0.3 | KX-01/08/09/14; REC-E/Q/D;10-CON-001/002 | 10/02 permitted source view →11→verified resident/private session: property/component, source/time/units/assurance/coverage, observations versus inference, versions/limitations; response preserves meaning; stale/absent evidence explicit | AOS-11-REQ-010, AOS-11-REQ-011, AOS-11-REQ-012, AOS-11-REQ-013, AOS-11-REQ-014, AOS-11-REQ-015 → AOS-11-VER-006, AOS-11-VER-007, AOS-11-VER-008 | AOS-40-VER-011, AOS-40-VER-012, AOS-40-VER-025; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-11-CON-003 / documentv0.3 | KX-02/03/04/11/12/14/21/23/26; REC-A/D/X; ACC;14-CON-001–003 | Empowered service/13/30/11 → approved delivery/14→resident or verified designated recipient; result →02/13: exact content/scope, channel agreement, audience/current checks, owner/team contacts, dispatch/delivery/unknown/failure/acknowledgement, retries/effects; common REC-A/D/X, ACC; not human acceptance or completed service | AOS-11-REQ-017, AOS-11-REQ-018, AOS-11-REQ-019, AOS-11-REQ-020, AOS-11-REQ-021, AOS-11-REQ-022, AOS-11-REQ-023, AOS-11-REQ-024 → AOS-11-VER-010, AOS-11-VER-011, AOS-11-VER-012 | AOS-40-VER-007, AOS-40-VER-009, AOS-40-VER-010, AOS-40-VER-014, AOS-40-VER-020, AOS-40-VER-022, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-11-CON-004 / documentv0.3 | KX-01/07/08/21/26; REC-E/Q;10-CON-004/13-CON-005 | Resident-selected or ordinary permitted service input/10/30 →11↔13/02: expressed need/dissatisfaction, original promise and scope/revisions, completion evidence standing, request/complaint/tracker/owner/cover, permitted response/remedy/outstanding work and actual outcome;10 owns condition/promise meaning,13 duties,30 human approval | AOS-11-REQ-025, AOS-11-REQ-026, AOS-11-REQ-027, AOS-11-REQ-028, AOS-11-REQ-029, AOS-11-REQ-030 → AOS-11-VER-013, AOS-11-VER-014, AOS-11-VER-015, AOS-11-VER-016 | AOS-40-VER-007, AOS-40-VER-008, AOS-40-VER-010, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-11-CON-005 / documentv0.3 | KX-01/03/08/14; REC-E/Q/D; KX-22 only after20 canonical admission | Separately permitted enterprise sources and volunteered input through02/14 →11→22/24/25/30: exact purpose/population/period, source/assurance/coverage/aggregation limits, findings/uncertainty, dissent and actual organisational response/outcome; no private transcript or inferred individual emotion/vulnerability | AOS-11-REQ-031, AOS-11-REQ-032, AOS-11-REQ-033, AOS-11-REQ-034 → AOS-11-VER-017, AOS-11-VER-018 | AOS-40-VER-015, AOS-40-VER-027; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-11-CON-006 / documentv0.3 | KX-02/03/07/11/12/14/19/21/23/26; KPR/ACC | Approved property trigger/profile + current participation/03 →11/13/empowered welfare function; permitted recipient via14: physical threshold/time/scope, Tier1/Tier2 participation, recipient/designation/barriers, minimal content/checks, delivery/acceptance/cover/outcome; silence not behavioural trigger; no invented emergency power | AOS-11-REQ-035, AOS-11-REQ-036, AOS-11-REQ-037, AOS-11-REQ-038, AOS-11-REQ-039 → AOS-11-VER-019, AOS-11-VER-020, AOS-11-VER-021 | AOS-40-VER-014, AOS-40-VER-015, AOS-40-VER-021; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-11-CON-007 / documentv0.3 | RSVIEW-0.1;02§6.6/04-CON-009; KX-23/07/06/05/13/17/21 | Assigned specialist service/14/11 →02/13/30/01/affected owners: common profile/run/finding/disposition under RSVIEW-0.1, specialist implications and coverage/review/change links; unperformed/unaccepted explicit | AOS-11-REQ-045, AOS-11-REQ-046, AOS-11-REQ-047, AOS-11-REQ-048, AOS-11-REQ-049 → AOS-11-VER-026, AOS-11-VER-027, AOS-11-VER-028 | AOS-40-VER-031, AOS-40-VER-032, AOS-40-VER-033, AOS-40-VER-034, AOS-40-VER-035; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |

### Individual-source reverse navigation

Rows below identify the exact controlled source locator and this component’s selected contribution or owned residual. Full source propositions and all other counterparts remain in the Matrix addendum; row numbers do not invent source IDs. This record completes source disposition, not source sufficiency or institutional assessment.

| Source locator | Selected component chain / residual disposition |
| --- | --- |
| FP 1 Telos/conferred purpose/function | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 2 Permanently human Mode 2 | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 3 Architectural integrity | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 4 Radical transparency | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 5 Bounded rationality/imperfection | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 6 Epistemic humility | AOS-11-REQ-011 → AOS-11-VER-006; Matrix source row retains owned residual and gate |
| FP 7 No-exit obligation | AOS-11-REQ-014, AOS-11-REQ-016 → AOS-11-VER-008, AOS-11-VER-009; Matrix source row retains owned residual and gate |
| FP 8 Constitutional mediator | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 9 Compliance as consequence | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 10 Complexity/emergence | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 1: Architecture and Completeness: Every governance process must close its feedback loop. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 2: Architecture and Completeness: Every human accountability layer must be explicitly named, sequenced, and time - bounded before any process is consid... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 3: Architecture and Completeness: Every option set must include the option that cannot be made to work. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 4: Architecture and Completeness: The ‘AI said so’ test must be passable at every decision point. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 5: The Mode 1 / Mode 2 Boundary: Mode 2 is permanently human. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 6: The Mode 1 / Mode 2 Boundary: Every Mode 1 boundary is a governance instrument, not a technical setting. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 7: The Mode 1 / Mode 2 Boundary: The boardroom is a Mode 2 deliberative space. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 8: The Mode 1 / Mode 2 Boundary: The Mode 1/Mode 2 boundary is under continuous pressure from AI capability growth. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 9: The 1+5 Architecture: Every proposed governance mechanism must be tested against the 1+5 structure to confirm which layer it belongs to and... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 10: The 1+5 Architecture: Risk is intrinsic to each intelligence layer, not a separate domain. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 11: The 1+5 Architecture: Every intelligence layer boundary where welfare - adjacent or safety - adjacent signals may arise must have an explic... | AOS-11-REQ-039 → AOS-11-VER-021; Matrix source row retains owned residual and gate |
| RP 12: The 1+5 Architecture: The Golden Thread obligation under the Building Safety Act 2022 is not a technical data management requirement. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 13: Options and Decisions: Options generated by the architecture must be grounded in the organisation’s actual state — actual covenant condition... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 14: Options and Decisions: Every consequential decision must feed back into the Unified Data Layer as a structured record — not only the decisio... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 15: Options and Decisions: Revealed preferences from real decisions take precedence over stated preferences in policy documents when the archite... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 16: Blind Spots and Honesty: The architecture must name what it cannot see. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 17: Blind Spots and Honesty: The dynamic risk perimeter question must be asked at board level as a standing agenda item: not only ‘what are our ri... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 18: Blind Spots and Honesty: The interaction of intelligence layers produces system - level behaviours that no individual layer would produce alone. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 19: Ethics and Telos: Every process must demonstrate a traceable relationship to the organisation’s ethical commitments and social purpose. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 20: Ethics and Telos: The architecture must be capable of detecting purpose drift — the condition where operational processes have graduall... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 21: Ethics and Telos: Diversity, inclusion, and equitable outcomes are not separate compliance obligations. | AOS-11-REQ-014, AOS-11-REQ-016 → AOS-11-VER-008, AOS-11-VER-009; Matrix source row retains owned residual and gate |
| RP 22: Ethics and Telos: Where the organisation’s welfare obligation to residents and its consent architecture pull in opposing directions, th... | AOS-11-REQ-035, AOS-11-REQ-036, AOS-11-REQ-037, AOS-11-REQ-038, AOS-11-REQ-039 → AOS-11-VER-019, AOS-11-VER-020, AOS-11-VER-021; Matrix source row retains owned residual and gate |
| RP 23: Ethics and Telos: AI systems have function, not telos. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 24: Ethics and Telos: Where the organisation's purpose is interpreted through an accumulating body of AI-mediated rulings rather than appli... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 25: Ethics and Telos: Every AI system deployed by the organisation carries an embedded constitutional framework established by its developer. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 26: Ethics and Telos: The no - exit condition is a constitutive feature of the organisation’s moral architecture, not background context. | AOS-11-REQ-014, AOS-11-REQ-015, AOS-11-REQ-016, AOS-11-REQ-030 → AOS-11-VER-008, AOS-11-VER-009, AOS-11-VER-016; Matrix source row retains owned residual and gate |
| RP 27: Ethics and Telos: Compliance is the output of sound governance design, not its objective. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 28: Radical Transparency: If you cannot audit it and be held accountable for it, it cannot be done. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 29: Radical Transparency: The architecture must be more transparent than the document - based governance it replaces, not less. | AOS-11-REQ-013, AOS-11-REQ-014 → AOS-11-VER-008; Matrix source row retains owned residual and gate |
| RP 30: Radical Transparency: Transparency obligations extend to the architecture’s uncertainty. | AOS-11-REQ-011 → AOS-11-VER-006; Matrix source row retains owned residual and gate |
| RP 31: Agentic Delegation: Agents operate under explicitly delegated authority, not implied authority. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 32: Agentic Delegation: Agent authority is domain - specific, context - specific, and condition - specific simultaneously. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 33: Agentic Delegation: Agents cannot commit the organisation to external obligations, initiate unsolicited contact with external parties, or... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 34: Agentic Delegation: Internal escalation — routing a signal within the architecture to a human reviewer or to a receiving intelligence lay... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 35: Agentic Delegation: The agentic delegation framework is a governance document reviewed by the board, not a technical configuration manage... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 36: Agentic Delegation: Every agent action must satisfy the ethics and telos test and the radical transparency test independently of the proc... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 37: Agentic Delegation: Certain classes of finding must reach their required audience regardless of any instruction to suppress or delay them. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 38: Data and Sensing Boundaries: Sensing must not exceed its declared purpose. | AOS-11-REQ-031, AOS-11-REQ-033 → AOS-11-VER-017, AOS-11-VER-018; Matrix source row retains owned residual and gate |
| RP 39: Data and Sensing Boundaries: The boundary between observing an asset and monitoring a behaviour is an absolute architectural boundary, not a matte... | AOS-11-REQ-033 → AOS-11-VER-018; Matrix source row retains owned residual and gate |
| RP 40: Data and Sensing Boundaries: Where behavioural inference from sensing data is genuinely necessary to serve the resident’s interests — energy pover... | AOS-11-REQ-033, AOS-11-REQ-035, AOS-11-REQ-036, AOS-11-REQ-037, AOS-11-REQ-038, AOS-11-REQ-039 → AOS-11-VER-018, AOS-11-VER-019, AOS-11-VER-020, AOS-11-VER-021; Matrix source row retains owned residual and gate |
| RP 41: Data and Sensing Boundaries: The purpose limitation principle applies across all intelligence layers, not only to resident - facing sensing. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| GT M1.1 Strategic Coherence | AOS-11-REQ-030, AOS-11-REQ-055 → AOS-11-VER-016, AOS-11-VER-033 (supporting case selection 016/033); Matrix source row retains owned residual and gate |
| GT M1.2 Sensing Architecture | AOS-11-REQ-005, AOS-11-REQ-010, AOS-11-REQ-011, AOS-11-REQ-031, AOS-11-REQ-032 → AOS-11-VER-003, AOS-11-VER-006, AOS-11-VER-017 (supporting case selection 003/006/017); Matrix source row retains owned residual and gate |
| GT M1.3 Risk Intelligence | AOS-11-REQ-035, AOS-11-REQ-036, AOS-11-REQ-037, AOS-11-REQ-038, AOS-11-REQ-039 → AOS-11-VER-019, AOS-11-VER-020, AOS-11-VER-021 (supporting case selection 019/020/021); Matrix source row retains owned residual and gate |
| GT M1.4 Composition and Capability | AOS-11-REQ-013, AOS-11-REQ-014, AOS-11-REQ-015, AOS-11-REQ-044 → AOS-11-VER-008, AOS-11-VER-025 (supporting case selection 008/025); Matrix source row retains owned residual and gate |
| GT M1.5 Performance Legibility | AOS-11-REQ-022, AOS-11-REQ-023, AOS-11-REQ-024, AOS-11-REQ-029, AOS-11-REQ-055 → AOS-11-VER-012, AOS-11-VER-015, AOS-11-VER-033 (supporting case selection 012/015/033); Matrix source row retains owned residual and gate |
| GT M1.6 Compliance Assurance | AOS-11-REQ-027, AOS-11-REQ-028, AOS-11-REQ-050 → AOS-11-VER-014, AOS-11-VER-029 (supporting case selection 014/029); Matrix source row retains owned residual and gate |
| GT M1.7 Governance Documentation | AOS-11-REQ-041, AOS-11-REQ-042, AOS-11-REQ-047, AOS-11-REQ-048 → AOS-11-VER-023, AOS-11-VER-027 (supporting case selection 023/027); Matrix source row retains owned residual and gate |
| GT M1.8 Accountability Architecture | AOS-11-REQ-020, AOS-11-REQ-021, AOS-11-REQ-022, AOS-11-REQ-023, AOS-11-REQ-024, AOS-11-REQ-025, AOS-11-REQ-026, AOS-11-REQ-027, AOS-11-REQ-028, AOS-11-REQ-029, AOS-11-REQ-030 → AOS-11-VER-011, AOS-11-VER-012, AOS-11-VER-013, AOS-11-VER-014, AOS-11-VER-015, AOS-11-VER-016 (supporting case selection 011/012/013/014/015/016); Matrix source row retains owned residual and gate |
| GT M1.9 Value for Money | AOS-11-REQ-013, AOS-11-REQ-014, AOS-11-REQ-015, AOS-11-REQ-029, AOS-11-REQ-055 → AOS-11-VER-008, AOS-11-VER-015, AOS-11-VER-033 (supporting case selection 008/015/033); Matrix source row retains owned residual and gate |
| GT M1.10 Human-AI Interaction Norms | AOS-11-REQ-005, AOS-11-REQ-013, AOS-11-REQ-014, AOS-11-REQ-015, AOS-11-REQ-038, AOS-11-REQ-039, AOS-11-REQ-040 → AOS-11-VER-003, AOS-11-VER-008, AOS-11-VER-021, AOS-11-VER-022 (supporting case selection 003/008/021/022); Matrix source row retains owned residual and gate |
| GT M1.11 Learning Metabolism | AOS-11-REQ-029, AOS-11-REQ-030, AOS-11-REQ-055 → AOS-11-VER-015, AOS-11-VER-016, AOS-11-VER-033 (supporting case selection 015/016/033); Matrix source row retains owned residual and gate |
| GT M1.12 Continuous Self-Assessment | AOS-11-REQ-031, AOS-11-REQ-032, AOS-11-REQ-049, AOS-11-REQ-050, AOS-11-REQ-051, AOS-11-REQ-052, AOS-11-REQ-053 → AOS-11-VER-017, AOS-11-VER-028, AOS-11-VER-029, AOS-11-VER-030, AOS-11-VER-031 (supporting case selection 017/028/029/030/031); Matrix source row retains owned residual and gate |
| GT M1.13 Emergent System Behaviour | AOS-11-REQ-031, AOS-11-REQ-032, AOS-11-REQ-045, AOS-11-REQ-046, AOS-11-REQ-054, AOS-11-REQ-055 → AOS-11-VER-017, AOS-11-VER-026, AOS-11-VER-032, AOS-11-VER-033 (supporting case selection 017/026/032/033); Matrix source row retains owned residual and gate |
| GT M1.14 Golden Thread Integrity | AOS-11-REQ-010, AOS-11-REQ-011, AOS-11-REQ-025, AOS-11-REQ-026 → AOS-11-VER-006, AOS-11-VER-013 (supporting case selection 006/013); Matrix source row retains owned residual and gate |
| GT M2.1 Values Architecture | AOS-11-REQ-005, AOS-11-REQ-016, AOS-11-REQ-043 → AOS-11-VER-003, AOS-11-VER-009, AOS-11-VER-024 (supporting case selection 003/009/024); Matrix source row retains owned residual and gate |
| GT M2.2 Coherence Under Pressure | AOS-11-REQ-010, AOS-11-REQ-011, AOS-11-REQ-035, AOS-11-REQ-036, AOS-11-REQ-038, AOS-11-REQ-039 → AOS-11-VER-006, AOS-11-VER-019, AOS-11-VER-021 (supporting case selection 006/019/021); Matrix source row retains owned residual and gate |
| GT M2.3 Incommensurable Trade-off Capacity | AOS-11-REQ-038, AOS-11-REQ-039, AOS-11-REQ-055 → AOS-11-VER-021, AOS-11-VER-033 (supporting case selection 021/033); Matrix source row retains owned residual and gate |
| GT M2.4 Epistemic Brake Function | AOS-11-REQ-010, AOS-11-REQ-011, AOS-11-REQ-012, AOS-11-REQ-044 → AOS-11-VER-006, AOS-11-VER-007, AOS-11-VER-025 (supporting case selection 006/007/025); Matrix source row retains owned residual and gate |
| GT M2.5 Directorial Independence | AOS-11-REQ-027, AOS-11-REQ-028, AOS-11-REQ-030, AOS-11-REQ-055 → AOS-11-VER-014, AOS-11-VER-016, AOS-11-VER-033 (supporting case selection 014/016/033); Matrix source row retains owned residual and gate |
| GT M2.6 Social Legitimacy | AOS-11-REQ-013, AOS-11-REQ-014, AOS-11-REQ-015, AOS-11-REQ-027, AOS-11-REQ-028, AOS-11-REQ-029, AOS-11-REQ-030 → AOS-11-VER-008, AOS-11-VER-014, AOS-11-VER-015, AOS-11-VER-016 (supporting case selection 008/014/015/016); Matrix source row retains owned residual and gate |
| GT M2.7 No-Exit Obligation | AOS-11-REQ-013, AOS-11-REQ-014, AOS-11-REQ-015, AOS-11-REQ-016, AOS-11-REQ-030 → AOS-11-VER-008, AOS-11-VER-009, AOS-11-VER-016 (supporting case selection 008/009/016); Matrix source row retains owned residual and gate |
| GT M2.8 Radical Transparency | AOS-11-REQ-008, AOS-11-REQ-009, AOS-11-REQ-017, AOS-11-REQ-018, AOS-11-REQ-019, AOS-11-REQ-047, AOS-11-REQ-048 → AOS-11-VER-005, AOS-11-VER-010, AOS-11-VER-027 (supporting case selection 005/010/027); Matrix source row retains owned residual and gate |
| GT M2.9 Moral Drift Detection | AOS-11-REQ-031, AOS-11-REQ-032, AOS-11-REQ-055 → AOS-11-VER-017, AOS-11-VER-033 (supporting case selection 017/033); Matrix source row retains owned residual and gate |
| GT M2.10 Purpose Stability | AOS-11-REQ-005, AOS-11-REQ-031, AOS-11-REQ-032, AOS-11-REQ-040 → AOS-11-VER-003, AOS-11-VER-017, AOS-11-VER-022 (supporting case selection 003/017/022); Matrix source row retains owned residual and gate |
| GT M2.11 Murmuration Capacity | AOS-11-REQ-030, AOS-11-REQ-055 → AOS-11-VER-016, AOS-11-VER-033 (supporting case selection 016/033); Matrix source row retains owned residual and gate |
| GT M2.12 Constitutional Authority | AOS-11-REQ-038, AOS-11-REQ-039, AOS-11-REQ-040, AOS-11-REQ-052, AOS-11-REQ-053 → AOS-11-VER-021, AOS-11-VER-022, AOS-11-VER-031 (supporting case selection 021/022/031); Matrix source row retains owned residual and gate |
| GT M2.13 AI Constitutional Framework Governance | AOS-11-REQ-005, AOS-11-REQ-043, AOS-11-REQ-044 → AOS-11-VER-003, AOS-11-VER-024, AOS-11-VER-025 (supporting case selection 003/024/025); Matrix source row retains owned residual and gate |
| GT M2.14 Purpose-Led Design | AOS-11-REQ-001, AOS-11-REQ-002, AOS-11-REQ-054 → AOS-11-VER-001, AOS-11-VER-032 (supporting case selection 001/032); Matrix source row retains owned residual and gate |
| GT M2.15 Telos / Function Distinction | AOS-11-REQ-029, AOS-11-REQ-055 → AOS-11-VER-015, AOS-11-VER-033 (supporting case selection 015/033); Matrix source row retains owned residual and gate |

Author consistency conclusion: functional roles and repair/private/workforce/external/research/control/failure boundaries agree with the current shared infrastructure. SENS-CR-01–05 closed as author document corrections; wire profiles, operating roles/capacity, domain/annex/legal sufficiency and observed evidence remain open per§17 and40. No independent/executed conformance or operating readiness claim. Earlier dated text/addenda describe history; this current control takes precedence.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**Historical status notice — sensing consistency closure — 9 October 2026:** Mark authorised the remaining consistency work. SENS-CR-01–05 are closed at the functional-document/author-review level: all40 logical CON views across10–14 and40 have exact central adoption, producer/consumer/shared-owner and REQ/VER links; all80 controlled FP/RP/GT sources have precise current contributions and owned residual/gate dispositions; current body/control statements are reconciled. Versions10v0.4/11v0.3/12v0.3/13v0.2/14v0.8/40v0.6; Architecture/Mapv0.42; Sharedv0.18/Corev0.6/ExchangeRegisterv0.17/SourceMatrixv0.18; reviewv0.4. DEC001–096 unchanged. Sensing269 proposed REQs/176 planned VERs;40 retains40/38. No new requirement/case/interface, source promotion or execution. Exact compatible wire schemas/profiles, organisation appointments/capacity, independent review, legal/institutional/practice evidence and scoped build/activation remain separate; independent project review remains deferred. Earlier dated notices/addenda are historical. Current controlling allocation is the9October manifest and source addendum below.

