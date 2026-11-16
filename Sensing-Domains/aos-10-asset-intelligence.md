# AOS-10 — Asset Intelligence

Document: aos-10-asset-intelligence · Source revision or record: v0.5 functional baseline, editorial edition 29 October 2026

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

| Document control | Value |
| --- | --- |
| Identifier / version / date | AOS-10 / 0.5 / 9 October 2026 |
| Status | Functional specification review draft; proposed requirements; verification planned, not executed |
| Architecture baseline | AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3. |
| Current component baseline | AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3. |
| Common baseline | AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3. |
| Governing source / quality baseline | Preserved source manifest; FP v4; RP v6; Governance Intelligence Tests; AOS-QS v0.1; component template v0.4 |
| Project owner / specification custodian | Mark Sweeny |
| Accountable operating owner | Asset service owner; organisational appointment pending; competent inspection/building-safety and statutory dutyholders are separate roles |
| Author / reviewers | Codex at Mark's request; author structural and consistency checks; Mark functional review pending; independent project review deferred |
| Approval / readiness | Existing approved directions guide drafting; exact requirements proposed; no whole-document approval, G3/G4, operating activation or conformance claimed |
| Release scope | Asset functional architecture; repair demonstration allocation; exact executable release/profile scope not yet authorised |
| Change history | 0.3 — reciprocal AOS-13 v0.1 references and current architecture baseline only; original REQ/VER text, IDs and status retained.  0.2 supplier participation redraft at Mark's request, 8 October 2026; REQ-049 / VER-034 added; original IDs retained; 0.1 initial functional draft; no new constitutional decision, approved IF family, technology selection or numerical default |

## 1. Purpose and scope

Asset Intelligence provides an evidence-grounded account of the physical homes, buildings and components for which the organisation has responsibilities. It makes condition, missing knowledge, developing physical risks and the effects of maintenance legible to service teams and governance. Without it the organisation cannot distinguish a known physical condition from an incomplete record, inferential forecast or administrative work status.

Its intended outcome is a Living Asset Register that links attributable observation to interpreted condition, proposed intervention, human-authorised action and actual outcome. A safe or completed label must have the evidence required for that exact claim. Missing telemetry must remain visible while inspection, resident reporting and manual service continue through permitted routes.

Scope covers property/component identities and relationships; physical inspections, reports and telemetry; coverage/freshness; uncertain condition and maintenance analysis; physical-risk referrals; repair promise/completion evidence; investment-planning inputs; governed building-safety information; actual consequence feedback; and its own external adaptation research. Continuous sensing is an optional implementation capability, not a universal requirement to install sensors in every home.

AOS-10 is one of five sensing domains. It does not own resident profiling/contact delivery (11), staff matters (12), work orchestration/overdue detection and duty tracking (13), external retrieval/exchange (14), cross-domain synthesis (22) or human decisions (30). It cannot replace competent physical assessment, determine statutory liability, automatically allocate capital or treat physical signals as implicit permission to infer residents' conduct. Digital-twin modelling is optional; a 3D model is not necessary to satisfy this functional specification.

## 2. Authority and sources

FP v4 and RP v6 govern; approved architecture decisions constrain interpretation. Books explain intent. Requirements below are proposed engineering obligations, not new approved decisions. External sources provide dated research evidence and require competent applicability mapping; a guidance page is not itself an organisational authority grant.

| Source key | Exact source / derivation and use |
| --- | --- |
| ARCH | AOS-00 v0.33 §§3.1/4.2/6/9, REQ-041–044 and VER-019; Specification Map §4 AOS-10; v0.34 adds this allocation only |
| FP / RP / GT | FP v4 principles 1–10; RP v6 domains 1–9, especially domain 3 Golden Thread and 9 Sensing; all 29 GT tests allocated in Appendix A |
| B4 | Book 4, Asset Intelligence chapter: physical condition, Living Asset Register, telemetry/manual evidence, early warning, investment and building safety; explanatory, not current legal/product authority |
| QS | AOS-QS v0.1, QS-04–28; component template v0.4 including required §4.4 |
| DATA | AOS-02 v0.8 §§5/6/10; Core v0.6 REC-E/Q/A/D/X; Shared v0.15; Register v0.14; DEC-045–048 |
| CONTROL | AOS-01/03/04/05 v0.8; Control Coordination v0.2; Protected Reporting and Recovery v0.1; DEC-028–030/042–044/049–061/067–078 |
| REPAIR | DEC-036–041; Operational Profiles v0.1 §§4/5; 30 v0.5 repair duties; 40 v0.2 VER-007–010 |
| RESEARCH | DEC-086; 04 CON-009; 02 CON-007 / RSVIEW-0.1; 01 §10.8; 14 retrieval; 13 coordination; 30 human disposition |
| GI | 20–25 current versions above; source-assured inputs, canonical analysis, presentation and oversight; DEC-088–091 |

### 2.1 External research used in this draft

Access/verification date: 8 October 2026. Brief summaries record the architectural implication only; full source text and legal mapping remain separate. No numeric statutory deadline, blanket compliance claim or vendor commitment is imported.

| Key | Primary source / status / bounded implication |
| --- | --- |
| EXT-01 | [Regulator of Social Housing: Safety and Quality Standard](https://www.gov.uk/government/publications/safety-and-quality-standard), England, published standard; §2.1.1 individual-property physical assessment and §2.3 repair communication support attributable physical evidence and clear repair records. Operational applicability/assurance requires competent human mapping. |
| EXT-02 | [Building Safety Regulator: keeping higher-risk building information — golden thread](https://www.gov.uk/guidance/keeping-information-about-a-higher-risk-building-the-golden-thread), guidance, stage/dutyholder-specific; informs current, secure, usable information and evidenced handover. A generic asset register cannot establish fulfilment of every statutory information duty. |
| EXT-03 | [Awaab's Law guidance for social landlords](https://www.gov.uk/government/publications/awaabs-law-guidance-for-social-landlords), England, current Phase 1 guidance collection, accessed 8 October; relevant hazard awareness, investigation and work evidence must be distinguishable from resident-promised dates. Actual regulations and applicability control legal conclusions. |
| EXT-04 | [Awaab's Law Phase 2 guidance](https://www.gov.uk/government/publications/awaabs-law-phase-2-guidance-for-social-housing-landlords/awaabs-law-phase-2-guidance-for-social-landlords), non-statutory guidance; expanded requirements take effect 30 November 2026, future at this draft date. Research must preserve effective-date standing rather than activate future rules early. |
| EXT-05 | [MHCLG: delivering a data standard to support Awaab's Law](https://mhclgdigital.blog.gov.uk/2025/08/20/delivering-a-data-standard-to-support-awaabs-law-in-social-housing/), government development account, 20 August 2025; property/investigation/work-order/appointment relationships are mapping candidates. DEC-048 retains HACT as preferred reference for assessment; exact released version, licence, mappings and conformance remain unapproved. Direct HACT page retrieval was unavailable; this is not evidence of latest HACT definitions. |

England-specific sources are not silently generalised across jurisdictions or tenures. The source manifest remains unchanged. Book forecasts, supplier examples and market claims do not become guarantees of predictive accuracy, legal compliance or investment return.

## 3. Responsibilities and context

| Responsibility | AOS-10 contribution / authoritative counterpart |
| --- | --- |
| Physical evidence and condition | Asset owner/competent inspectors steward domain meaning; 02 owns shared record semantics; 14 owns supplier/external intake; 03 controls permitted use |
| Coverage and risk | 10 exposes observed/unobserved physical scope and bounded risks; 13 routes duty; 30 supports empowered human response; 22 synthesises across domains |
| Repairs | 10 supplies promise/completion/condition evidence; 13 compares dates and orchestrates accepted duties; 11 governs resident participation/agreed channels and delivery; 30 records authorised human decisions |
| Investment | 10 supplies condition/scenario inputs; 22 prepares alternatives; 30 supports human approval; expenditure authority comes from 01 and the organisation's approved instruments |
| Building-safety information | 10 supports evidence custody and gap reporting with 02/03/14; statutory dutyholders retain legal duties; board governance accountability is separate |
| Research | Assigned agent/shared service researches this specialist remit through 14; 10 owns relevance; 13 tracks handoff; 30/01 retain disposition/amendment powers |

Trust boundaries include resident/home to device or inspector, supplier to admitted evidence, raw evidence to probabilistic interpretation, component to shared controls, internal to external disclosure, and software support to human judgement. Housing-management/asset systems, contractor feeds and sensors are candidate sources; none is authoritative for every fact merely by being connected.

### 3.1 Supplier participation and functional realisation

**AOS responsibilities are logical functions, not mandatory separate products.** Existing supplier sensors, connectivity, cloud services, analytics, case management, portals and apps can implement relevant parts of the architecture. A supplier can provide observations only, observations plus interpreted findings, or a combined service that realises several component functions. The organisation need not duplicate capable supplier software merely to give every AOS component its own application.

The integration question is: which exact obligations does each supplier service fulfil, what evidence and governed records does it provide, where are controls enforced, and what remains with other systems or humans? A supplier's risk interpretation can be admitted as an attributed analytical finding with method/version/limitations; AOS does not require it to be re-created internally. Where evidence cannot be exported, an accessible controlled reference and permitted review path must still support the declared obligation; an inaccessible dashboard label cannot alone prove conformance.

| Supplier offering | Candidate AOS function / view | Evidence and boundary to demonstrate |
| --- | --- | --- |
| Environmental/asset sensors and device status | 10 FUN-001/002; CON-001/002 | Physical quantity/unit, device/property/component identity, observed time, provenance, quality and lost coverage; no implicit resident behaviour inference |
| Gateway, cloud collection and connectors | 14 intake/exchange; 02 admission; 05 runtime/security | Authenticated source, delivery/ordering/duplicate semantics, integrity, outage visibility and governed purpose/access |
| Supplier condition/risk analytics | 10 FUN-003; CON-002/003 | Observation versus derived finding, supporting evidence, exact analytical version, uncertainty, evaluated scope and referral meaning |
| Asset portal/register/reporting | 10 FUN-002; CON-002/005; relevant GI rendering interfaces | Coverage/currentness/lineage and permitted readable views; no complete safety or institution-wide governance claim from dashboard colour |
| Maintenance/case-management platform | 13 workflow plus 10 CON-003/004 and 30 human decision support | Accepted owner, original promise, work scope, actual completion evidence, exceptions, duplicate/retry reconciliation and human approvals |
| Resident application/communications | 11 participation/delivery with 10 evidence and 13 tracking | Agreed channels, accessible alternatives, purpose/use checks, challenge/correction and distinct delivery/acceptance/service outcomes |
| Building-information repository | 10 FUN-006; CON-006; 02/03/14 custody/access/transfer | Current category inventory, exact versions/gaps, dutyholder scope, secure access and separate usable handover confirmation |

Participation arrangements may include a standalone operational portal with governed manual/reference exchange, API/event integration with existing systems, or a combined supplier platform spanning functions. Each is assessed against its declared scope: a manual exchange does not meet an automated-service claim, and an API's existence does not prove its fields, permissions or reliability satisfy the AOS contracts. The same named source of truth and authority rules apply whichever arrangement is used. Avoid competing case masters: declare the authoritative record for each meaning and the correction/reconciliation route.

Suppliers may meet some obligations directly, others through configuration or integration, and leave some outside their scope. Compliance is evaluated per exact requirement and assembled release, not awarded to an entire product from broad capability resemblance. The organisation and humans retain their accountable and reserved duties regardless of hosting or supplier branding. §18 provides an illustrative mapping; §20 provides the response matrix.

## 4. Capabilities and functions

### 4.1 Capabilities

| CAP | Outcome / requirement range |
| --- | --- |
| AOS-10-CAP-001 | Attributable physical asset evidence and Living Asset Register; REQ-001–010/048 |
| AOS-10-CAP-002 | Bounded early warning and accepted physical-risk/service handoff; 011–012/020–022 |
| AOS-10-CAP-003 | Resident-promise and actual repair evidence; 013–019/032 |
| AOS-10-CAP-004 | Investment and governance inputs with uncertainty and human judgement preserved; 023/044 |
| AOS-10-CAP-005 | Governed building-safety information and usable transfer; 024–027/047 |
| AOS-10-CAP-006 | Permitted, secure, correctable and recoverable operation; 028–038/045–046 |
| AOS-10-CAP-007 | Specialist external research and human-governed adaptation; 039–043 |
| AOS-10-CAP-008 | Attributable supplier participation and implementation coverage; 049 |

### 4.2 Functions

| FUN | Trigger → inputs → behaviour/output / authority and failure |
| --- | --- |
| AOS-10-FUN-001 Admit observation | Permitted source event → scope/provenance/use checks → admitted evidence or explicit rejection/quarantine; never convert unknown identity into certainty; CAP-001/006, CON-001 |
| AOS-10-FUN-002 Maintain register | Evidence/correction/freshness change → source-assured observations and coverage → versioned condition view; conflicts/gaps preserved; CAP-001, CON-002 |
| AOS-10-FUN-003 Analyse and refer | Approved analytical trigger → bounded evidence/rule → inference, forecast or physical-risk referral; uncertainty and human route explicit; CAP-002/004, CON-003/005 |
| AOS-10-FUN-004 Supply repair evidence | Repair/promise/work evidence change → original promise and completion rule → controlled classifications supplied to Process; unknown/partial/disputed paths distinct; CAP-003, CON-004 |
| AOS-10-FUN-005 Prepare scenarios | Authorised planning request → condition/resource/assumption inputs → non-binding alternatives and distributional consequences; no capital commitment; CAP-004, CON-005 |
| AOS-10-FUN-006 Steward building information | Applicable profile/update/handover → exact inventory/currentness/use → governed view/transfer evidence and owned gaps; legal dutyholder remains human; CAP-005, CON-006 |
| AOS-10-FUN-007 Correct and recover | Changed evidence/use, outage or restoration → impact/current restrictions/prior effects → selective reassessment and approved fallback/continuation; no blind retry; CAP-006, CON-001–006 |
| AOS-10-FUN-008 Research adaptation | Approved profile trigger → permitted external sources → common run/finding/reviewer/disposition records; gaps and urgency visible; change/activation separate; CAP-007, CON-007 |
| AOS-10-FUN-009 Assess supplier realisation | Proposed supplier/configuration change → exact capability/requirement/contract declaration → scoped fit, evidence and owned gap assessment; no selection or activation by mapping alone; CAP-008, existing CON-001–007 and common manifest |

### 4.3 Requirements and record metadata

Each row below is one proposed component-level obligation. Category and source are explicit. Rationale is the corresponding function's prevention of false knowledge, unowned duty or unauthorised effect. Owner is the asset service owner, with domain-specific competent stewards in §3; approver is Mark for specification disposition and the empowered organisational authority for its commissioned application. All rows have status **proposed**, scope **functional draft**, history **0.1 initial allocation, 8 October 2026; REQ-049 added at 0.2 under Mark's supplier-participation direction**. Dependencies are the cited component/contracts plus §§6/16/17; linked CAP/FUN follow the ranges above and each VER's CON allocation. Exact source locators use this document's §2 register. No open setup value becomes a build default.

| Requirement | Independently verifiable obligation | Source / derivation | Planned VER |
| --- | --- | --- | --- |
| AOS-10-REQ-001 | **Scope:** For every asset observation or analysis, AOS-10 shall identify the physical asset purpose and applicable organisation, property/building/component and observation scope. | ARCH §3.1; RP9 | AOS-10-VER-001 |
| AOS-10-REQ-002 | **Identity:** AOS-10 shall admit asset relationships only with governed identity, effective dates and explicit unresolved reconciliation status. | 02 §§5/6/10; DEC-045 | AOS-10-VER-001 |
| AOS-10-REQ-003 | **Evidence:** AOS-10 shall preserve each observation's source, method, observed time, admission time, units, assurance, uncertainty and correction lineage through the governed evidence contract. | 02 CON-001; Core REC-E; DEC-046 | AOS-10-VER-002 |
| AOS-10-REQ-004 | **Coverage:** Each condition view shall expose its covered property/component/hazard/time scope and material missing, inaccessible, stale, failed or unperformed observations. | B4 Asset; RP5/7/9 | AOS-10-VER-003 |
| AOS-10-REQ-005 | **Register:** The Living Asset Register shall distinguish physical observation, interpreted condition, forecast, human decision, action and verified outcome as separate linked meanings. | B4 Asset; RP1/7; 02 REC-E/Q | AOS-10-VER-004 |
| AOS-10-REQ-006 | **Condition:** AOS-10 shall retain unresolved contradictory condition evidence rather than silently replacing it with the newest arrival or an aggregate score. | 02 §10; DEC-046; FP5/6 | AOS-10-VER-005 |
| AOS-10-REQ-007 | **Manual assessment:** AOS-10 shall support identifiable physical inspection and resident-reported condition evidence when sensors are absent or unavailable. | EXT-01; B4 Asset; RP9 | AOS-10-VER-006 |
| AOS-10-REQ-008 | **No substitution:** AOS-10 shall not represent telemetry or model interpretation as a completed physical assessment without evidence of that assessment. | EXT-01; FP3/4/6 | AOS-10-VER-006 |
| AOS-10-REQ-009 | **Analysis:** Every condition inference shall identify supporting evidence, applicable analytical version, assumptions and limitations separately from observed facts. | 04 §§4/13; RP7 | AOS-10-VER-007 |
| AOS-10-REQ-010 | **Prediction:** Each maintenance forecast shall expose its scenario, horizon, uncertainty, evaluation basis and conditions under which it cannot support a conclusion. | B4 Asset; FP5/6; QS-18 | AOS-10-VER-007 |
| AOS-10-REQ-011 | **Urgent concerns:** AOS-10 shall refer a suspected acute physical safety concern through the separately approved human safety protocol without waiting for ordinary analytical or governance review. | DEC-051; RP3; 30 §10 | AOS-10-VER-008 |
| AOS-10-REQ-012 | **Action boundary:** Before any consequential asset action, AOS-10 shall obtain current authority and permitted-use checks for that exact proposed operation. | 01/03/04; DEC-028–030/042–044; COORD CHECK/ACT | AOS-10-VER-009 |
| AOS-10-REQ-013 | **Promise source:** AOS-10 shall supply the resident-communicated repair completion commitment and its provenance separately from internal scheduling targets. | DEC-036/037; ARCH REQ-041–044; Profiles §§4/5 | AOS-10-VER-010 |
| AOS-10-REQ-014 | **Comparison meaning:** AOS-10 shall supply the promised-date precision and approved calendar/timezone comparison meaning without introducing a grace period. | DEC-036 | AOS-10-VER-011 |
| AOS-10-REQ-015 | **Promise revision:** AOS-10 shall recognise a revised resident commitment only with authorised human revision and evidence of communication, preserving the original commitment and breach history. | DEC-037 | AOS-10-VER-012 |
| AOS-10-REQ-016 | **Completion:** AOS-10 shall label repair completion established only when the repair-specific completion rule is satisfied by an identifiable completion record and required work or inspection evidence. | DEC-038; Profiles §§4/5 | AOS-10-VER-013 |
| AOS-10-REQ-017 | **Unknown completion:** Where completion cannot be established after the promised boundary, AOS-10 shall supply “completion unverified after promised date” for an owned verification escalation. | DEC-039 | AOS-10-VER-014 |
| AOS-10-REQ-018 | **Incomplete scope:** Where part of the promised scope remains outstanding, AOS-10 shall preserve the original repair as incomplete and identify completed and outstanding work separately. | DEC-040 | AOS-10-VER-015 |
| AOS-10-REQ-019 | **Dispute:** AOS-10 shall preserve contested completion as disputed evidence for human resolution rather than treating resident silence or a contractor status as resolution. | DEC-038; FP7; 30 REQ-021–033 | AOS-10-VER-016 |
| AOS-10-REQ-020 | **Workflow handoff:** AOS-10 shall transfer condition or repair findings with evidence and explicit uncertainty to AOS-13's governed lifecycle without treating receipt as acceptance of responsibility. | RP1/3/8; 13 boundary; COORD ACC | AOS-10-VER-017 |
| AOS-10-REQ-021 | **Outcome:** AOS-10 shall link actual work and inspection outcomes to originating evidence and decisions, retaining the distinction between an action attempted and condition improved. | RP1/4; Core REC-X/E/Q | AOS-10-VER-018 |
| AOS-10-REQ-022 | **Risk inputs:** Each asset-risk contribution shall identify physical concern, potential consequences, exposure scope, evidence limits and accountable human route. | RP3/5; B4 Asset; general architectural risk inputs (CAP-02 use-case assessment deferred) | AOS-10-VER-008 |
| AOS-10-REQ-023 | **Investment:** Each investment-planning input shall expose condition evidence, assumptions, resource constraints, alternative scenarios and uncertain consequences without claiming a human capital-allocation decision. | B4 Asset; FP1/2; 22 §§4/10 | AOS-10-VER-019 |
| AOS-10-REQ-024 | **Golden Thread scope:** Each building-safety information view shall identify the building, applicable lifecycle/dutyholder scope, required information categories and unresolved applicability gaps under a competent human-approved profile. | EXT-02; RP3 Golden Thread; ARCH §4.2 | AOS-10-VER-020 |
| AOS-10-REQ-025 | **Golden Thread custody:** AOS-10 shall preserve identifiable current versions and revision history of governed building-safety information with authorised secure access and disclosed completeness gaps. | EXT-02; 02/03; FP4 | AOS-10-VER-021 |
| AOS-10-REQ-026 | **Golden Thread transfer:** An authorised building-safety transfer shall record exact information versions, recipient scope, delivery and separate confirmation that information is usable, with failed or unconfirmed transfers left owned. | EXT-02; 14 §10; COORD ACC | AOS-10-VER-022 |
| AOS-10-REQ-027 | **Regulatory applicability:** AOS-10 shall distinguish the source's publication and effective dates, jurisdiction and legal standing from the organisation's approved operational rule and actual evidence of compliance. | EXT-01–04; DEC-086; FP9 | AOS-10-VER-023 |
| AOS-10-REQ-028 | **Data minimisation:** AOS-10 shall use and disclose asset evidence only for the checked purpose, audience and permitted data/inference scope under AOS-03. | 03 §§7/9; RP9; DEC-049–053 | AOS-10-VER-024 |
| AOS-10-REQ-029 | **Behaviour prohibition:** AOS-10 shall not infer individual occupancy, habits, emotions, personal conduct or preferences from physical asset signals as part of Asset Intelligence; any separately proposed person-related purpose requires its own governed component scope and approval. | RP9; DEC-088; 03 boundary | AOS-10-VER-024 |
| AOS-10-REQ-030 | **Optional sensing:** AOS-10 shall preserve core-service access and a permitted manual evidence route when a resident declines optional sensing or optional data use. | DEC-052; FP7; RP6/9 | AOS-10-VER-025 |
| AOS-10-REQ-031 | **Correction:** When evidence or permitted use changes, AOS-10 shall identify affected dependent views and pending work for selective reassessment without erasing original evidence standing. | DEC-047/089; COORD CHG; 02 §10 | AOS-10-VER-026 |
| AOS-10-REQ-032 | **Resident challenge:** AOS-10 shall provide permitted condition/repair evidence and a tracked correction or challenge referral through AOS-11/13 rather than equating silence or message delivery with acceptance. | DEC-041; FP7; 11/13/30 boundaries | AOS-10-VER-016 |
| AOS-10-REQ-033 | **Security:** AOS-10 shall admit telemetry only through approved source identity, integrity and runtime controls, quarantining unauthenticated, malicious or semantically invalid data. | 05/14; 02 admission; RP9 | AOS-10-VER-027 |
| AOS-10-REQ-034 | **Quality:** AOS-10 shall evaluate probabilistic asset analysis against a human-approved task/population/error rubric before a dependent performance claim. | QS-18; 04 §13; FP5/6 | AOS-10-VER-028 |
| AOS-10-REQ-035 | **Degraded operation:** When asset evidence or a dependency fails, AOS-10 shall disclose the affected coverage and support the approved manual/human fallback without inventing safe condition or closure. | B4 Asset; 05/COORD/KPR; FP5 | AOS-10-VER-029 |
| AOS-10-REQ-036 | **Recovery:** Recovered asset processing shall reconcile current authority, data-use restrictions and previously attempted effects before repeating a consequential operation. | DEC-028–030; KPR §§4–6; 05 §10 | AOS-10-VER-029 |
| AOS-10-REQ-037 | **Audit:** AOS-10 shall retain permitted evidence sufficient to reconstruct a consequential finding's trigger, inputs, actor, applied rule, authority, action, human intervention and observed outcome. | RP7; QS-19; 02 REC-E/Q/A/D/X | AOS-10-VER-018 |
| AOS-10-REQ-038 | **Common contracts:** AOS-10 producers and consumers shall declare exact common contract/view revisions and reject unsupported or ambiguous semantics rather than silently coercing them. | 02; Shared v0.15; Register v0.14; QS-12 | AOS-10-VER-030 |
| AOS-10-REQ-039 | **Research profile:** AOS-10 shall perform external adaptation research only within an approved component-owned profile using the common research meanings and permitted retrieval route. | DEC-086; 04 CON-009; 02 CON-007 | AOS-10-VER-031 |
| AOS-10-REQ-040 | **Research findings:** Every asset research finding shall separate verified source content, component interpretation, affected specification elements and proposed operational or amendment implications. | DEC-086; RSVIEW-0.1; 14 §10 | AOS-10-VER-031 |
| AOS-10-REQ-041 | **Research coverage:** Each asset research run shall disclose complete, partial, failed or unperformed coverage and limit a no-material-finding claim to its actual searched scope. | DEC-086; 04 §6.6; 02 §6.6 | AOS-10-VER-032 |
| AOS-10-REQ-042 | **Research disposition:** AOS-10 shall track each material research finding to an accepted human reviewer or an owned unresolved handoff with approved cover/escalation. | DEC-086; 13/30; COORD ACC | AOS-10-VER-033 |
| AOS-10-REQ-043 | **Research amendment:** AOS-10 shall not treat source publication, research acceptance or a proposal as authority to amend a specification, expand sensing or activate a changed operation. | DEC-086/018; 01 §10.8; 04 CON-009 | AOS-10-VER-033 |
| AOS-10-REQ-044 | **Governance contribution:** Asset governance submissions shall expose omissions, conflicting evidence and distributional effects separately from institution-wide judgements or a certificate of safety. | FP1–10; RP3/5/6/7; GT M1.2/3/14 | AOS-10-VER-019 |
| AOS-10-REQ-045 | **Scoped standing:** AOS-10 shall label demonstration fixtures, draft proposals, implemented controls and observed operating outcomes with their actual distinct standing. | QS-09/24–28; 40 §§5/15 | AOS-10-VER-030 |
| AOS-10-REQ-046 | **Retention:** Asset evidence lifecycle shall apply governed retention, correction and deletion to originals and derived views without claiming an audit label creates indefinite retention rights. | DEC-047; 02/03; KPR | AOS-10-VER-026 |
| AOS-10-REQ-047 | **Accountability:** AOS-10 shall distinguish the organisation's governance accountability and operational repair responsibility from statutory building-safety dutyholder appointments. | EXT-02; RP3; 30 §§3/7 | AOS-10-VER-020 |
| AOS-10-REQ-048 | **Observation freshness:** AOS-10 shall assess evidence freshness against the approved observation-purpose profile, recording the material period of lost coverage rather than using one universal freshness interval. | B4 Asset; RP5/9; QS-18 | AOS-10-VER-003 |
| AOS-10-REQ-049 | **Supplier realisation:** Each declared supplier implementation scope shall maintain a versioned allocation of its capabilities/configuration to applicable AOS-10 requirements and contracts, including conformance evidence or owned gaps and dependencies. | Mark's 8 October supplier-participation drafting direction; ARCH logical responsibility catalogue; QS-11/12/21/26 | AOS-10-VER-034 |

### 4.4 External research and specification adaptation

Inherit the common rules of 04 CON-009 and 02 CON-007 / RSVIEW-0.1 without a competing field dictionary. Operational physical sensing and external research are different functions.

| Profile element | Component-owned allocation |
| --- | --- |
| Remit/baseline | AOS-10 exact revision, including supplier participation; condition evidence, inspection practice, physical hazards, repair/maintenance analysis, sensing boundaries, investment assumptions and building-safety information; affected CAP/FUN/REQ/CON identified |
| Developments/sources | Applicable law/regulator/standards changes; competent inspection research; sensor reliability/security; asset-data practice; incidents and maintenance evidence; prefer original regulator/government/standards issuer/research sources; jurisdiction, tenure, lifecycle and source standing explicit |
| Assignment/triggers | Asset owner appoints bounded agent/shared service and approves cadence, event triggers and coverage expectations. No schedule or always-on scanning activated by this draft; unknown setup is ISS-006 |
| Controls | External retrieval through 14; tools/rights/purpose under 01/03/04/05; licence/access/privacy limits; no optional resident sensing expansion, hostile instructions, vendor endorsement or self-calibration |
| Evidence/assessment | Publication/event/access/effective dates, verified content versus interpretation, exact affected elements, alternatives, uncertainty, materiality/urgency and impacts on 11/13/14/22/30/40 |
| Coverage/quality | Complete/partial/failed/unperformed and bounded no-material-finding; source fidelity/relevance and false/missed finding rubric approved by competent humans; actual search perimeter and limitations retained |
| Human review/change | Accepted reviewer, response window, cover and escalation from approved profile; accepted/rejected/deferred/unresolved findings with rationale; separate 01 amendment, verification, activation and outcome records |
| Records/adoption | Common profile/run/finding/disposition views and exact revisions; 02 admission, 14 retrieval, 13 duty tracking, 30 disposition, 01 amendment; corrections/deduplication/selective reassessment per common definitions; no new IF family |

Normal: trigger → permitted retrieval → source verification → specialist assessment → material finding or bounded no-finding → accepted review/disposition → separately approved amendment → verification/activation/outcome. Degraded: denied/stale/conflicting/partial retrieval preserves actual coverage and owned uncertainty; unresponsive reviewers invoke approved cover. A suspected live safety concern uses the already permitted human protocol while research/amendment remains pending. VER-023/031–033 cover all eight required research dimensions. Research remains inactive until the commissioned profile exists.

## 5. State model

Persistent states are governed object meanings, not powers acquired by transition. Each change identifies actor, current authority, source revision, event/effective time, evidence and resulting scope. Approved profile timeouts cause explicit stale/expired/unacknowledged status and owned follow-up; they never mean success.

| Object | States / entry, transition and closure rules |
| --- | --- |
| Observation | Received → admitted or rejected/quarantined; admitted may become contested/corrected/superseded/restricted/deleted under 02/03. Source admission is not assurance that its claim is true. |
| Condition/coverage view | Known within stated scope, uncertain/conflicting, partial, stale or unavailable. New evidence creates a new revision; a human inspection can establish only its evidenced scope/time, not permanent safety. |
| Repair evidence | Promise unresolved or established; completion unverified, evidenced incomplete, partial, disputed or established under the repair-specific rule. After B, unverified completion retains DEC-039 classification. Process owns overdue/duty state; human-authorised communicated revision preserves original/breach history. |
| Finding/duty | Prepared → submitted → received → accepted by empowered human → in progress → evidenced disposition/outcome. Receipt is not acceptance; 13 owns tracking, cover and escalation; 10 retains its evidence contribution. |
| Building information | Applicability unresolved/profiled; category missing/present/current/contested/superseded; transfer prepared/delivered/usable-confirmed or failed/unconfirmed. Handover closure needs required confirmations and owned residual gaps. |
| Research | Common profile/run/finding/disposition states from 02 §6.6; no local replacement. Accepted finding does not mean approved amendment or activation. |

## 6. Semantic contracts and interfaces

These are logical domain views of shared meanings, not newly approved wire schemas or IF identifiers. Preserve AOS-02-IF-001, AOS-01-IF-001, proposed AOS-03-IF-001/AOS-04-IF-001 and existing AOS-13-IF-001 where consumed. Common semantic owners remain authoritative.

| CON | Producer → consumer / minimum meaning / authority and failure |
| --- | --- |
| AOS-10-CON-001 Asset observation | Human/source adapter via14 → 02/10: organisation, building/property/component and relationship revision; source/method; physical quantity/unit/calibration basis where applicable; observed/admitted times; purpose, assurance, uncertainty, correction/access/lifecycle. 02 REC-E/Q owns common evidence; invalid or ambiguous scope stays rejected/unresolved. |
| AOS-10-CON-002 Living Asset Register | 10 through02 → permitted service/22/24/30: exact object/view revision, observations versus inference, condition/time/coverage cells, conflicts/freshness/gaps, model/rule, limitations and lineage. Unsafe aggregation prohibited; no claim beyond evidenced scope. |
| AOS-10-CON-003 Physical finding/action/outcome | 10/competent humans → 13/30/02; returned work evidence →10: concern, physical consequence/exposure, urgency basis, tracker/owner/cover, acceptance, authorised action, attempted/partial/actual effect and resulting observation. Common REC-Q/A/D/X and ACC; receipt is not accepted responsibility. |
| AOS-10-CON-004 Repair evidence | Controlled records/human/contractor via14/02 →10→13/11/30: repair and promised scope, original communicated commitment, precision/timezone and communication proof, authorised revisions, internal targets separate, completion rule/work/inspection evidence, completion time, incomplete/partial/unverified/disputed classification and provenance. 02/Profiles and DEC-036–041 own shared semantics; 13 detects/tracks, 11 delivers contact, 30 supports human decisions. |
| AOS-10-CON-005 Planning/governance input | 10 with permitted02/14 inputs →22/24/30/25: physical condition, scenario/horizon, costs/resource constraints, alternatives, distributional consequences, uncertainty/coverage, actual outcome and precise standing. REC-E/Q; no approved capital decision or institution-wide pass inferred. |
| AOS-10-CON-006 Building-safety view/transfer | Competent stewards/02/10 → permitted dutyholders/humans/external recipients through14: exact building/lifecycle/applicability profile, category inventory, current versions/history, gaps, authorised audience, delivery/usability confirmation and owned residual duties. Shared custody/access/exchange definitions; no statutory completeness inferred from transfer alone. |
| AOS-10-CON-007 Own research | Assigned research service/14/10 →02/13/30/01/affected owners: common profile/run/finding/disposition meanings, exact affected elements and asset-specific implications under RSVIEW-0.1; failed/partial retrieval and unaccepted reviewer remain explicit. |

Every exchange includes stable IDs/revisions, organisation/entity, producer/consumer, exact contract/view, purpose/use/authority references, event/effective/admission time and standing. Physical units and comparison precision must be explicit; invalid values/unknown applicability cannot support a favourable result. Arrival order is distinct from effective time; duplicates retain identity and do not add independent evidence. Acknowledgement distinguishes transport receipt, duty acceptance, usable handover and factual assurance. Retries reconcile prior effects and current permissions; correction/revocation reopens materially affected views/work. Wire types, enumerations, conversion/calibration rules, ordering/deduplication keys, transport timeouts/retry bounds and exact endpoint compatibility require approved profiles before build; no implicit values are supplied here. Asset service owner with 02/13/14 controls those gates, ISS-001/002.

### 6.1 Supplier interface detail and ownership

The CON views specify the meaning to preserve; they are not an API implementation specification. For each proposed integration, supplier and organisation must agree exact field/schema/view versions, identity mapping, physical units, event/effective times, analytical labels and evidence references, access/authority enforcement, transport and authentication, acknowledgement, ordering/deduplication, retry/replay/revocation, service limits, outage handling, retention/correction/deletion and reconciliation. Declare read versus write/command rights explicitly. Existing APIs/events/manual exports are candidates to map, not selected transport defaults.

The supplier declaration identifies the authoritative source for each observation, inference, promise, work status and outcome, and which party maintains each mapping/control. A supplier platform spanning 10/11/13/14 must demonstrate each responsibility and cross-function boundary even if the exchange is internal to one product. Outsourcing cannot make evidence, permissions or human acceptance unobservable. Exact executable agreements and observed compatibility remain ISS-001/003/005, linked to REQ-038/049 and VER-030/034.

## 7. Authority and decision boundaries

Permitted Mode 1 work can admit evidence, apply approved deterministic rules, produce bounded analysis and send an expressly delegated internal finding. A request to issue work, purchase materials, change a resident promise, operate a device or disclose externally is a separate consequential operation requiring current controls. No physical actuator authority is granted by connection or by this draft; any later actuator scope must be commissioned under the same exact delegation/data-use/runtime controls.

Human decisions include applicability/dutyholder appointments, disputed closure, promise/scope revision, repair-specific completion-rule approval, safety response under the approved protocol, capital allocation and incommensurable judgement. Board governance and statutory human duties remain distinct. Technical condition scores cannot adjudicate residents' legitimacy, consent or moral priority. Model-provider substitution cannot inherit an untested asset quality claim.

Revocation or changed evidence affects the last enforceable point and dependent pending work under current common controls. Explain constraint meaning, authority basis and referral by default under DEC-027; any reviewed privacy/security/feasibility explanation exception limits disclosure, not enforcement. Human sign-off cannot waive a non-waivable prohibition.

## 8. Reasoning principles applied

FP1 ties evidence to conferred purpose; FP2 reserves incommensurable trade-offs; FP3 requires enforced integrity; FP4 makes evidence/limits legible; FP5/6 require fault/uncertainty handling; FP7 protects residents with limited exit; FP8 preserves human constitutional authority; FP9 distinguishes purpose-led design from legal validation; FP10 requires interactions and cumulative consequence review. These are technical contributions, not full-principle conformance claims.

| RP v6 domain / thematic locator | Application / planned evidence |
| --- | --- |
| 1 Architecture/completeness, sequenced human layers, feedback | CON-003/004; VER-008/017/018/029; unaccepted duty never vanishes |
| 2 Modes, protected human space, standing boundaries | §§7/9; VER-009/019/024/033; no AI capture of protected board deliberation |
| 3 1+5, intrinsic risk, safety, Golden Thread | VER-008/020–022; asset contributes without replacing dutyholders or governance |
| 4 Options/decisions, actual state/consequence feedback | VER-018/019; observations, forecasts and actual effects distinct |
| 5 Blind spots/perimeter/emergence | VER-003/005/019/028/029; aggregate indicators expose gaps and distribution |
| 6 Ethics/telos/no-exit/purpose drift | VER-019/024/025; no optional-sensing penalty or automatic moral/capital choice |
| 7 Radical transparency/uncertainty | VER-002–007/018/021; source and inference separately reconstructable |
| 8 Delegation, internal/external duty | VER-009/017/022/033; exact authority, accepted owner and failed handoff visible |
| 9 Sensing, asset/behaviour boundary, permitted purpose | VER-001/024/025/027; physical evidence is not individual conduct inference |

Appendix A supplies all 29 GT tests, including bounded non-software contributions. None is marked passed from drafting. Apparent conflict remains evidenced and referred to the empowered human authority.

## 9. Data, privacy and disclosure

Physical evidence can still expose personal information: dwelling linkage, photographs, report text and patterns of sensor readings require purpose/access/inference controls. Minimise person-linked content; keep detailed source evidence separately controlled where an aggregate view is sufficient. A resident report is attributed evidence about physical condition, not automatic permission to construct a personal profile. Emotional/preferences context is human-provided or confirmed under DEC-088; asset signals cannot silently supply it.

Optional sensing refusal/withdrawal cannot reduce access to core services. Accessible manual reporting/inspection arrangements remain permitted, with any practical gaps exposed rather than blamed on residents. Distinguish consent from other lawful bases and organisation authorisation; no blanket consent assumption is introduced. A refusal of access to a particular visit is neither proof of safe condition nor a licence for alternative surveillance; refer service/access needs to humans through 11/13.

Apply 02/03 retention, correction, deletion and restrictions to source records, summaries, models/indices and restored copies. Corrections preserve standing without granting indefinite retention of deleted content. Confidentiality uses audience/purpose-specific restrictions and necessary accountable review, not suppression of material uncertainty. Building-safety access obligations require competent profile mapping; “golden thread” is not unlimited disclosure rights. AI must not observe protected board deliberation; subsequent authorised human accounts are distinct.

## 10. Behaviour and workflows

### 10.1 Condition and maintenance

Trigger → admitted physical evidence/provenance → scoped condition/coverage assessment → current use/authority → bounded finding/forecast → 13 accepted human route or approved intervention → actual work/inspection evidence → revised condition and learning. Missing sources create explicit coverage loss with manual fallback. Conflicting observations preserve both accounts and referral. A suspicion of acute risk uses the separately approved human safety protocol; neither sensors nor ordinary meetings are prerequisites to that referral. No prediction closes the underlying concern.

### 10.2 Repair promise and completion

Source original resident-communicated promise, scope and precision through controlled records. Date-only commitments end at the end of the promised calendar date in the approved organisation timezone; exact-time commitments use their time. B is the symbolic approved boundary, not a new configurable grace period. AOS-13 performs comparison and tracking using evidence supplied by10.

Before or at B, do not falsely assert overdue status. After B, evidenced outstanding promised work supports overdue-incomplete; unknown completion is **completion unverified after promised date**, requiring owned verification under DEC-039. A missing/conflicting promise is a different owned evidence exception. Established on-time completion supports no overdue-repair alert; completion after B preserves historical lateness even if work is now complete. Contractor closed status alone and resident silence do not establish completion.

Partial work retains original incomplete standing; human-authorised scope changes and communicated revisions preserve promise/breach history. A new promise does not automatically close an escalation. Dispute preserves opposing evidence and human review. 13/30 track explicit human acceptance and actual service action; 11 delivers current named-owner and accountable-team contact details through resident-agreed channels. Sending contact details, accepting duty and repairing the home are distinct outcomes. Failed communication and absent acceptance remain owned.

### 10.3 Investment and building information

Planning request → current scoped condition/coverage → alternative resource/scenario assumptions → unranked evidence and consequence inputs to22 → human consideration/decision through30 → authorised implementation → actual physical/financial outcomes. No composite condition score dictates value trade-offs.

Building profile/update/handover → competent applicability/category inventory → current, versioned, audience-checked information → permitted transfer → separate receipt and usable confirmation → outstanding categories/duties → actual follow-up. Statutory records and governance evidence remain distinct; software supports custody, not a legal certificate. Phase-effective/source changes trigger research and human mapping, not silent activation.

## 11. Failure, escalation and recovery

Lost telemetry, inaccessible inspection, corrupt units or missing provenance produce disclosed coverage limits and owned evidence/service follow-up. Human-approved manual routes remain available; a quiet feed is not proof of safety. A suspected acute concern is not delayed merely because analytical confidence is low; communicate uncertainty through the approved human protocol.

Unknown prior work/device effect requires reconciliation before retry. A lost handoff remains with its tracker until empowered acceptance; approved cover applies when the primary human is absent. If both normal and fallback reporting fail, preserve an owned exception and approved human fallback without creating new contact powers. Failed or partial work cannot become completion through a restored status snapshot.

Restore isolated state, apply current authority/use/lifecycle restrictions, reconcile original and subsequent effects and prove current evidence/version scope before approved continuation under05/KPR. Recovery does not retroactively validate missing inspections or resolve an outstanding safety duty. Maintain human service continuity without requiring a successful model output.

## 12. Evidence, provenance and audit

Consequential records link trigger → exact source/scope/assurance → actor and analytical/rule revision → authority/use checks → finding/human rationale → attempted/performed/prevented action → consequence → challenge/intervention → outcome. Include observed/admission/effective times, units, uncertainty, omitted scope, tracker/owner/cover and version/retention/access references. Evidence owner is the asset steward for domain meaning and02 for shared records; human dutyholder and workflow records retain their separate owners.

Capture applied rules, input references, outputs, transitions and approved human rationale; private model chain-of-thought is not required. Retrospective generated explanations do not prove a prior check or inspection occurred. Integrity hashes cannot prove factual truth or completeness. Synthetic fixture truth is explicitly different from live observations. Review actual misses, near-misses and distributional consequences through permitted25/30 processes without automatic self-calibration.

## 13. Security and operation

05 governs runtime/security/resilience;14 governs external trust. Asset-specific source profiles specify device identity, permitted physical quantities/purposes, calibration/quality provenance, transport integrity, segmentation/isolation and revocation where relevant. Supplier credentials, telemetry and retrieved text must not bypass action authority. Quarantine malicious/unauthenticated/replayed or impossible data; expose lost coverage and preserve allowed human service.

Performance/availability/recovery/freshness/inspection coverage and human response capacity are scope-specific approved parameters, not invented universal thresholds. Analytical evaluation distinguishes deterministic controls from probabilistic fidelity, missed/false hazards, forecast calibration, excluded conditions and population/distributional error. Competent human owners approve task, fixtures, rubric, thresholds, uncertainty communication, change triggers and representative assessment before claims. Longitudinal review compares predicted versus actual effects without automatically changing models or rules. Critical control failures cannot be averaged away by a favourable model score.

## 14. Invariants

| INV | Invariant / linked REQ / VER |
| --- | --- |
| AOS-10-INV-001 | Missing observation never establishes safe condition; 004/008/035/048 → 003/006/029 |
| AOS-10-INV-002 | Source content, admission and prediction create no action authority; 009/012/043 → 007/009/033 |
| AOS-10-INV-003 | Internal targets cannot silently reset resident promises; 013–015 → 010–012 |
| AOS-10-INV-004 | Unknown completion after B remains unverified; contractor status/silence alone is insufficient; 016/017/019 → 013/014/016 |
| AOS-10-INV-005 | Physical signals do not imply permission for individual behaviour inference; 028/029 → 024 |
| AOS-10-INV-006 | Declining optional sensing does not remove core service; 030 → 025 |
| AOS-10-INV-007 | Golden-thread custody/transfer does not confer legal completeness or replace statutory duties; 024–027/047 → 020–023 |
| AOS-10-INV-008 | Accepted research cannot activate its own amendment; 039–043 → 031–033 |

## 15. Conformance and acceptance

All claims below are **unsubstantiated planned claims**; no cases have been executed. Test records later require exact versions, date, assessor, environment, method, observed evidence and limitations. Demonstration/document review does not prove live operation, legal compliance or institutional judgement.

| CR | Proposed bounded claim / linked requirements and evidence |
| --- | --- |
| AOS-10-CR-001 | Evidence/register/coverage semantics; 001–010/048; VER-001–007 |
| AOS-10-CR-002 | Risk/repair/outcome boundaries; 011–022/032/037; VER-008–018 |
| AOS-10-CR-003 | Planning and building-safety information contribution; 023–027/044/047; VER-019–023 |
| AOS-10-CR-004 | Permitted secure correctable/recoverable operation; 028–038/045–046; VER-024–030 and 018 |
| AOS-10-CR-005 | Own research/profile/review/change boundaries; 039–043; VER-031–033 and 023 |
| AOS-10-CR-006 | Declared supplier scope is attributable and evidence-limited; 049; VER-034 plus the allocated functional cases |

Common case preconditions: fixed exact component/common-contract/source manifest; approved isolated synthetic fixtures and destinations or explicitly labelled document walkthrough; competent appointed assessors; approved identity/purpose/authority/current restriction profiles, clocks/units and expected-result rubric where applicable. Missing approval/fixture produces blocked/not-performed, not pass. Planned methods are component/integration boundary tests with human review; a document walkthrough may assess logic but not implementation enforcement. Evidence for each case includes input/expected fixtures, actual ordered admission/check/output/effect, versions, human judgement where required, uncertainty, findings/remedy/accepted owner and rerun links. Assessors below own comparison against the stated expectation; no model certifies itself.

### AOS-10-VER-001 — Scope and identity

**Requirements:** AOS-10-REQ-001, AOS-10-REQ-002. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Two organisations, a building, communal component and dwelling; an unresolved duplicate property identifier and a changed ownership relationship.

**Procedure:** Admit each record; change the effective relationship; attempt to merge unresolved identifiers and cross the organisation scope.

**Expected result:** Exact entity and effective relationship remain visible; ambiguous identity is unresolved and cross-scope use is denied.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Property/organisation identity steward; CON-001. Explicit enforcement observations required for any control claim.

### AOS-10-VER-002 — Observation semantics

**Requirements:** AOS-10-REQ-003. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Physical inspection, resident report and sensor reading with distinct event/admission times; valid and invalid units.

**Procedure:** Admit, render, reorder and correct records; attempt a unit-free numerical comparison.

**Expected result:** Source/method/units/time/assurance/lineage survive; invalid meaning cannot support a condition conclusion.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Data and asset assessors; CON-001/002. Explicit enforcement observations required for any control claim.

### AOS-10-VER-003 — Coverage and freshness

**Requirements:** AOS-10-REQ-004, AOS-10-REQ-048. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Coverage cells containing fresh, stale, absent, inaccessible and failed data; approved symbolic freshness profile F.

**Procedure:** Render individual and aggregate views across the observation boundary; remove a feed and attempt to display a uniformly safe portfolio.

**Expected result:** Gaps and lost-coverage periods remain visible per scope; no average conceals an unobserved hazard/property.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Asset/assurance assessors; CON-002. Explicit enforcement observations required for any control claim.

### AOS-10-VER-004 — Register meanings

**Requirements:** AOS-10-REQ-005. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Observation, model condition, forecast, authorised work and subsequent inspection for one component.

**Procedure:** Build the view and follow every lineage link; attempt to present a forecast as an inspection or planned work as actual improvement.

**Expected result:** Distinct meanings and exact evidence standing are preserved; unsupported favourable status is rejected.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Asset/data assessors; CON-002/003. Explicit enforcement observations required for any control claim.

### AOS-10-VER-005 — Conflict

**Requirements:** AOS-10-REQ-006. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Contradictory inspection and sensor evidence, delivered in both orders.

**Procedure:** Admit both; calculate a view; request clarification and apply an authorised correction.

**Expected result:** Arrival order does not resolve fact assurance; contradiction and owned review persist until evidenced disposition.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Asset inspector/data assessor; CON-001/002. Explicit enforcement observations required for any control claim.

### AOS-10-VER-006 — Physical and manual evidence

**Requirements:** AOS-10-REQ-007, AOS-10-REQ-008. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus A home without sensors, a failed feed, an identifiable physical assessment and an unsupported claim that telemetry proves that assessment.

**Procedure:** Admit manual evidence, retain its scope/limitations, and attempt to mark physical assessment complete using telemetry alone.

**Expected result:** Manual assessment remains supported; physical-assessment standing requires actual evidence; unobserved scope remains explicit.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Competent inspection/service assessors; CON-001/002. Explicit enforcement observations required for any control claim.

### AOS-10-VER-007 — Inference and forecast

**Requirements:** AOS-10-REQ-009, AOS-10-REQ-010. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Known fixture conditions, out-of-distribution cases, forecast assumptions/horizon and absent evaluation basis.

**Procedure:** Produce outputs; vary assumptions; compare observation and interpretation; request certainty outside evaluated scope.

**Expected result:** Inference/forecast carry versions, assumptions and uncertainty; unsupported certainty/accuracy claims do not pass.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Asset/model evaluation assessors; CON-002/005. Explicit enforcement observations required for any control claim.

### AOS-10-VER-008 — Acute concern and risk

**Requirements:** AOS-10-REQ-011, AOS-10-REQ-022. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Suspected urgent physical hazard, uncertain cause, approved human safety protocol, unavailable primary owner.

**Procedure:** Detect concern, send bounded permitted referral, activate approved cover, and delay normal governance review.

**Expected result:** Concern reaches an empowered human route without waiting for ordinary review; uncertainty is retained; no novel emergency agent power appears.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Safety/workflow assessors; CON-003; 30 safety boundary. Explicit enforcement observations required for any control claim.

### AOS-10-VER-009 — Action and authority

**Requirements:** AOS-10-REQ-012. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Permitted evidence-read operation, proposed work order or physical-device command, expired/revoked permission.

**Procedure:** Exercise current checks at the last enforceable point; attempt denied and revoked operations.

**Expected result:** Only exactly permitted effects occur; prevention is observable; analytical capability cannot create work/actuator authority.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Authority/security assessors; common REC-A/D/X, CHECK/ACT. Explicit enforcement observations required for any control claim.

### AOS-10-VER-010 — Promise versus target

**Requirements:** AOS-10-REQ-013. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Communicated promise P, later internal target T, provenance, missing/contradictory communicated date.

**Procedure:** Supply each evidence variant to Process; attempt to replace P using T.

**Expected result:** P remains authoritative for the resident-promise comparison; unavailable P creates an owned evidence exception, not a fabricated date.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Repairs/data assessors; CON-004; 40 VER-008. Explicit enforcement observations required for any control claim.

### AOS-10-VER-011 — Promised boundary

**Requirements:** AOS-10-REQ-014. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Approved date-only organisation timezone and precise-timestamp commitments; immediately before/at/after boundary B.

**Procedure:** Compare the fixtures using approved profile meaning, including a calendar transition; try an added grace interval.

**Expected result:** Date-only boundary is end of that date; exact timestamps retain precision; no overdue status at/before B; no default grace period.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Repairs/time-profile assessors; CON-004; 40 VER-008. Explicit enforcement observations required for any control claim.

### AOS-10-VER-012 — Promise revision

**Requirements:** AOS-10-REQ-015. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus P, authorised communicated revision P2, internal reschedule, unauthorised revision and outstanding escalation.

**Procedure:** Attempt all revisions and inspect preserved history and workflow status.

**Expected result:** Only authorised communicated revision acquires new-promise standing; original/breach history survives and existing escalation is not automatically closed.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Repairs/human workflow assessors; CON-004; 40 VER-008. Explicit enforcement observations required for any control claim.

### AOS-10-VER-013 — Completion rule

**Requirements:** AOS-10-REQ-016. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Repair-specific approved rule, identified work and inspection records, contractor closed flag alone and resident silence.

**Procedure:** Evaluate each variant; seed complete evidence both before and after B.

**Expected result:** Completion standing follows the rule and evidence; contractor flag/silence alone cannot establish completion; actual completion time is preserved.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Repairs/inspection assessors; CON-004; 40 VER-007/008. Explicit enforcement observations required for any control claim.

### AOS-10-VER-014 — Unknown completion

**Requirements:** AOS-10-REQ-017. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus t>B and unavailable or conflicting completion evidence; separate evidenced outstanding-work case.

**Procedure:** Supply classifications to Process; request definitive overdue-incomplete and definitive complete statuses.

**Expected result:** Unknown variant is “completion unverified after promised date” and gets owned verification; evidenced incomplete variant may support overdue-incomplete; neither is silently conflated.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Repairs/workflow assessors; CON-004; 40 VER-008. Explicit enforcement observations required for any control claim.

### AOS-10-VER-015 — Partial scope

**Requirements:** AOS-10-REQ-018. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Two promised tasks, one complete; proposed split or scope revision without human/resident evidence.

**Procedure:** Render completed/outstanding tasks; attempt to close original or erase its promise by splitting.

**Expected result:** Original remains incomplete; each scope part is visible; changed scope requires authorised human and resident communication evidence.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Repairs/service assessors; CON-004. Explicit enforcement observations required for any control claim.

### AOS-10-VER-016 — Contested completion and challenge

**Requirements:** AOS-10-REQ-019, AOS-10-REQ-032. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Resident contests closure, contact channel is agreed, contractor evidence conflicts; silence alternative.

**Procedure:** Preserve evidence, refer through 11/13, test failed delivery and absent human acceptance, then authorised dispute disposition.

**Expected result:** Dispute is owned and contestable; silence/delivery do not resolve it; permitted resident evidence and actual disposition remain linked.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Resident/repairs/workflow assessors; CON-004; 40 VER-010. Explicit enforcement observations required for any control claim.

### AOS-10-VER-017 — Handoff and duplicates

**Requirements:** AOS-10-REQ-020. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Condition finding, duplicate event, unavailable owner and unacknowledged workflow transfer.

**Procedure:** Send/retry with stable identities, separate receipt from acceptance, invoke approved cover and inspect pending status.

**Expected result:** No duplicate consequential action; duty remains owned until empowered acceptance; failed cover remains an exception.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Workflow/asset assessors; CON-003; 40 VER-009. Explicit enforcement observations required for any control claim.

### AOS-10-VER-018 — Outcome and audit

**Requirements:** AOS-10-REQ-021, AOS-10-REQ-037. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Inspection finding, human-authorised action, partial execution, subsequent outcome and failed intervention.

**Procedure:** Follow trigger-to-outcome links; request reconstruction using captured evidence; attempt to use a later generated explanation as proof.

**Expected result:** Attempt/action/improvement are distinct; authority/rationale/consequence reconstructable; missing contemporaneous evidence stays a gap.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Asset/audit assessors; CON-001/003. Explicit enforcement observations required for any control claim.

### AOS-10-VER-019 — Investment and governance

**Requirements:** AOS-10-REQ-023, AOS-10-REQ-044. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Contrasting physical condition, costs/resources and unequal impacts; an infeasible option and competing incommensurable objectives.

**Procedure:** Prepare scenarios with 22; vary assumptions; request an automatic capital commitment or a scalar institutional pass.

**Expected result:** Actual constraints/uncertainty/distribution remain legible; alternatives preserved; human allocation and moral judgement remain reserved.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Asset/finance/governance human assessors; CON-005; 40 VER-013/027. Explicit enforcement observations required for any control claim.

### AOS-10-VER-020 — Building applicability and accountability

**Requirements:** AOS-10-REQ-024, AOS-10-REQ-047. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Two buildings with different human-approved lifecycle/applicability profiles and dutyholders; incomplete category inventory.

**Procedure:** Construct views; attempt to infer full legal applicability from a height field or replace statutory appointment with board approval.

**Expected result:** Profile/category gaps remain owned; statutory dutyholder and governance responsibility stay distinct; no autonomous legal determination.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Competent building-safety/legal and governance assessors; CON-006. Explicit enforcement observations required for any control claim.

### AOS-10-VER-021 — Building information custody

**Requirements:** AOS-10-REQ-025. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Current, superseded, missing and contradictory safety records plus authorised/unauthorised audiences.

**Procedure:** Update current view with history preserved; request access, corrections and plain-language usability review.

**Expected result:** Exact current versions and gaps visible; secure audience checks enforced; usability requires human evidence, not digitisation alone.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Building-safety/data/access assessors; CON-006; 40 VER-036. Explicit enforcement observations required for any control claim.

### AOS-10-VER-022 — Building information transfer

**Requirements:** AOS-10-REQ-026. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Authorised handover recipient, exact inventory, delivery failure and delivered-but-unusable package.

**Procedure:** Transfer through 14; reconcile retry; obtain separate receipt/usability confirmation and maintain unresolved duties.

**Expected result:** Delivery is not usable acceptance; failed/missing items remain owned; exact versions and permissions survive transfer.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Building-safety/boundary assessors; CON-006; 40 VER-036. Explicit enforcement observations required for any control claim.

### AOS-10-VER-023 — Current versus future regulation

**Requirements:** AOS-10-REQ-027. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Current England Phase 1 source, future-effective Phase 2 source, draft and wrong-jurisdiction source; approved operational mapping.

**Procedure:** Record source standing/dates; propose adaptation; attempt premature rule activation and confuse a resident promise with a statutory timing rule.

**Expected result:** Future/draft content does not silently become current law or activation; different timing obligations remain distinct; competent human mapping is required.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Legal/research/service assessors; CON-004/006/007. Explicit enforcement observations required for any control claim.

### AOS-10-VER-024 — Use and prohibited inference

**Requirements:** AOS-10-REQ-028, AOS-10-REQ-029. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Permitted damp/temperature signal, proposed occupancy/habit/emotion inference, unauthorised cross-entity disclosure and hostile source instructions.

**Procedure:** Attempt each operation at enforcement surface; admit permitted physical evidence without unnecessary person profile.

**Expected result:** Only checked physical-purpose operations occur; prohibited inference/disclosure/instructions are blocked and evidenced.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Privacy/security/asset assessors; CON-001; 40 VER-015/017. Explicit enforcement observations required for any control claim.

### AOS-10-VER-025 — Optional sensing

**Requirements:** AOS-10-REQ-030. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Resident declines optional sensors/data use, with core repair need and accessible manual alternatives.

**Procedure:** Exercise decline and withdrawal; inspect service eligibility, manual route and burden under human review.

**Expected result:** Core service remains available; no adverse automated eligibility inference; manual alternative and remaining observation gaps visible.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Resident/privacy/service assessors; CON-001/003; 40 VER-010/015. Explicit enforcement observations required for any control claim.

### AOS-10-VER-026 — Correction and lifecycle

**Requirements:** AOS-10-REQ-031, AOS-10-REQ-046. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Corrected observation, revoked use, dependent forecast/workflow, governed retention/deletion and restored derived copy.

**Procedure:** Map impacts, selectively reassess/restrict affected work, apply lifecycle across copies and inspect historical standing.

**Expected result:** Affected outputs/work are corrected or restricted with lineage; unrelated valid work is not blanket frozen; deletion obligations survive restoration.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Data/privacy/workflow assessors; CON-001/002; 40 VER-025. Explicit enforcement observations required for any control claim.

### AOS-10-VER-027 — Hostile telemetry

**Requirements:** AOS-10-REQ-033. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Unauthenticated device, altered packet, impossible units, replay, compromised vendor connector and malicious payload.

**Procedure:** Attempt admission and downstream action; revoke source permission and inspect quarantine/fallback.

**Expected result:** Invalid/hostile material cannot alter authoritative condition or confer action authority; affected coverage and owned response exposed.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Security/boundary/data assessors; CON-001; 40 VER-020. Explicit enforcement observations required for any control claim.

### AOS-10-VER-028 — Analytical quality

**Requirements:** AOS-10-REQ-034. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Approved task/population/rubric/error thresholds, representative and excluded cases, changed model and subgroup gaps.

**Procedure:** Run repeatable evaluation, assess false/missed concerns and fidelity, change model and compare accepted scope.

**Expected result:** Claim is bounded to accepted evidence and scope; critical control failures cannot average away; unapproved model change cannot inherit quality claims.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Independent competent asset/model assessors; CON-002/005; 40 VER-026. Explicit enforcement observations required for any control claim.

### AOS-10-VER-029 — Outage and recovery

**Requirements:** AOS-10-REQ-035, AOS-10-REQ-036. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Lost feed/dependency, manual service route, unknown earlier work effect and restored stale permission.

**Procedure:** Degrade, operate permitted fallback, restore isolated state, apply current restrictions and reconcile before retry.

**Expected result:** No false safe/complete state; work and coverage stay owned; no duplicated effect or revived permission; scoped continuation needs approved release.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Operations/service/control assessors; CON-001/003; 40 VER-021/022. Explicit enforcement observations required for any control claim.

### AOS-10-VER-030 — Contract compatibility and standing

**Requirements:** AOS-10-REQ-038, AOS-10-REQ-045. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Common exact-version manifest, unsupported unit/view, synthetic data and operating evidence.

**Procedure:** Round-trip each view; reject incompatible semantics; render outputs in all standing categories.

**Expected result:** One authoritative common meaning; unsupported payload unresolved; no synthetic/draft output acquires operational evidence standing.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Data/assurance assessors; all CON views; 40 VER-001/025. Explicit enforcement observations required for any control claim.

### AOS-10-VER-031 — Research relevance and shared duties

**Requirements:** AOS-10-REQ-039, AOS-10-REQ-040. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Approved asset research profile and relevant verified inspection/sensor development; one shared finding relevant to 10 and 14.

**Procedure:** Retrieve through 14, preserve source dates, analyse exact affected sections and route distinct component implications.

**Expected result:** Source versus inference and separate duties visible; source collection does not discharge specialist review.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Asset/research assessors; CON-007; 40 VER-031/033. Explicit enforcement observations required for any control claim.

### AOS-10-VER-032 — Research coverage and hostile retrieval

**Requirements:** AOS-10-REQ-041. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Stale baseline/conflicting source, partial/denied retrieval, no finding in limited scope, hostile instructions and failed run.

**Procedure:** Exercise each run, challenge bounded no-finding claim and source fidelity, prevent instruction/tool expansion.

**Expected result:** Actual coverage/uncertainty exposed; denied/failed run is not reassurance; hostile text creates no authority.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Research/security assessors; CON-007; 40 VER-032/034. Explicit enforcement observations required for any control claim.

### AOS-10-VER-033 — Research review and amendment

**Requirements:** AOS-10-REQ-042, AOS-10-REQ-043. **Method:** component/integration boundary test and competent human review; document walkthrough only until executable fixtures exist.

**Preconditions / inputs:** Common §15 prerequisites plus Material/urgent finding, unavailable reviewer, approved cover and proposed specification/operational change without approval.

**Procedure:** Track handoff/escalation, support separately permitted urgent human response, seek authorised amendment and attempt premature activation.

**Expected result:** Unaccepted duty remains owned; operational response and amendment distinct; approval, verification and activation require their own records.

**Evidence / assessor / counterpart:** Common run evidence plus case-specific source/classification/transition and actual effect records; Research/authority/workflow assessors; CON-007; 40 VER-033/035. Explicit enforcement observations required for any control claim.

### AOS-10-VER-034 — Supplier realisation and coverage declaration

**Requirements:** AOS-10-REQ-049. **Method:** structured supplier-scope inspection and integration walkthrough, followed by actual functional/control tests for any conformance claim. **Assessor:** asset/data/exchange/service owners with competent procurement/security/privacy and relevant human reviewers.

**Preconditions / inputs:** Common §15 prerequisites; a versioned hypothetical supplier offer containing sensors, analytics, portal, case management and resident app; alternatives for portal/manual exchange and API integration; exact requirements/common manifest, supplier capability/configuration evidence and deliberately unsupported claims. No actual supplier is presumed conformant.

**Procedure:** Map hardware/software/functions to exact REQs/CONs and source ownership. Identify direct, configured, integrated and outside-scope contributions. Trace a physical finding through analytical evidence, accepted service duty and actual outcome; inspect missing fields/versions, unavailable method evidence, duplicate case-master conflict and hidden internal handoff. Attempt to declare full AOS-10 conformance from raw readings or the existence of an API. Compare the standalone and combined-platform arrangements against their declared automated/manual scope.

**Expected result:** Every declared in-scope obligation has a responsible implementation party and actual evidence or an explicit owned gap/dependency; existing supplier analytics/workflows may be reused without erasing their provenance or controls; product boundaries do not replace logical responsibilities. Missing evidence/compatibility prevents the dependent claim. Manual exchange is not labelled automated, receipt is not duty acceptance, and no supplier mapping selects a product, grants powers or proves the remaining functional cases.

**Evidence:** Exact supplier/configuration/manifest revisions, requirement-response matrix, contract/source ownership mappings, worked sequence and observed enforcement where executed, evidence references, gaps/owners/remedy gates and human review disposition. Counterparts: 40 REQ-001–003/014/026 and VER-001/025 for assembled scope/compatibility; item12a supplier alignment briefing.

## 16. Dependencies and staged handover

Drafting uses approved source directions and existing logical contracts; 11v0.3/12v0.3/13v0.2 now provide functional counterparts; exact executable mapping and observed end-to-end compatibility remain dependencies. Build requires exact domain view/schema mappings with02/14, completion/date/inspection/coverage profiles, fixtures, sensor/source admission rules, model evaluation and action-check enforcement. Activation additionally requires appointed asset/inspection/safety/service owners, competent applicability/dutyholder inventory, accepted human cover/capacity, permitted resident channels, actual privacy/lifecycle and manual continuity arrangements, scoped commissioning evidence and human release authority. Operations require evidence currentness, inspections, accepted duties, outcome feedback, lifecycle/revocation/recovery and research/profile upkeep.

02 owns shared source/record definitions;01 authority;03 permitted use/identity;04 agent lifecycle;05 runtime;11 resident assistance;13 orchestration;14 exchange;20–25 GI;30 human workflow support;40 assembled assurance. Supplier products, sensor deployments, HACT wire mappings, models and statutory profiles are unselected, not assumed. Exact-version endpoint compatibility must be demonstrated before affected activation.

## 17. Issues and controlled unknowns

All issues are open implementation/detail dependencies rather than requests to infer new general design policy. Confidence is high that the dependencies exist; their organisation-specific values are unassessed. Resolution requires evidence and explicit disposition, not an issue being mentioned in a draft.

| ISS / type | Description / source / affected capability | Owner / evidence / gate / disposition |
| --- | --- | --- |
| AOS-10-ISS-001 dependency | Exact domain/common mappings, HACT version/licence, identities/units/enumerations and endpoint compatibility; §6/DEC-048, all CON | Asset/data/exchange stewards; versioned mappings and round-trip evidence before affected build; open, no defaults |
| AOS-10-ISS-002 dependency | Source/inspection/freshness/coverage/calibration profiles, approved clocks/precision and repair completion rules; CAP-001/003 | Asset/inspection/repairs owners; approved profiles and fixtures before dependent build/test; open |
| AOS-10-ISS-003 dependency | 11v0.3/13v0.2 executable resident-channel/duty lifecycle integration; CAP-002/003 | Domain/service/30/40 owners; exact REQ/VER adoption and synthetic end-to-end execution before repair activation; open |
| AOS-10-ISS-004 dependency | Building lifecycle/applicability, category inventory, legal timing and statutory dutyholder profiles; CAP-005 | Competent safety/legal/dutyholder humans; approved current-source mapping and actual custody/usability evidence before compliance/activation claim; open |
| AOS-10-ISS-005 dependency | Analytical tasks/model/supplier choices, evaluations, human safety cover, capacity and manual continuity; CAP-001/002/004/006 | Asset/model/security/service owners; approved rubric/control/fallback evidence before dependent operation; open |
| AOS-10-ISS-006 dependency | Own research assignment/triggers/coverage/rubric/reviewer windows/cover; CAP-007 | Asset/research/14/13/30 owners; approved common profile and VER-023/031–033 evidence before research activation; open |
| AOS-10-ISS-007 dependency | Review, source sufficiency and actual evidence after current row allocation and release/assurance evidence; all CAP | Mark/source/40/qualified reviewers; disposition, exact manifest and executed scoped cases before readiness/conformance; independent project review deferred; open |

## 18. Implementation guidance — non-normative

An evidence graph or versioned register can link dwellings, components, inspections, reports, work and outcomes. A coverage matrix by property, concern and period is useful because a portfolio average can conceal an unobserved hazard. Source adapters can normalise units while retaining originals and conversion provenance. A digital twin may support this, but neither 3D geometry nor a named platform is required.

Treat building-safety information as a governed category inventory with controlled current views and transfer receipts, not a folder whose existence proves completeness. Keep promise and internal schedule as separate fields. Use symbolic fixture B/F during functional review; builders must receive approved concrete comparison/freshness profiles. None of these patterns selects a technology, approves sensing or licenses a vendor.

### 18.1 Worked supplier example — illustrative, not a conformance assessment

Aico/HomeLINK is an illustrative candidate because its published offer includes environmental sensors/gateway, analytical portal, case management and resident app. Public pages consulted 8 October 2026: [HomeLINK products and capabilities](https://www.aico.co.uk/homelink/) and [standalone dashboard and integration discussion](https://www.aico.co.uk/blog/not-another-dashboard/). These establish an architectural discussion basis, not exact API availability, contract compatibility or tested conformance. No product has been selected.

For example, a humidity/temperature observation from an installed sensor is supplied with device/property identity and event time. A supplier analytics service interprets a possible damp/mould risk. The observation and attributed analytical finding enter governed02 records through14 and populate10's condition/coverage view; a finding can reference the supplier's analysis rather than duplicate it.

The approved response route passes the finding to13. This could be realised by the supplier's case-management software or an existing repairs platform: the declared case master records accountable ownership, explicit human acceptance and permitted inspection/work. A resident app could realise relevant11 interactions only within the agreed channel/use/access arrangements, with an accessible alternative. A competent inspection and subsequent work supply actual evidence;10 updates condition, preserving original finding, uncertainty and outcome.22/30 can receive permitted governance inputs, with original and residual gaps visible.

This example is a possible implementation pattern. It does not assert that the named supplier exports every required item or satisfies the AOS completion, privacy, handoff or authority rules. Those are questions for the response matrix and tests. An unavailable sensor produces explicit lost coverage and permitted manual assessment; an alert alone proves neither damp's cause nor repair completion. An operational supplier UI may remain in use alongside AOS governance presentation; no forced replacement dashboard is implied.

## 19. Traceability and change

§2 source/approved decision → §4 CAP/FUN/REQ → §5 state and §6 CON → §14 INV → §15 VER → future exact executed evidence. Each requirement row links its planned case and each case names its requirements; sources/status/owner/history are inherited only from explicit §4.3 metadata. AOS-00 REQ-041–044/VER-019 and DEC-036–041 allocate to 10 REQ-013–020/032, VER-010–017 and CON-004. AOS-40 REQ-015/016, VER-007–010 consume this evidence; new 40 VER-036 links building-information cases020–022. Evidence contributions to all29 GT tests appear in Appendix A.

0.1 creates initial asset requirements, views and planned cases. AOS-00/Map v0.34 records allocation; 40 v0.2 corrects the unknown-completion contrast to DEC-039 and adds explicit asset/building-information counterparts. No DEC, original source record, approved IF or common meaning is renumbered. Changes require impact analysis and permitted human amendment, preserving exact prior standing and selectively reassessing dependent work under DEC-089.

Version0.2 adds supplier participation (§3.1), integration ownership (§6.1), worked example (§18.1) and response matrix (§20.1). Mark's recorded drafting direction → CAP-008/FUN-009/REQ-049 → existing CON-001–007/common manifest → VER-034 → future exact supplier/implementation evidence. Original REQ-001–048/VER-001–033 remain unchanged; exact supplier obligation allocation is an addition, not a product approval. Architecture/Map v0.35 records this standing direction for all five sensing domains; common/source/DEC statuses remain unchanged.

## 20. Build and operational handover

The functional handover comprises this draft, cited common/source versions, stable requirement/view/case IDs, unresolved dependency owners and the explicit reserved-human boundaries. It is not a build-ready implementation contract. Before an authorised slice, deliver its exact machine-readable/domain mappings, controls, source and analytical profiles, accepted fixture/rubric/case evidence, environment/destinations, role/cover and capacity assignments, manual continuity/recovery arrangements, release/rollback/stop authority and permitted evidence lifecycle.

The selected repair demonstration can stage these dependencies without claiming complete asset coverage. Sensors, investment analytics and golden-thread statutory claims may be excluded from an exact initial slice only with explicit scope/exclusions/owners; no exclusion can erase required safety handling or the approved resident-promise rules. Full functional suite development continues alongside bounded implementation.

### 20.1 Supplier response matrix and integration handover

Use one response row for each exact applicable requirement, referencing its precise revision. The grouped rows below help suppliers organise the initial response; they do not replace requirement-level coverage or let a partial capability count as full fulfilment. Supplier evidence may include existing technical documentation, controlled source references, configuration, demonstrations and actual test results with declared standing.

| Requirement group / exact references | Supplier capability/configuration and extent | Evidence to request | Gaps, integration and accountable party |
| --- | --- | --- | --- |
| Observation/identity/coverage: 001–008/048, CON-001/002 | State hardware/feed/manual sources, quantities, metadata and coverage supported | Sample records, identity/unit/time mappings, quality/provenance, outage/conflict demonstrations | Missing fields/calibration/history, source mapping and inspection responsibilities |
| Analysis/risk: 009–012/022/034, CON-002/003 | State supplier analytics, versions, evaluated scope and proposed referral/control configuration | Method/limitations, validation evidence, false/missed-concern evaluation and enforcement tests | Unavailable evaluation, excluded conditions and human safety route |
| Repair/workflow/outcome: 013–021/032/037, CON-003/004 | State case-management contribution and authoritative promise/work/completion records | Promise/communication/completion examples, accepted owner, partial/disputed/unknown cases and outcome lineage | Other repairs/contact systems, human approval, case-master and reconciliation gaps |
| Planning/governance/building information: 023–027/044/047, CON-005/006 | State scenario/report/repository contribution; identify unsupported scope explicitly | Assumptions/currentness/inventory, audience checks, transfer/usability and applicability evidence | Finance/governance/dutyholder functions and statutory mapping retained elsewhere |
| Permitted secure lifecycle/operation: 028–031/033/035–036/038/045–046 | State security/access/use/correction/deletion/recovery controls and enforcement location | Control/lifecycle evidence, degraded/manual routes, exact compatibility and recovery tests | Shared-control ownership, contract/API versions, service parameters and supplier exit/data portability arrangements |
| Own research: 039–043, CON-007 | State any contracted specialist research contribution or mark outside scope | Bounded profile/run/finding evidence and accepted human review/change links | External source access, common records and retained component owner duties |
| Supplier realisation: 049 | Declare exact product/service/configuration/release scope and requirement allocation | Versioned requirement-by-requirement response and linked actual evidence/owned gaps | Named responsible implementation parties and build/activation/remedy gates |

Each completed row records **exact REQ/version; supplier product/service/configuration; direct/configured/integrated/outside-scope status; met/partial/not-met/not-assessed conclusion with evidence; contract/profile/source ownership; gap and responsible party; required integration/remedy and decision gate**. “Met” requires scoped accepted evidence, not marketing similarity. Outside-supplier-scope does not waive a requirement from an organisational release: another named party must fulfil it or the release must explicitly exclude the capability without waiving governing safety/authority duties.

Use this declaration to agree the integration specification, responsibilities and commissioning evidence. It supports procurement discussions but is not a price request or supplier certification. API/schema/authentication/service details are completed for the selected scope before dependent build/activation; named examples remain explanatory.

## 21. Review and findings

Author checks cover all21 template sections, supplier-facing realisation and 49 proposed requirements/34 planned cases, distinct stable IDs, requirement-to-case reciprocity, complete29-test applicability, explicit missing profiles and preserved source/common/decision meanings. They do not execute any test or provide independent assessment. Specification-quality conclusion: organised functional draft with controlled unknowns and planned verification. Design-adequacy conclusion: author review finds the proposed functional scope consistent with approved physical-sensing, human-authority and repair directions; Mark's judgement and commissioned/executed evidence remain outstanding. No G3/G4, implementation safety, institutional effectiveness or legal-conformance claim is made.

Next functional work is AOS-11 Resident Intelligence and AOS-13 Process Intelligence, each applying Mark's standing supplier-participation consideration, maintaining reciprocal repair/contact/accepted-duty boundaries. Existing pilot, common implementation and independent-review dependencies retain their separate open status.

## Component summary

AOS-10 supplies physical asset evidence, scoped condition/coverage, bounded risk and repair evidence, planning inputs and governed building-safety information. It distinguishes uncertainty from safety, administrative status from completed work, and technical custody from human/statutory accountability. Own research can propose adaptation; humans and common controls retain amendment and operating powers.

## Appendix A — All 29 Governance Intelligence Tests

All institutional test statuses are **not assessed**. The board with competent independent human assessment owns institutional conclusions; asset/service stewards own only the evidence contributions below. Protected board deliberation stays unobserved by AI. Missing evidence is a gap, not a favourable institutional answer.

| Test / controlled title | Asset contribution / planned cases | Human or cross-domain assessment boundary |
| --- | --- | --- |
| M1.1 Strategic Coherence | Condition/investment scenarios; 019 | Board strategy-purpose coherence and actual outcomes |
| M1.2 Sensing Architecture | Observation scope/coverage/failure; 001–007/029 | Whole sensing perimeter across all five domains |
| M1.3 Risk Intelligence | Physical concern and owned referral; 008/017/019 | Board foresight and cross-domain consequence evidence; CAP-02 use case deferred to Phase 2, not a core dependency |
| M1.4 Composition and Capability | Competent inspection/assessor role dependencies; 006/020/028 | Board composition, expertise and diversity |
| M1.5 Performance Legibility | Condition/work/outcome distinction; 004/018/019 | Complete operating/financial futures and performance |
| M1.6 Compliance Assurance | Applicable source/category/standing; 020–023 | Competent legal mapping and actual statutory fulfilment |
| M1.7 Governance Documentation | Current version and lineage; 002/021/026 | Accuracy of actual instruments and policy-practice coherence |
| M1.8 Accountability Architecture | Accepted duties and challenge; 016/017/022 | Actual responsiveness and influence beyond delivery |
| M1.9 Value for Money | Condition/resource alternatives; 019 | Human value objectives, finance and moral trade-offs |
| M1.10 Human-AI Interaction Norms | Action/human boundaries; 009/019/024/033 | Practice under real pressure, not merely controls on paper |
| M1.11 Learning Metabolism | Actual outcome versus forecast; 007/018/028 | Actual understanding/change over time without self-calibration |
| M1.12 Continuous Self-Assessment | Coverage and research; 003/031–033 | Board development/culture and whole-system review |
| M1.13 Emergent System Behaviour | Aggregate gaps/distribution/compound failure; 003/019/029 | Cross-domain/system effects and governed response |
| M1.14 Golden Thread Integrity | Inventory/currency/usable transfer; 020–022 | Statutory dutyholder fulfilment and board accountability |
| M2.1 Values Architecture | Purpose/use/no-exit boundaries; 009/024/025 | Actual structural values and organisational practice |
| M2.2 Coherence Under Pressure | Safety uncertainty and competing constraints; 008/019 | Human account of difficult decisions and reasons |
| M2.3 Incommensurable Trade-off Capacity | Preserved alternatives; 019 | Empowered human adjudication and dissent |
| M2.4 Epistemic Brake Function | Gaps/conflict/unknown completion; 003/005/007/014 | Human unease and actual investigation |
| M2.5 Directorial Independence | Unfiltered uncertain asset evidence; 019/021 | Independent dissent and resistance to framing |
| M2.6 Social Legitimacy | Resident challenge/manual route; 016/025 | Actual resident legitimacy and influence |
| M2.7 No-Exit Obligation | No optional-sensing penalty; 024/025 | Service burden/accessibility and lived resident evidence |
| M2.8 Radical Transparency | Evidence/inference/limitations; 002–007/018/021 | Affected people can interrogate significant reasons |
| M2.9 Moral Drift Detection | Distribution/outcomes and research; 018/019/028/031 | 25/30 longitudinal founding-purpose comparison and response |
| M2.10 Purpose Stability | Purpose-bound physical evidence; 001/024/033 | Board articulation and actual purpose-consistent choices |
| M2.11 Murmuration Capacity | Permitted evidence to independent human review; 019 | Collective sense-making remains human; no boardroom capture |
| M2.12 Constitutional Authority | No authority by inference; 009/019/033 | Board constitutional mediation and substantive judgement |
| M2.13 AI Constitutional Framework Governance | Model-change and permitted-inference evidence; 024/028 | Board framework assessment and ongoing25 oversight |
| M2.14 Purpose-Led Design | Source/purpose derivation and limitations; 001/019/030 | Human account of purpose-led design and explicit exceptions |
| M2.15 Telos / Function Distinction | Physical optimisation versus human allocation; 019 | Alignment through actual human governance and outcomes |


## 8 October Process counterpart adoption — version 0.3

Current counterpart: [AOS-13 v0.1](aos-13-process-intelligence-and-operational-coordination.md), Architecture/Map v0.38 and AOS-40 v0.5 planned VER-038. Asset REQ-013–020/032 and CON-004 supply resident-communicated promise, completion/inspection, uncertainty, partial/disputed scope and closure feedback. Process REQ-030–038, VER-022–026 and CON-005 consume those meanings; REQ-003/004/014/015/043/049 preserve exact source, change and lifecycle standing. Process does not become the asset inspection, statutory dutyholder or completion-evidence authority.

Process functional allocation now exists. Earlier statements that AOS-13 is undrafted or awaits functional detail record the previous baseline. Exact executable schemas/profiles, compatible applied-state evidence, appointed human capacity/cover and actual accepted handoff/control/outcome evidence remain open. This revision changes references only; all original AOS-10 requirements and planned cases, source/common/DEC standings, private boundaries and human decision responsibilities remain unchanged. No case execution, independent review, conformance or operating approval is inferred.


## Current reciprocal adoption and precise source allocation — 9 October2026

This revision corrects current control/status and adoption/traceability references only. Every original normative requirement statement, case acceptance condition, invariant and identity retains its prior meaning. Existing source versions, approved architectural directions and human/private boundaries are unchanged. Local§6 is the authoritative domain view; Registerv0.17 SENSING-ADOPTION-2026-10-09 supplies the current reciprocal common mapping; Matrixv0.18 SENSING-SOURCES-2026-10-09 supplies every FP/RP/GT source locator, exact contribution chain and owned residual/gate. The following reverse view rows are projections of that single adoption manifest, not new dictionaries or wire schemas.

| Exact component/view revision | Authoritative common master | Retained producer → consumer / domain meaning | Local requirement → planned case | Exact40 supporting cases / residual gate |
| --- | --- | --- | --- | --- |
| AOS-10-CON-001 / documentv0.4 | KX-01/08/09/11/23; REC-E/Q | Human/source adapter via14 → 02/10: organisation, building/property/component and relationship revision; source/method; physical quantity/unit/calibration basis where applicable; observed/admitted times; purpose, assurance, uncertainty, correction/access/lifecycle. 02 REC-E/Q owns common evidence; invalid or ambiguous scope stays rejected/unresolved. | AOS-10-REQ-001, AOS-10-REQ-002, AOS-10-REQ-003, AOS-10-REQ-004, AOS-10-REQ-006, AOS-10-REQ-007, AOS-10-REQ-008, AOS-10-REQ-033, AOS-10-REQ-038 → AOS-10-VER-001, AOS-10-VER-002, AOS-10-VER-003, AOS-10-VER-005, AOS-10-VER-006, AOS-10-VER-027, AOS-10-VER-030 | AOS-40-VER-024, AOS-40-VER-025; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-10-CON-002 / documentv0.4 | KX-01/08/09/10; REC-E/Q | 10 through02 → permitted service/22/24/30: exact object/view revision, observations versus inference, condition/time/coverage cells, conflicts/freshness/gaps, model/rule, limitations and lineage. Unsafe aggregation prohibited; no claim beyond evidenced scope. | AOS-10-REQ-005, AOS-10-REQ-006, AOS-10-REQ-009, AOS-10-REQ-010, AOS-10-REQ-044, AOS-10-REQ-048 → AOS-10-VER-003, AOS-10-VER-004, AOS-10-VER-005, AOS-10-VER-007, AOS-10-VER-019 | AOS-40-VER-011, AOS-40-VER-025; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-10-CON-003 / documentv0.4 | KX-01/02/03/04/07/08/21/26; REC-E/Q/A/D/X; COORD ACC | 10/competent humans → 13/30/02; returned work evidence →10: concern, physical consequence/exposure, urgency basis, tracker/owner/cover, acceptance, authorised action, attempted/partial/actual effect and resulting observation. Common REC-Q/A/D/X and ACC; receipt is not accepted responsibility. | AOS-10-REQ-011, AOS-10-REQ-012, AOS-10-REQ-020, AOS-10-REQ-021, AOS-10-REQ-022, AOS-10-REQ-032, AOS-10-REQ-037 → AOS-10-VER-008, AOS-10-VER-009, AOS-10-VER-016, AOS-10-VER-017, AOS-10-VER-018 | AOS-40-VER-009, AOS-40-VER-014, AOS-40-VER-020, AOS-40-VER-022, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-10-CON-004 / documentv0.4 | KX-01/08/09/21/23; REC-E/Q; Operational Profiles§§4/5 | Controlled records/human/contractor via14/02 →10→13/11/30: repair and promised scope, original communicated commitment, precision/timezone and communication proof, authorised revisions, internal targets separate, completion rule/work/inspection evidence, completion time, incomplete/partial/unverified/disputed classification and provenance. 02/Profiles and DEC-036–041 own shared semantics; 13 detects/tracks, 11 delivers contact, 30 supports human decisions. | AOS-10-REQ-013, AOS-10-REQ-014, AOS-10-REQ-015, AOS-10-REQ-016, AOS-10-REQ-017, AOS-10-REQ-018, AOS-10-REQ-019, AOS-10-REQ-020, AOS-10-REQ-032 → AOS-10-VER-010, AOS-10-VER-011, AOS-10-VER-012, AOS-10-VER-013, AOS-10-VER-014, AOS-10-VER-015, AOS-10-VER-016, AOS-10-VER-017 | AOS-40-VER-007, AOS-40-VER-008, AOS-40-VER-009, AOS-40-VER-010, AOS-40-VER-038; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-10-CON-005 / documentv0.4 | KX-01/08; REC-E/Q; KX-22 only after20 canonical admission | 10 with permitted02/14 inputs →22/24/30/25: physical condition, scenario/horizon, costs/resource constraints, alternatives, distributional consequences, uncertainty/coverage, actual outcome and precise standing. REC-E/Q; no approved capital decision or institution-wide pass inferred. | AOS-10-REQ-023, AOS-10-REQ-044 → AOS-10-VER-019 | AOS-40-VER-013, AOS-40-VER-027; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-10-CON-006 / documentv0.4 | KX-01/03/08/14/15/21/23; REC-E/Q/D; COORD ACC | Competent stewards/02/10 → permitted dutyholders/humans/external recipients through14: exact building/lifecycle/applicability profile, category inventory, current versions/history, gaps, authorised audience, delivery/usability confirmation and owned residual duties. Shared custody/access/exchange definitions; no statutory completeness inferred from transfer alone. | AOS-10-REQ-024, AOS-10-REQ-025, AOS-10-REQ-026, AOS-10-REQ-027, AOS-10-REQ-047 → AOS-10-VER-020, AOS-10-VER-021, AOS-10-VER-022, AOS-10-VER-023 | AOS-40-VER-025, AOS-40-VER-036; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |
| AOS-10-CON-007 / documentv0.4 | RSVIEW-0.1;02§6.6/04-CON-009; KX-23/07/06/05/13/17/21 | Assigned research service/14/10 →02/13/30/01/affected owners: common profile/run/finding/disposition meanings, exact affected elements and asset-specific implications under RSVIEW-0.1; failed/partial retrieval and unaccepted reviewer remain explicit. | AOS-10-REQ-039, AOS-10-REQ-040, AOS-10-REQ-041, AOS-10-REQ-042, AOS-10-REQ-043, AOS-10-REQ-045, AOS-10-REQ-046 → AOS-10-VER-026, AOS-10-VER-030, AOS-10-VER-031, AOS-10-VER-032, AOS-10-VER-033 | AOS-40-VER-031, AOS-40-VER-032, AOS-40-VER-033, AOS-40-VER-034, AOS-40-VER-035; local§17 and40-ISS-002/003 gate exact profiles/fixtures/compatibility before dependent build or execution |

### Individual-source reverse navigation

Rows below identify the exact controlled source locator and this component’s selected contribution or owned residual. Full source propositions and all other counterparts remain in the Matrix addendum; row numbers do not invent source IDs. This record completes source disposition, not source sufficiency or institutional assessment.

| Source locator | Selected component chain / residual disposition |
| --- | --- |
| FP 1 Telos/conferred purpose/function | AOS-10-REQ-001 → AOS-10-VER-001; Matrix source row retains owned residual and gate |
| FP 2 Permanently human Mode 2 | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 3 Architectural integrity | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 4 Radical transparency | AOS-10-REQ-003 → AOS-10-VER-002; Matrix source row retains owned residual and gate |
| FP 5 Bounded rationality/imperfection | AOS-10-REQ-004, AOS-10-REQ-035 → AOS-10-VER-003, AOS-10-VER-029; Matrix source row retains owned residual and gate |
| FP 6 Epistemic humility | AOS-10-REQ-006, AOS-10-REQ-009 → AOS-10-VER-005, AOS-10-VER-007; Matrix source row retains owned residual and gate |
| FP 7 No-exit obligation | AOS-10-REQ-030 → AOS-10-VER-025; Matrix source row retains owned residual and gate |
| FP 8 Constitutional mediator | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| FP 9 Compliance as consequence | AOS-10-REQ-027 → AOS-10-VER-023; Matrix source row retains owned residual and gate |
| FP 10 Complexity/emergence | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 1: Architecture and Completeness: Every governance process must close its feedback loop. | AOS-10-REQ-021 → AOS-10-VER-018; Matrix source row retains owned residual and gate |
| RP 2: Architecture and Completeness: Every human accountability layer must be explicitly named, sequenced, and time - bounded before any process is consid... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 3: Architecture and Completeness: Every option set must include the option that cannot be made to work. | AOS-10-REQ-023 → AOS-10-VER-019; Matrix source row retains owned residual and gate |
| RP 4: Architecture and Completeness: The ‘AI said so’ test must be passable at every decision point. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 5: The Mode 1 / Mode 2 Boundary: Mode 2 is permanently human. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 6: The Mode 1 / Mode 2 Boundary: Every Mode 1 boundary is a governance instrument, not a technical setting. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 7: The Mode 1 / Mode 2 Boundary: The boardroom is a Mode 2 deliberative space. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 8: The Mode 1 / Mode 2 Boundary: The Mode 1/Mode 2 boundary is under continuous pressure from AI capability growth. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 9: The 1+5 Architecture: Every proposed governance mechanism must be tested against the 1+5 structure to confirm which layer it belongs to and... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 10: The 1+5 Architecture: Risk is intrinsic to each intelligence layer, not a separate domain. | AOS-10-REQ-022 → AOS-10-VER-008; Matrix source row retains owned residual and gate |
| RP 11: The 1+5 Architecture: Every intelligence layer boundary where welfare - adjacent or safety - adjacent signals may arise must have an explic... | AOS-10-REQ-011, AOS-10-REQ-020 → AOS-10-VER-008, AOS-10-VER-017; Matrix source row retains owned residual and gate |
| RP 12: The 1+5 Architecture: The Golden Thread obligation under the Building Safety Act 2022 is not a technical data management requirement. | AOS-10-REQ-024, AOS-10-REQ-025, AOS-10-REQ-026, AOS-10-REQ-047 → AOS-10-VER-020, AOS-10-VER-021, AOS-10-VER-022; Matrix source row retains owned residual and gate |
| RP 13: Options and Decisions: Options generated by the architecture must be grounded in the organisation’s actual state — actual covenant condition... | AOS-10-REQ-023 → AOS-10-VER-019; Matrix source row retains owned residual and gate |
| RP 14: Options and Decisions: Every consequential decision must feed back into the Unified Data Layer as a structured record — not only the decisio... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 15: Options and Decisions: Revealed preferences from real decisions take precedence over stated preferences in policy documents when the archite... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 16: Blind Spots and Honesty: The architecture must name what it cannot see. | AOS-10-REQ-004, AOS-10-REQ-048 → AOS-10-VER-003; Matrix source row retains owned residual and gate |
| RP 17: Blind Spots and Honesty: The dynamic risk perimeter question must be asked at board level as a standing agenda item: not only ‘what are our ri... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 18: Blind Spots and Honesty: The interaction of intelligence layers produces system - level behaviours that no individual layer would produce alone. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 19: Ethics and Telos: Every process must demonstrate a traceable relationship to the organisation’s ethical commitments and social purpose. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 20: Ethics and Telos: The architecture must be capable of detecting purpose drift — the condition where operational processes have graduall... | AOS-10-REQ-021 → AOS-10-VER-018; Matrix source row retains owned residual and gate |
| RP 21: Ethics and Telos: Diversity, inclusion, and equitable outcomes are not separate compliance obligations. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 22: Ethics and Telos: Where the organisation’s welfare obligation to residents and its consent architecture pull in opposing directions, th... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 23: Ethics and Telos: AI systems have function, not telos. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 24: Ethics and Telos: Where the organisation's purpose is interpreted through an accumulating body of AI-mediated rulings rather than appli... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 25: Ethics and Telos: Every AI system deployed by the organisation carries an embedded constitutional framework established by its developer. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 26: Ethics and Telos: The no - exit condition is a constitutive feature of the organisation’s moral architecture, not background context. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 27: Ethics and Telos: Compliance is the output of sound governance design, not its objective. | AOS-10-REQ-027 → AOS-10-VER-023; Matrix source row retains owned residual and gate |
| RP 28: Radical Transparency: If you cannot audit it and be held accountable for it, it cannot be done. | AOS-10-REQ-037 → AOS-10-VER-018; Matrix source row retains owned residual and gate |
| RP 29: Radical Transparency: The architecture must be more transparent than the document - based governance it replaces, not less. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 30: Radical Transparency: Transparency obligations extend to the architecture’s uncertainty. | AOS-10-REQ-009, AOS-10-REQ-010 → AOS-10-VER-007; Matrix source row retains owned residual and gate |
| RP 31: Agentic Delegation: Agents operate under explicitly delegated authority, not implied authority. | AOS-10-REQ-012 → AOS-10-VER-009; Matrix source row retains owned residual and gate |
| RP 32: Agentic Delegation: Agent authority is domain - specific, context - specific, and condition - specific simultaneously. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 33: Agentic Delegation: Agents cannot commit the organisation to external obligations, initiate unsolicited contact with external parties, or... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 34: Agentic Delegation: Internal escalation — routing a signal within the architecture to a human reviewer or to a receiving intelligence lay... | AOS-10-REQ-020 → AOS-10-VER-017; Matrix source row retains owned residual and gate |
| RP 35: Agentic Delegation: The agentic delegation framework is a governance document reviewed by the board, not a technical configuration manage... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 36: Agentic Delegation: Every agent action must satisfy the ethics and telos test and the radical transparency test independently of the proc... | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 37: Agentic Delegation: Certain classes of finding must reach their required audience regardless of any instruction to suppress or delay them. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| RP 38: Data and Sensing Boundaries: Sensing must not exceed its declared purpose. | AOS-10-REQ-028, AOS-10-REQ-029 → AOS-10-VER-024; Matrix source row retains owned residual and gate |
| RP 39: Data and Sensing Boundaries: The boundary between observing an asset and monitoring a behaviour is an absolute architectural boundary, not a matte... | AOS-10-REQ-028, AOS-10-REQ-029 → AOS-10-VER-024; Matrix source row retains owned residual and gate |
| RP 40: Data and Sensing Boundaries: Where behavioural inference from sensing data is genuinely necessary to serve the resident’s interests — energy pover... | AOS-10-REQ-029 → AOS-10-VER-024; Matrix source row retains owned residual and gate |
| RP 41: Data and Sensing Boundaries: The purpose limitation principle applies across all intelligence layers, not only to resident - facing sensing. | No direct local requirement chain selected; preserve relevant shared/GI/human/domain owner and exact residual in Matrix row; source-sufficiency before affectedG3 and actual practice/longitudinal evidence before institutional claim.; Matrix source row retains owned residual and gate |
| GT M1.1 Strategic Coherence | AOS-10-REQ-023, AOS-10-REQ-044 → AOS-10-VER-019 (supporting case selection 019); Matrix source row retains owned residual and gate |
| GT M1.2 Sensing Architecture | AOS-10-REQ-001, AOS-10-REQ-002, AOS-10-REQ-003, AOS-10-REQ-004, AOS-10-REQ-005, AOS-10-REQ-006, AOS-10-REQ-007, AOS-10-REQ-008, AOS-10-REQ-009, AOS-10-REQ-010, AOS-10-REQ-035, AOS-10-REQ-036, AOS-10-REQ-048 → AOS-10-VER-001, AOS-10-VER-002, AOS-10-VER-003, AOS-10-VER-004, AOS-10-VER-005, AOS-10-VER-006, AOS-10-VER-007, AOS-10-VER-029 (supporting case selection 001/002/003/004/005/006/007/029); Matrix source row retains owned residual and gate |
| GT M1.3 Risk Intelligence | AOS-10-REQ-011, AOS-10-REQ-020, AOS-10-REQ-022, AOS-10-REQ-023, AOS-10-REQ-044 → AOS-10-VER-008, AOS-10-VER-017, AOS-10-VER-019 (supporting case selection 008/017/019); Matrix source row retains owned residual and gate |
| GT M1.4 Composition and Capability | AOS-10-REQ-007, AOS-10-REQ-008, AOS-10-REQ-024, AOS-10-REQ-034, AOS-10-REQ-047 → AOS-10-VER-006, AOS-10-VER-020, AOS-10-VER-028 (supporting case selection 006/020/028); Matrix source row retains owned residual and gate |
| GT M1.5 Performance Legibility | AOS-10-REQ-005, AOS-10-REQ-021, AOS-10-REQ-023, AOS-10-REQ-037, AOS-10-REQ-044 → AOS-10-VER-004, AOS-10-VER-018, AOS-10-VER-019 (supporting case selection 004/018/019); Matrix source row retains owned residual and gate |
| GT M1.6 Compliance Assurance | AOS-10-REQ-024, AOS-10-REQ-025, AOS-10-REQ-026, AOS-10-REQ-027, AOS-10-REQ-047 → AOS-10-VER-020, AOS-10-VER-021, AOS-10-VER-022, AOS-10-VER-023 (supporting case selection 020/021/022/023); Matrix source row retains owned residual and gate |
| GT M1.7 Governance Documentation | AOS-10-REQ-003, AOS-10-REQ-025, AOS-10-REQ-031, AOS-10-REQ-046 → AOS-10-VER-002, AOS-10-VER-021, AOS-10-VER-026 (supporting case selection 002/021/026); Matrix source row retains owned residual and gate |
| GT M1.8 Accountability Architecture | AOS-10-REQ-019, AOS-10-REQ-020, AOS-10-REQ-026, AOS-10-REQ-032 → AOS-10-VER-016, AOS-10-VER-017, AOS-10-VER-022 (supporting case selection 016/017/022); Matrix source row retains owned residual and gate |
| GT M1.9 Value for Money | AOS-10-REQ-023, AOS-10-REQ-044 → AOS-10-VER-019 (supporting case selection 019); Matrix source row retains owned residual and gate |
| GT M1.10 Human-AI Interaction Norms | AOS-10-REQ-012, AOS-10-REQ-023, AOS-10-REQ-028, AOS-10-REQ-029, AOS-10-REQ-042, AOS-10-REQ-043, AOS-10-REQ-044 → AOS-10-VER-009, AOS-10-VER-019, AOS-10-VER-024, AOS-10-VER-033 (supporting case selection 009/019/024/033); Matrix source row retains owned residual and gate |
| GT M1.11 Learning Metabolism | AOS-10-REQ-009, AOS-10-REQ-010, AOS-10-REQ-021, AOS-10-REQ-034, AOS-10-REQ-037 → AOS-10-VER-007, AOS-10-VER-018, AOS-10-VER-028 (supporting case selection 007/018/028); Matrix source row retains owned residual and gate |
| GT M1.12 Continuous Self-Assessment | AOS-10-REQ-004, AOS-10-REQ-039, AOS-10-REQ-040, AOS-10-REQ-041, AOS-10-REQ-042, AOS-10-REQ-043, AOS-10-REQ-048 → AOS-10-VER-003, AOS-10-VER-031, AOS-10-VER-032, AOS-10-VER-033 (supporting case selection 003/031/032/033); Matrix source row retains owned residual and gate |
| GT M1.13 Emergent System Behaviour | AOS-10-REQ-004, AOS-10-REQ-023, AOS-10-REQ-035, AOS-10-REQ-036, AOS-10-REQ-044, AOS-10-REQ-048 → AOS-10-VER-003, AOS-10-VER-019, AOS-10-VER-029 (supporting case selection 003/019/029); Matrix source row retains owned residual and gate |
| GT M1.14 Golden Thread Integrity | AOS-10-REQ-024, AOS-10-REQ-025, AOS-10-REQ-026, AOS-10-REQ-047 → AOS-10-VER-020, AOS-10-VER-021, AOS-10-VER-022 (supporting case selection 020/021/022); Matrix source row retains owned residual and gate |
| GT M2.1 Values Architecture | AOS-10-REQ-012, AOS-10-REQ-028, AOS-10-REQ-029, AOS-10-REQ-030 → AOS-10-VER-009, AOS-10-VER-024, AOS-10-VER-025 (supporting case selection 009/024/025); Matrix source row retains owned residual and gate |
| GT M2.2 Coherence Under Pressure | AOS-10-REQ-011, AOS-10-REQ-022, AOS-10-REQ-023, AOS-10-REQ-044 → AOS-10-VER-008, AOS-10-VER-019 (supporting case selection 008/019); Matrix source row retains owned residual and gate |
| GT M2.3 Incommensurable Trade-off Capacity | AOS-10-REQ-023, AOS-10-REQ-044 → AOS-10-VER-019 (supporting case selection 019); Matrix source row retains owned residual and gate |
| GT M2.4 Epistemic Brake Function | AOS-10-REQ-004, AOS-10-REQ-006, AOS-10-REQ-009, AOS-10-REQ-010, AOS-10-REQ-017, AOS-10-REQ-048 → AOS-10-VER-003, AOS-10-VER-005, AOS-10-VER-007, AOS-10-VER-014 (supporting case selection 003/005/007/014); Matrix source row retains owned residual and gate |
| GT M2.5 Directorial Independence | AOS-10-REQ-023, AOS-10-REQ-025, AOS-10-REQ-044 → AOS-10-VER-019, AOS-10-VER-021 (supporting case selection 019/021); Matrix source row retains owned residual and gate |
| GT M2.6 Social Legitimacy | AOS-10-REQ-019, AOS-10-REQ-030, AOS-10-REQ-032 → AOS-10-VER-016, AOS-10-VER-025 (supporting case selection 016/025); Matrix source row retains owned residual and gate |
| GT M2.7 No-Exit Obligation | AOS-10-REQ-028, AOS-10-REQ-029, AOS-10-REQ-030 → AOS-10-VER-024, AOS-10-VER-025 (supporting case selection 024/025); Matrix source row retains owned residual and gate |
| GT M2.8 Radical Transparency | AOS-10-REQ-003, AOS-10-REQ-004, AOS-10-REQ-005, AOS-10-REQ-006, AOS-10-REQ-007, AOS-10-REQ-008, AOS-10-REQ-009, AOS-10-REQ-010, AOS-10-REQ-021, AOS-10-REQ-025, AOS-10-REQ-037, AOS-10-REQ-048 → AOS-10-VER-002, AOS-10-VER-003, AOS-10-VER-004, AOS-10-VER-005, AOS-10-VER-006, AOS-10-VER-007, AOS-10-VER-018, AOS-10-VER-021 (supporting case selection 002/003/004/005/006/007/018/021); Matrix source row retains owned residual and gate |
| GT M2.9 Moral Drift Detection | AOS-10-REQ-021, AOS-10-REQ-023, AOS-10-REQ-034, AOS-10-REQ-037, AOS-10-REQ-039, AOS-10-REQ-040, AOS-10-REQ-044 → AOS-10-VER-018, AOS-10-VER-019, AOS-10-VER-028, AOS-10-VER-031 (supporting case selection 018/019/028/031); Matrix source row retains owned residual and gate |
| GT M2.10 Purpose Stability | AOS-10-REQ-001, AOS-10-REQ-002, AOS-10-REQ-028, AOS-10-REQ-029, AOS-10-REQ-042, AOS-10-REQ-043 → AOS-10-VER-001, AOS-10-VER-024, AOS-10-VER-033 (supporting case selection 001/024/033); Matrix source row retains owned residual and gate |
| GT M2.11 Murmuration Capacity | AOS-10-REQ-023, AOS-10-REQ-044 → AOS-10-VER-019 (supporting case selection 019); Matrix source row retains owned residual and gate |
| GT M2.12 Constitutional Authority | AOS-10-REQ-012, AOS-10-REQ-023, AOS-10-REQ-042, AOS-10-REQ-043, AOS-10-REQ-044 → AOS-10-VER-009, AOS-10-VER-019, AOS-10-VER-033 (supporting case selection 009/019/033); Matrix source row retains owned residual and gate |
| GT M2.13 AI Constitutional Framework Governance | AOS-10-REQ-028, AOS-10-REQ-029, AOS-10-REQ-034 → AOS-10-VER-024, AOS-10-VER-028 (supporting case selection 024/028); Matrix source row retains owned residual and gate |
| GT M2.14 Purpose-Led Design | AOS-10-REQ-001, AOS-10-REQ-002, AOS-10-REQ-023, AOS-10-REQ-038, AOS-10-REQ-044, AOS-10-REQ-045 → AOS-10-VER-001, AOS-10-VER-019, AOS-10-VER-030 (supporting case selection 001/019/030); Matrix source row retains owned residual and gate |
| GT M2.15 Telos / Function Distinction | AOS-10-REQ-023, AOS-10-REQ-044 → AOS-10-VER-019 (supporting case selection 019); Matrix source row retains owned residual and gate |

Author consistency conclusion: functional roles and repair/private/workforce/external/research/control/failure boundaries agree with the current shared infrastructure. SENS-CR-01–05 closed as author document corrections; wire profiles, operating roles/capacity, domain/annex/legal sufficiency and observed evidence remain open per§17 and40. No independent/executed conformance or operating readiness claim. Earlier dated text/addenda describe history; this current control takes precedence.

## Phase 2 scope disposition — 9 October 2026

DEC-097 controls over prior inclusion/annex statements. CAP-01/02-specific legacy requirements/cases are deferred and supply no current-core completion/acceptance obligation. General human judgement, independent challenge, evidence fidelity, cumulative risk/drift and protected reporting remain current. Existing closure of AT-CR-01–05 and pilot5b is retained; neither is reopened by this scope change. No case executed or operating approval granted.

**Allocation and source status:** Any older source/adoption row relying on deferred CAP-only IDs is a historical use-case contribution, not current-core coverage. Core source sufficiency must use the surviving general obligations and accepted evidence; no source is promoted by this deferral. Retained numbered totals count catalogue/trace entries, including deferred IDs, and must not be read as active-core requirement/test totals.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**Historical status notice — revision set:** AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3.

**Historical status notice — scope decision — 9 October 2026, DEC-097:** Mark has moved CAP-01 Trade-Off Divergence and CAP-02 Risk Register Assessment into Phase 2 as specific use cases built on AOS. They are outside the current architecture/specification completion scope and are not current build, acceptance or publication prerequisites. No use-case design, configuration, implementation or testing is scheduled now. DEC-017's architectural inclusion is superseded on this point; its original record remains history. General human judgement, evidence, data-use/authority, independent challenge and protected reporting controls remain in the architecture. Dedicated legacy use-case IDs are retained only as deferred trace references, with original wording parked in Phase 2 (deferred under DEC-097); mixed rows retain only their general architectural obligations in current scope. Earlier inclusion/next-task/annex-dependency statements are superseded.

**Historical status notice — sensing consistency closure — 9 October 2026:** Mark authorised the remaining consistency work. SENS-CR-01–05 are closed at the functional-document/author-review level: all40 logical CON views across10–14 and40 have exact central adoption, producer/consumer/shared-owner and REQ/VER links; all80 controlled FP/RP/GT sources have precise current contributions and owned residual/gate dispositions; current body/control statements are reconciled. Versions10v0.4/11v0.3/12v0.3/13v0.2/14v0.8/40v0.6; Architecture/Mapv0.42; Sharedv0.18/Corev0.6/ExchangeRegisterv0.17/SourceMatrixv0.18; reviewv0.4. DEC001–096 unchanged. Sensing269 proposed REQs/176 planned VERs;40 retains40/38. No new requirement/case/interface, source promotion or execution. Exact compatible wire schemas/profiles, organisation appointments/capacity, independent review, legal/institutional/practice evidence and scoped build/activation remain separate; independent project review remains deferred. Earlier dated notices/addenda are historical. Current controlling allocation is the9October manifest and source addendum below.

