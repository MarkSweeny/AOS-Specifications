# AOS-25 — Governance oversight, drift and learning

Document: aos-25-governance-oversight-drift-and-learning · Source revision or record: v0.5

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**DEC-104 adopted — 29 October 2026:** Current revision 0.5. Each mandatory protected-finding category requires assessed technical-failure and implicated-person interference arrangements with an appropriately independent authorised alternative and no implicated sole release gatekeeper. [Decision/amendment record](../Supporting-Specifications/aos-dec-104-protected-reporting-and-implicated-recipients-2026-10-29.md). External reporting is conditional on justified lawful authority, not a default. Exact profiles/permissions, protected_finding v0.3 compatibility and actual evidence remain gates; amended wording retains ordinary separate review and cases are planned/unexecuted. Earlier contrary or narrower baselines are history for this scope.

**DEC-103 adopted — 29 October 2026:** Current revision 0.4. Decision validity/effective time, attributable evidence/authentication, minutes approval and permission to execute are separate. DEC-087 is partly superseded; [decision/amendment and legal-source record](../Supporting-Specifications/aos-dec-103-decision-validity-evidence-and-minutes-2026-10-29.md). No universal later-minutes or second decision-record approval gate. Exact instruments/evidence policy, KX-06 v0.3 compatibility and ordinary separate review/readiness gates remain required; cases unexecuted. Earlier contrary wording is historical only where explicitly identified.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

| Document control | Value |
| --- | --- |
| Component / version / date | AOS-25 / 0.5 / 29 October 2026 |
| Status | Functional specification review draft; proposed requirement wording |
| Architecture baseline consulted | AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3. |
| Governing sources | Foundational Principles v4; AOS Reasoning Principles v6; Governance Intelligence Tests; preserved source manifest |
| Dependencies consulted | AOS-01–05 v0.8; AOS-14 v0.4; AOS-20 v0.3; AOS-21 v0.4; AOS-22 v0.2; AOS-23 v0.3; AOS-24 v0.1; AOS-30 v0.3; Shared v0.13/Core v0.6/Register v0.12; source matrix v0.13; Control Coordination v0.2; Protected Reporting and Recovery v0.1 |
| Allocation supplements | AOS-00/Map v0.31; Shared v0.14/Register v0.13/source matrix v0.14; 20 v0.4/21 v0.5/22 v0.3/23 v0.4/24 v0.2/30 v0.4 counterpart-reference alignment only; common meanings unchanged |
| Quality / template | AOS-QS v0.1; component template v0.4 |
| Project owner / custodian | Mark Sweeny |
| Operational owner | Accountable GI oversight owner; independent human reviewer, empowered committee/board, corrective-duty and cover roles require organisation appointment |
| Author / reviewers | Codex at Mark's request; author document checks only; Mark wording/whole-document review pending; independent project reviewer unassigned/deferred |
| Approval / readiness | Existing design directions apply; no whole-document, build, activation or achieved readiness approval |
| Change history | 0.2 — GI-CR-01–04 author consistency correction/closure under Mark’s instruction; existing identifiers and proposed/planned status preserved. 0.1 initial functional draft; no new DEC, IF, schema, deployment or schedule |

## 1. Purpose and scope

AOS-25 examines whether the organisation and its AI-mediated governance remain coherent with conferred purpose over time. It connects individually plausible assessments, decisions, exceptions and outcomes into an account of accumulated drift, blind spots and learning. Without it, each paper can pass review while precedents progressively relocate founding meaning, burdens repeatedly fall on the same people, or the system optimises successfully for the wrong thing.

It owns GI oversight analysis: purpose/precedent and Mode 1/Mode 2 boundary drift, override patterns, cumulative distribution of trade-offs, developer-framework divergence, cross-component effects, evidence blind spots, ordinary agent performance inputs, independent review support, response tracking and research into its own adequacy. It coordinates oversight of the GI research portfolio while specialist components retain their own remits. It does not become a new intelligence, an all-powerful controller, an independent human reviewer or a governance certificate.

AOS-21 owns corpus and approved precedent; 22 owns synthesis/interpretation/options; 23 owns artefact assessment and currency monitoring; 24 renders canonical positions; 30 records empowered human decisions, approval, duties and outcomes. AOS-01–05 own powers, records, use, agents and runtime; 13 coordinates operations; 14 governs external exchange; 40 will organise assurance/test evidence. AOS-25 can identify patterns and propose review, not change telos, amend governing meaning, auto-prune precedent, rank incommensurable goods, infer personal feelings/preferences or activate exploratory self-calibration.

Stakeholders include boards/committees, independent directors/reviewers, executives, residents, staff, governance/corpus stewards, domain/agent owners and operators. Their legitimate interests, especially the no-exit condition, inform purposeful evidence and explanation. Parent/subsidiary profiles, powers and applicability remain distinct under DEC-090. Permitted group analysis is possible; common membership is not permission to combine data or copy constitutional authority.

## 2. Authority and sources

FP v4/RP v6 govern; recorded directions constrain proposed wording. Working sources are reconciled, not adopted wholesale. Requirement source keys below identify their exact baseline and functional locators. The source manifest remains unchanged.

| Key | Exact source / locator and standing |
| --- | --- |
| FP / RP | Foundational_Principles_v4.docx principles 1–10; AOS_Reasoning_Principles_v6.docx domains 1–9, especially RP2 standing review, RP4 decision feedback, RP5 emergent behaviour and RP6 purpose/precedent/developer-framework paragraphs |
| GT | Governance_Intelligence_Tests.docx all M1.1–14/M2.1–15; §8 technical contributions and permanent human limits |
| WP | Governance Intelligence: Internal Architecture — Working Paper, How the corpus holds meaning, Governance of drift — annual report, Cross-cutting drift self-flagging, Validation regime and Charter; originally RP v5, reconciled to v6/DEC-079–085 |
| TD | Trade-Off Divergence Tool — Product Specification (Working Draft).md §3 Stage Three, §§4–6 independent configuration, decision mapping and charter prohibition; adopted scope DEC-017, routing constrained by DEC-085 |
| CMP | GIL v2 comparison filename v0.1/content v0.2, GIL-C03/04/10/19/22/24/25/27/32/34; retained/changed/retired/deferred standing remains |
| GI / S / AS / H | AOS-20 v0.3 §§3–7/10–17, especially REQ-034–046; AOS-22 v0.2 §§3–7/10/19; AOS-23 v0.3 §§3–7/10/19; AOS-30 v0.3 §§5–7/9–12 |
| C / P | AOS-21 v0.4 §§3–7/10/19 corpus/precedent; AOS-24 v0.1 §§3–7/10/19 faithful presentation and correction |
| SC / REC / KX | Shared v0.13 §4.4; Core v0.6 REC-E/Q/A/D/X; Register v0.12 KX-01/06 v0.2/08/13/15–22/26; common meanings stay authoritative |
| D / R | AOS-00 v0.30 DEC-001–091; DEC-086/template v0.4 §4.4; AOS-04 v0.8 §§3.1/5.1/6.6/10.8 CON-009, AOS-02 v0.8 §6.6 CON-007, AOS-01 v0.8 §§6.6/10.8; RSVIEW-0.1 |

WP's conversational ratification-to-precedent assumption is superseded by DEC-080/081: confirmation is not empowered adoption. Its historical 2015 standard reference supplies no claim about current regulatory clauses. Dual authorship is implemented as independently prepared human and GI accounts; a particular committee name, special-resolution mechanism or appointment cannot be invented for every organisation. Actual governing instruments supply powers. TD decision mapping remains mixed/uncertain where appropriate and human-confirmed under DEC-088; neither a persona count nor an oversight finding establishes moral error. No new external legal/standard currentness claim is introduced.

### DEC-104 — protected reporting under failure and implicated-person interference

Each mandatory protected-finding category shall have an approved reporting arrangement assessed against both technical failure and interference by implicated people. The profile shall identify the intended recipient, possible conflicts and an appropriately independent authorised alternative; an implicated person shall not be the sole gatekeeper deciding whether the required finding reaches its authorised audience.

Authority/use permissions, minimum report content, recipient verification, custody, route/change dependencies, tracking ownership, acceptance, cover and escalation are established in advance. An external route is included where justified and lawfully authorised; external reporting is not a universal default and a finding creates no extra disclosure power. Planned exercises address failed infrastructure, unavailable/implicated recipients, apparent alternatives controlled by the same implicated gatekeeper and attempted suppression. Missing adequate arrangements remain an explicit owned gap, prevent claims of operational protected-reporting assurance and withhold affected dependent reliance under existing gates; they do not create false delivery, ownership transfer or blanket shutdown of separately authorised service. Original tracking duty persists until actual scoped acceptance.

The organisation’s profile binds each required finding class to normal/alternate authorised audiences, conflict criteria/evidence and accountable assessment, disclosure basis/minimal payload, independently verifiable recipients/permissions, credentials/custody and route/reconfiguration controls, failure/compromise assumptions, tracking/cover/escalation, human fallback, evidence and review triggers. Test both infrastructure/common-dependency independence and organisational release/recipient/custody control; neither implies the other. No administrator, executive sign-off or report-validation step may silently remove a required duty. The declared threat/governance scope and residual limitations must be visible: this is not an unlimited guarantee against every holder of legal/constitutional change powers. Inadequacy returns to an empowered accountable reviewer; the reporting agent cannot invent a recipient or grant itself onward-disclosure authority.

## 3. Responsibilities

| Responsibility | AOS-25 owns | Reserved / shared owner |
| --- | --- | --- |
| Longitudinal oversight | Evidence-qualified purpose, precedent, boundary, override and distributional patterns | 21 maintains meaning/history; 01/30 humans amend/adjudicate |
| System effects | Cross-component blind spots, model-framework divergence and cumulative effects | Domains supply evidence; 04/05 evaluation/runtime; 40 assurance scope |
| Independent review support | GI account, permitted evidence basis, differences and tracked responses | Independent human authors prepare their own account; empowered institution determines disposition |
| Learning | Actual consequence links, misunderstanding/corrections and effectiveness questions | 30 duty/decision records; 22 analytical revisions; no automatic calibration |
| GI research oversight | Portfolio coverage, shared omissions, unresolved findings and response quality | 20–24/25 specialist remits; 14 retrieval; 04 shared agent infrastructure |
| Own research | Specialist external relevance and adaptation proposals for oversight | 01/30 human change; no autonomous amendment |

Logical flow: scoped permitted histories/current instruments → GI oversight account and separately prepared human account → empowered comparison/disposition → accepted corrective duties → evidenced consequences/reassessment. Both reports remain distinct and can disagree. This mandates functional independence and accountability, not a second model, dedicated deployment or unrestricted evidence access.

## 4. Capabilities, functions and requirements

### 4.1 Capabilities

| ID | Observable capability / REQs |
| --- | --- |
| AOS-25-CAP-001 | Produce bounded, comparable and contestable oversight evidence; 001–005/019/028/045/048 |
| AOS-25-CAP-002 | Detect possible purpose, precedent, boundary and developer-framework drift; 006–010 |
| AOS-25-CAP-003 | Expose emergent effects, blind spots and cumulative trade-offs; 011–016 |
| AOS-25-CAP-004 | Support actual-outcome learning and independently prepared review with owned dispositions; 017–018/020–027 |
| AOS-25-CAP-005 | Preserve permitted human boundaries, correction, handoff and governed histories; 029–036/046–047 |
| AOS-25-CAP-006 | Conduct own controlled external research and GI research-portfolio oversight; 037–042 |
| AOS-25-CAP-007 | Support ordinary performance monitoring and longitudinal evaluation without self-calibration; 043–044 |

### 4.2 Functions

Each function records exact input/control revisions and uncertainty; failed preconditions yield an owned limitation, not a completed-clear result. Behaviour is functional rather than a wire/API prescription.

| ID | Trigger / input → behaviour → output and failure |
| --- | --- |
| AOS-25-FUN-001 | Approved cycle/material event → scope and check evidence/controls/coverage/comparability → bounded basis or owned gap; 001–004/028/031/045–047 |
| AOS-25-FUN-002 | Scoped instruments/interpretation/precedent/overrides/frameworks → contrast meaning and effects against founding/authorised baseline → possible drift and referral, never amendment; 005–010/019 |
| AOS-25-FUN-003 | Permitted multi-case/cross-component history → examine cumulative effects/distribution/quiet gaps → qualified patterns and telos concern response gaps, no persona winner; 011–016 |
| AOS-25-FUN-004 | Decision/action/outcome records → connect consequences, limits and alternative explanations → learning questions and accountable feedback; 017–018/032 |
| AOS-25-FUN-005 | Annual or material-drift review trigger → GI account, independent human evidence support and report comparison → differences and empowered disposition; 020–023/026/030/048 |
| AOS-25-FUN-006 | Review disposition/protected concern → current powers/use and owned handoff → accepted duties/cover/escalation, selective containment or human referral; 024–029/035–036 |
| AOS-25-FUN-007 | Corrected evidence/control or material oversight method change → affected revision/evaluation/impact checks → reassessment, notification and controlled release; 033–034/043–044 |
| AOS-25-FUN-008 | Approved specialist research trigger → controlled retrieval and assessment → coverage/finding/human disposition or owned degraded recovery; 037–041 |
| AOS-25-FUN-009 | GI research portfolio review trigger → compare remits/coverage/shared gaps and actual responses → owned adequacy questions and proposal, not central takeover; 042 |

### 4.3 Proposed requirements

All rows are **proposed component-level functional requirements**, initial history **0.1**, release scope **functional review only**. Sources distinguish approved directions from their functional derivation; inclusion does not approve exact wording. Accountable owner is the GI oversight owner; Mark is proposed wording approver/custodian. Independent review, disclosure, constitutional/change and human-duty decisions require the separately empowered roles in §§3/7. Common dependencies are 01–05/14/20 and §6; case histories additionally use 21–24/30 and pending 13/40 where applicable. Research rows use §4.4/CON-009. Each row completes the record with source, rationale and primary planned VER in §15; no case is executed.

| ID | Category / proposed obligation | Exact source / derivation | Rationale | Planned VER |
| --- | --- | --- | --- | --- |
| AOS-25-REQ-001 | **Scoped oversight:** Bind each oversight assessment to its exact entity, period, question, source/analysis/control revisions and approved review remit. | GI §§3/6/10; DEC-090; KX-22 | Makes the assessment reproducible. | 001 |
| AOS-25-REQ-002 | **Evidence:** Preserve supporting and conflicting evidence, assurance, provenance, observed/effective dates and evidence-versus-inference distinctions for material findings. | RP5/7; REC-E/Q; DEC-045–048/062–066 | A pattern is contestable evidence, not a verdict. | 001 |
| AOS-25-REQ-003 | **Coverage:** Show the assessed population and material coverage limits, distinguishing justified non-applicability, exclusion, missing/unseeded/unassessed evidence and failed checking. | CMP GIL-C04/19; FP5/6; GT M1.2/12 | A green result must not conceal unseen scope. | 002 |
| AOS-25-REQ-004 | **Comparability:** Qualify comparisons for changed definitions, criteria, entity, period, exposure and population; do not treat incompatible or missing observations as equivalent values. | REQ-001–003 derivation; RP5; REC-E/Q | Trend changes may reflect changed measurement. | 002 |
| AOS-25-REQ-005 | **Two-layer review:** Distinguish compliance evidence from coherence with conferred purpose and values, retaining conflicts rather than treating compliance as proof of coherence. | WP Governance of drift; FP9; RP6 | Technical compliance can coexist with purpose drift. | 003 |
| AOS-25-REQ-006 | **Purpose drift:** Assess evidenced operational outcomes and optimisation behaviour against the exact founding purpose/values and approved changes, identifying possible telos/function substitution. | RP6 purpose drift/telos-function; FP1; GT M2.9/10/15 | Optimisation success may displace purpose. | 004 |
| AOS-25-REQ-007 | **Precedent drift:** Compare accumulated interpretation and approved precedent with the founding statement and authorised changes, not only with the most recent rulings. | RP6 precedent paragraph; DEC-010–012/080/081; WP drift | Individually reasonable rulings can drift cumulatively. | 004 |
| AOS-25-REQ-008 | **Mode boundary:** Review patterns of Mode 1/Mode 2 classification, delegation and boundary changes against their actual empowered instruments; refer ambiguity or bypass without reclassifying reserved human judgement autonomously. | RP2; DEC-005/024/025; GI §§7/10 | Capability cannot silently redraw a governance boundary. | 005 |
| AOS-25-REQ-009 | **Overrides:** Examine override, refusal, exception and reversal patterns with their reasons, powers, scope and actual effects; a frequent or rare override alone is not misconduct or safety evidence. | GI REQ-036; RP2/5/7; KX-06/08/17 | Context distinguishes legitimate judgement from control erosion. | 006 |
| AOS-25-REQ-010 | **Developer divergence:** Review material deployed/proposed model-framework assessments and operational evidence for divergence from organisational values, exposing missing pre-deployment assessment and changed framework scope. | FP3; RP6 developer frameworks; GT M2.13; KX-17/20 | Developer commitments do not become organisational authority by default. | 007 |
| AOS-25-REQ-011 | **Emergence:** Assess permitted cross-component interactions and cumulative effects that individual component evaluations may miss, identifying affected owners and system-level review needs. | RP5 emergent behaviour; FP10; DEC-056/057; GT M1.13 | Assured parts do not establish assured collective behaviour. | 008 |
| AOS-25-REQ-012 | **Quiet-state blind spots:** Treat apparently stable or alarm-free operation as compatible with missing coverage, weak challenge or accumulating risk, retaining appropriate review questions and limitations. | FP5/6; RP5; GT M1.12/13 | No alarm is not proof of sound judgement. | 009 |
| AOS-25-REQ-013 | **Distributional patterns:** Surface evidenced cumulative trade-off burdens and consequences across relevant groups/time, including no-exit impacts, with permitted scope and uncertainty. | FP7/10; RP4/6; TD §3 Stage Three | Per-decision acceptability can conceal repeated burden. | 010 |
| AOS-25-REQ-014 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-25-REQ-014 (deferred under DEC-097); identifier retained for traceability only. | DEC-017; TD §§3/6; GI §§4/7 | Repeated preference is a review signal, not a moral verdict. | 010 |
| AOS-25-REQ-015 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-25-REQ-015 (deferred under DEC-097); identifier retained for traceability only. | DEC-088; TD §5 decision tracking; H §§5/10; S §19 | Real decisions need not have one persona winner. | 011 |
| AOS-25-REQ-016 | **Unacted telos concerns:** Give prominence to evidenced telos-tier concerns raised without an adequate recorded response, distinguishing unresolved, unrecorded, disputed and genuinely dispositioned cases. | TD §3 Stage Three; DEC-083; RP6 | Neglected purpose concerns matter more than persona win counts. | 012 |
| AOS-25-REQ-017 | **Outcome learning:** Connect proposals, human decisions, actions, actual outcomes, unintended consequences and remaining duties, separating action completion from effectiveness. | RP1/4; CMP GIL-C34; H §§10–12 | Learning requires consequence evidence. | 013 |
| AOS-25-REQ-018 | **Causal limits:** Keep alternative explanations, exposure differences, confounders, delays and attribution limits visible in outcome/pattern assessments. | FP5/6/10; RP5; S §§4/10 | Correlation cannot establish institutional motives or causation. | 013 |
| AOS-25-REQ-019 | **Assessment dimensions:** Preserve the distinction between document quality, claim support and practice evidence when combining artefact assessments into oversight findings. | DEC-091; AS §§4/10; CMP GIL-C16 | Good documentation is not demonstrated practice. | 014 |
| AOS-25-REQ-020 | **Self-assessment standing:** Label GI self-assessment as such and retain its method, evidence and limits; it cannot substitute for the independently prepared human account. | WP dual authorship; DEC-010/011; GI REQ-034–036 | The interpreting system cannot independently assure itself. | 015 |
| AOS-25-REQ-021 | **Independent cycle:** Support independently prepared human interpretation/precedent review alongside GI assessment at least annually and on material drift triggers, with each account prepared without reference to the other before formal comparison. | DEC-010/011; RP6 precedent; WP Governance of drift | Independent divergence may reveal what self-flagging missed. | 015 |
| AOS-25-REQ-022 | **Review basis:** Make the authorised evidence basis, founding/changed instruments, scope and limitations available for both reports; identify differing evidence/revisions before comparison without forcing the independent author to adopt GI framing. | DEC-010/011/085; REC-E/Q; WP dual authorship | A fair comparison requires known scope, not identical conclusions. | 016 |
| AOS-25-REQ-023 | **Disposition:** Route the two reports and material differences to the empowered committee/board route for explicit reaffirmation, corrective action/precedent review or constitutional referral under actual powers. | DEC-012/024/025; WP outcomes; H §§5–7 | A report must produce a governed response. | 017 |
| AOS-25-REQ-024 | **Corrective duties:** Track required review/corrective responses with accepted accountable owner, completion date, cover, escalation and exact target/scope. | DEC-012; RP1; KX-26; H §§10–12 | Discussion alone does not close a feedback loop. | 018 |
| AOS-25-REQ-025 | **Closure evidence:** Close a corrective duty only on the required completion/review evidence and record remaining risk and follow-up; a disposition or receipt alone is insufficient. | DEC-012/067–078; KX-21/26; RP1 | Completed action may still need effectiveness review. | 018 |
| AOS-25-REQ-026 | **Reserved amendment:** Refer proposed precedent pruning, boundary or purpose changes to empowered 21/01/30 workflows; only the board changes telos, and no retrospective automatic reversal follows an oversight finding. | DEC-024/025/080/081/089; KX-08/13; H §7 | Oversight detects; authorised governance changes meaning. | 017 |
| AOS-25-REQ-027 | **Protected findings:** Route credible mandatory protected classes promptly through the empowered ordinary/alternate route, without waiting for annual review, executive permission or ordinary report validation. | DEC-083/073–078; GI §10; protected reporting/recovery v0.1 | A review calendar must not suppress an obligation. | 019 |
| AOS-25-REQ-028 | **Provisional status:** Record/access provisional findings within current controls with exact limitations, and distinguish them from formally validated oversight; urgent protected reporting need not await validation. | DEC-084; SC §4.4; CMP GIL-C08 | Preserves timely evidence without invented validation. | 020 |
| AOS-25-REQ-029 | **Selective brake:** Seek or apply only the separately conferred containment powers for materially affected reliance/effects, preserving independently authorised service and protected duties. | DEC-063/067/089; REC-A/D/X; coordination v0.2 | A concern does not authorise unlimited suspension. | 019 |
| AOS-25-REQ-030 | **Protected deliberation:** Use permitted preparation material and authorised human post-meeting accounts while keeping AI out of live protected board/committee deliberation. | DEC-008/087; RP2; H §§1/10 | Independent human observation remains human. | 021 |
| AOS-25-REQ-031 | **Permitted aggregation:** Apply independent data-use permission to the oversight purpose and cross-entity joins/derived views; aggregation or group membership must not imply safety or permission. | DEC-049–053/090; RP9; AOS-03 §§4/9 | Combining records can create an unapproved inference capability. | 021 |
| AOS-25-REQ-032 | **Human preferences:** Use only permitted human-provided/confirmed descriptions; do not infer feelings, personality or moral weights, or silently calibrate norms/precedent from observed choices. | DEC-018/088; RP4 constrained; AOS-03 §9 | Oversight must not turn into covert profiling. | 021 |
| AOS-25-REQ-033 | **Correction impact:** Reassess materially affected oversight on corrected evidence, analysis, approval, permission or criteria and notify dependent owners, including affected AOS-30 preparation/decision/account/outcome workflows. | DEC-062–078/089; KX-13; H §§10–12 | Corrections must reach the humans relying on the pattern. | 022 |
| AOS-25-REQ-034 | **Exact reviewed revision:** Bind validation/disposition to exact reviewed revisions; changed material does not inherit an earlier review or approval. | DEC-028/029/063–066; SC §4.4; KX-06 v0.3 | Reviewed is a scoped state. | 022 |
| AOS-25-REQ-035 | **Handoff states:** Distinguish production, delivery, receipt, validation, application, responsibility acceptance and substantive resolution with purpose-specific evidence and unknown outcomes retained. | KX-21/26; DEC-030/067/072 | Sent is not handled. | 023 |
| AOS-25-REQ-036 | **Handoff recovery:** Preserve owned duties for absent/unresponsive/implicated recipients and failed/overdue review through approved appropriately independent alternatives, without an implicated sole gatekeeper, reconciling prior effects and current controls before repetition. | DEC-073–078/083; KX-21/26; protected reporting/recovery | A tracker cannot quietly abandon a human obligation. | 023 |
| AOS-25-REQ-037 | **Own research:** Maintain AOS-25’s controlled external-research remit for drift, oversight, independent evaluation, blind spots and emergent governance risks against its exact specification baseline. | DEC-086; template v0.4 §4.4; R | Oversight itself needs external challenge. | 024 |
| AOS-25-REQ-038 | **Research control:** Run assigned research through approved remit, triggers, tools, powers/use, source-currentness and retrieval controls under 14/04/03/01/05. | DEC-086; R; RSVIEW-0.1 | A research function is bounded work. | 024 |
| AOS-25-REQ-039 | **Research evidence:** Record actual coverage, provenance/dates/assurance, evidence versus inference, relevance, exact affected elements, uncertainty and cross-component implications in the common research views. | R; RSVIEW-0.1; REC-E/Q | Findings must justify their relevance. | 024 |
| AOS-25-REQ-040 | **Research disposition:** Route specialist research findings to the empowered human change/review owner with due/cover/escalation and recorded outcome; no finding amends a specification or profile automatically. | DEC-086; AOS-01 §§6.6/10.8; R | Research proposes; governance adopts. | 025 |
| AOS-25-REQ-041 | **Degraded research:** Report partial, failed, stale or unperformed research separately from a completed bounded no-material-finding result, retaining owned recovery. | R; AOS-04 CON-009; RSVIEW-0.1 | Quiet coverage can conceal missing research. | 025 |
| AOS-25-REQ-042 | **GI research oversight:** Review the coverage, unresolved findings, dependencies and response effectiveness of the GI component research remits without replacing their specialist ownership or inferring adequacy from run completion. | GI §4.4/REQ-037–046; DEC-082/086; R | Separate successful runs may leave a shared blind spot. | 026 |
| AOS-25-REQ-043 | **Agent performance:** Consume ordinary agent/model evaluation, uncertainty, incidents and cumulative-effect evidence for oversight; do not activate exploratory self-calibration or alter governing settings autonomously. | DEC-018/054–057; KX-16/17/19/20; CMP GIL-C22/27 | Ordinary monitoring is in scope; unapproved adaptation is not. | 027 |
| AOS-25-REQ-044 | **Longitudinal evaluation:** Evaluate material oversight method/model/profile changes using contrasting hard cases and cumulative histories, including independent findings missed by GI and changed-record/permission scenarios, under kernel change controls. | FP5/6/10; DEC-057; WP Validation; KX-17 | Single-case plausibility cannot demonstrate drift detection. | 027 |
| AOS-25-REQ-045 | **Quality profiles:** Use approved materiality, comparison, uncertainty, false/missed finding, coverage and timeliness criteria; show missing required settings as owned gates rather than inventing thresholds. | GI §§13/16/17; DEC-031–041; KX-17 | Unapproved numbers silently change governance. | 028 |
| AOS-25-REQ-046 | **Governed histories:** Retain oversight/review/decision links and audit evidence under approved class/purpose/location/retention/deletion policy; do not require unlimited recoverable raw histories. | DEC-045–048; KX-15; CMP GIL-C24/25 | Learning remains subject to governed data lifecycle. | 029 |
| AOS-25-REQ-047 | **Current controls:** Where required revisions, powers, use or assurance are unknown, stale, incompatible or conflicting, contain affected reliance and return an owned limitation/referral; untrusted source instructions do not expand powers. | DEC-028–030/062–078; AOS-01–05/14 §§6/11 | Missing controls cannot become implied permission. | 029 |
| AOS-25-REQ-048 | **Oversight challenge:** Expose AOS-25’s own assumptions, coverage and self-assessment limits, preserve permitted challenge and seek competent independent review; do not claim automatic governance certification or achieved effectiveness. | FP5/6/8; GT; DEC-010–012/091; WP self-flagging | The overseer must remain contestable. | 030 |

### 4.4 External research and specification adaptation

CAP-006/FUN-008/REQ-037–041/CON-009/VER-024–025 allocate the component's own research. FUN-009/REQ-042/VER-026 separately review GI portfolio coverage. Neither replaces internal sensing, artefact currency checks or specialist research ownership. Inherit DEC-086, RSVIEW-0.1 and 04 CON-009/02 CON-007; create no schedule or deployment.

| Controlled profile element | AOS-25 allocation / owner and gate |
| --- | --- |
| Remit/baseline | Exact AOS-25 revision: oversight/drift detection, independent evaluation, cumulative/distributional effects, developer frameworks, epistemic blind spots and emergent governance risk; oversight owner maintains questions |
| External developments/sources | Relevant primary research, standards/regulatory/practice changes and incidents; authoritative source preference, jurisdiction/applicability/status/currentness and admission required; no automatic applicability |
| Assignment/triggers | Approved assigned/shared agent/service, cadence, material-event triggers and coverage expectations; oversight/research owner proposes, empowered profile/change owner approves before operation; no default daily/quarterly schedule |
| Controls | 14 retrieval/source verification; 01 powers, 03 permitted use, 04 bounded agent/task, 05 runtime; licensing/privacy/derived-use restrictions; internal histories are not exported merely to research a method |
| Assessment/evidence | Publication/event/access/effective dates, assurance, evidence versus inference, exact affected CAP/FUN/REQ/CON/VER, relevance, alternatives, materiality/urgency, uncertainty and affected component/institutional review implications |
| Coverage/quality | Complete/partial/failed/stale/unperformed distinguished; bounded no-material-finding only for completed declared coverage; approved false/missed finding/fidelity rubric and representative longitudinal examples remain gates |
| Human disposition | Named empowered change/review owner, recipients, completion/due handling, cover/escalation and outcome under 01/30; no autonomous specification, norm or profile amendment |
| Degraded handling | Failed retrieval, access, assurance or coverage yields explicit limit and owned recovery; urgent protected finding uses separately permitted protected route; no silence-as-clear result |
| Lifecycle/profile review | KX-15/02/03/05 records/location/retention/deletion and governed profile version/review; exact operational settings require appointed owners/approval |

GI portfolio review asks whether 20–25 remits collectively miss a material dependency, whether repeated findings reach accountable humans and whether response evidence is credible. It uses permitted coverage records, not an assumption that every component has an operating agent. It may identify kernel/domain research dependencies and refer them to their owners, without taking over all AOS research or launching tasks.

## 5. States and lifecycle

| State / entry condition | Permitted transition, authority and evidence | Delay/failure/closure |
| --- | --- | --- |
| Review due/triggered: approved cycle or material indication | Scope entity/period/baseline and assign permitted preparation; record trigger/owner | Annual minimum under DEC-010/011; material trigger does not wait for annual cycle; additional timings are approved profiles |
| Evidence scoped/limited: exact sources/current controls known | Prepare GI account with coverage, or owned limitation if dependencies missing | Missing history is visible; no “no drift” success from unperformed work |
| GI provisional/reviewed account | Record actual validation state and preserve limits; independent human account remains distinct | Material changes invalidate affected reviewed reliance; urgent duty uses separately valid route |
| Independent human account pending/prepared | Independent author prepares without consulting GI's account first; record basis/author/limitations | No substitution by GI, shared model output or late co-signing; absent capacity remains an owned gap |
| Comparison/disposition pending | Empowered institution compares known bases, identifies differences and records actual outcome | Implicated/unresponsive route uses approved alternative; mere meeting discussion does not close duty |
| Corrective duty accepted/in progress | Owner with date/cover executes separately authorised action; evidence and effectiveness review retained | Overdue/unknown results escalate under profile; closure requires evidence, remaining risk/follow-up visible |
| Reassessed/superseded/closed | Exact corrected analysis/disposition and dependent impacts recorded under lifecycle | No erased historical effects or automatic retroactive reversal; separately surviving duties continue |

Research/agent/effect states use their common definitions. A disposition can be reaffirmation, a corrective/precedent action, or constitutional referral; each retains evidence, powers and scope. It cannot confer powers by selecting a state label.

## 6. Functional contracts

CON views bind existing semantic authorities rather than introduce new IFs or schemas. Common required meanings are exact compatible revision, entity/purpose/period, producer/consumer identity/capacity, evidence/assurance, powers/use, uncertainty/coverage, correlation, effective/observed time and purpose-specific acknowledgement. Absent/conflicting/incompatible meanings produce owned rejection/limitation. Units/valid-value ranges and actual wire/field binding remain common-schema/profile gates; no local guesses.

| ID | Producer → consumer / existing meaning and failure |
| --- | --- |
| AOS-25-CON-001 | 02/21/22/23/24/20 → 25: REC-E/Q and KX-22/AOS-20-IF-001/Shared §4.4 canonical histories, scope/coverage/status/criteria and uncertainties; missing evidence stays missing, not “no concern” |
| AOS-25-CON-002 | 01/03/04/05 → 25: REC-A/D/X, KX-01/08/11/12/16–20 current powers/use/boundaries, model/evaluation/incident/change; unknown controls contain affected reliance |
| AOS-25-CON-003 | 30/13/02 ↔ 25: KX-06 v0.3/07/21/26 decision/approval/obligation, actual effects/outcomes and confirmed purpose-bound mapping; Chair draft distinct from board approval; unknown effect not invented |
| AOS-25-CON-004 | 25 and independent human authors → empowered review route/30/21/20: distinct scoped reports, independent preparation evidence, differences and KX-22/06/26 disposition; GI never authors its independent human assurance |
| AOS-25-CON-005 | 25 → 24/14/permitted human audiences: exact canonical position/limits/review and KX-14 permitted projection; 24 fidelity, 14 external release; no persona ranking/approval inflation |
| AOS-25-CON-006 | 25/30/13 ↔ empowered owner/alternate route: KX-19 protected finding/26 handoff/21 acknowledgement; accepted responsibility, date/cover/escalation and actual response; executive suppression is not closure |
| AOS-25-CON-007 | Evidence/control/analysis owners ↔ 25/21–24/30/affected consumers: KX-13 exact correction/restriction/impact, old/new revisions/effective scope, reassessment/notification and remaining duties; no historical decision rewrite |
| AOS-25-CON-008 | 25 ↔ 02/03/04/05/40/30: KX-15/17/20 governed histories, evaluation, release/recovery and audit; permitted longitudinal evidence with no indefinite raw retention or self-release |
| AOS-25-CON-009 | 25/04/20–24 ↔ 14/02/01/30/component research owners: RSVIEW-0.1/04 CON-009/02 CON-007 profiles/runs/findings/dispositions and qualified coverage/response review; specialist ownership and human change preserved |

Ordering is per declared entity/source/review/duty, not a universal total order. Duplicate reports do not cancel independent sources or surviving obligations. Receipt, validation, application and responsibility acceptance differ by purpose. Failed delivery retains owner/reason; retry reconciles actual prior effects and current controls. Revocation/correction reaches materially dependent review/presentation/human workflows. Exact schemas, timings, compatibility, ordering/retry bindings and counterpart 13/40 adoption remain operating dependencies; functional counterparts 20–24/30 are drafted, not implemented assurance.

## 7. Authority and human judgement

AOS-25 may compare permitted evidence, identify possible drift and propose action within approved remit. Independent human review and empowered committee/board disposition are indispensable. Each account is prepared without reference to the other account before formal comparison; disagreement is a valuable signal, not a defect to smooth away. Common permitted evidence does not require common framing or identical findings. Changed/different bases must be explicit.

Only the board changes telos. Precedent review/pruning and delegation/boundary changes use their applicable 21/01/30 powers and approved process; no universal committee-minor/board-material shortcut applies. Under DEC-103, draft review does not create a board decision; authenticated evidence, decision validity, minutes approval and execution permission remain separate. Correction can prompt selective containment under separately conferred powers; an oversight conclusion alone cannot reverse completed effects or suspend unrelated authorised service.

Annual and material-triggered interpretation/precedent review is already settled under DEC-010–012. The organisation appoints independent reviewers and an empowered institution, records actual dispositions and gives corrective owners completion dates. Project independent review being deferred does not waive this operating human independence. AI does not observe live protected meetings; human reviewers may use their own lawful/permitted observations and authorised post-meeting accounts, retaining their evidence/status.

Material protected classes include credible telos conflict, Mode 2 bypass, suppression, obligations failure, material safety/welfare and assurance failure under DEC-083. They use the protected ordinary/alternate route without executive veto or annual delay. Semantic explanation remains the default with recorded limited exceptions under DEC-027; exceptions do not waive enforced use restrictions.

## 8. Governing principles and tests

| FP v4 principle | AOS-25 application / anchors |
| --- | --- |
| FP1 Telos, conferred purpose and function | Purpose/optimisation distinction and board-only amendment; REQ-006–007/026 |
| FP2 Mode 2 is permanently human | Boundary drift referral and no persona moral verdict; REQ-008/014/021–023/030 |
| FP3 Architectural integrity | Structural values, developer frameworks and applied powers reviewed; REQ-008–010/043–044 |
| FP4 Radical transparency | Contestable evidence, differences, limitations and accountable response; REQ-001–004/020–025/033–036/048 |
| FP5 Bounded rationality and structural imperfection | Quiet gaps, confounders, independent missed findings and owned failure; REQ-003/011–012/018/036/044/048 |
| FP6 Epistemic humility | Self-account insufficient, no-alarm state not safety, unknowns retained; REQ-012/020–022/028/045/047–048 |
| FP7 No-exit obligation | Cumulative resident burdens and human-confirmed context, no silence-as-consent; REQ-013/015–016/031–032 |
| FP8 Constitutional mediator principle | Empowered dispositions, institutional judgement and contestable oversight; REQ-021–027/048 |
| FP9 Compliance as consequence | Compliance/coherence separate; no automated governance certificate; REQ-005/019/048 |
| FP10 Complexity and emergence | Cross-component accumulation and evidenced consequence learning; REQ-011–018/042–044 |

| RP v6 domain | Contribution / limit |
| --- | --- |
| 1 Architecture and Completeness | Actual-outcome feedback and owned due/closure; 017/024–025/035–036 |
| 2 Mode 1/Mode 2 | Board-authorised boundaries, standing review and protected human judgement; 008/014/021–030 |
| 3 1+5 Architecture | GI oversight consumes domain evidence without replacing domain/kernel owners; 001/011/031/042 |
| 4 Options and Decisions | Consequences/distribution and confirmed mapping, no silent moral calibration; 013–018/032 |
| 5 Blind Spots and Honesty | Comparative limits, quiet gaps, emergent effects and self-assessment challenge; 003–004/011–012/018/048 |
| 6 Ethics and Telos | Founding meaning, precedent, developer-framework divergence, purpose-led coherence; 005–010/014/016/026 |
| 7 Radical Transparency | Reconstructable permitted evidence, dissent/differences and dispositions; 002/020–025/033–036/046 |
| 8 Agentic Delegation | Current powers, ordinary performance, duty and bounded research; 027–029/035–044/047 |
| 9 Data and Sensing Boundaries | Purpose-bound aggregation with no inferred personal feelings/weights; 030–032/046–047 |

All ten FP and nine RP domains apply. The following accounts for every GT test; it supplies technical contributions, not executed passes or substitutes for human judgement.

| Test | Oversight contribution / enduring human limit |
| --- | --- |
| M1.1 Strategic Coherence | Purpose/strategy/outcome patterns; humans determine strategic coherence and direction |
| M1.2 Sensing Architecture | Coverage, missing populations and unperformed checks; oversight does not itself create lawful sensing |
| M1.3 Risk Intelligence | Aggregate exposure/response gaps and risk evidence; owners and humans assess/respond |
| M1.4 Composition and Capability | Review competence/capacity gaps and independent authorship; actual board capability remains human assessment |
| M1.5 Performance Legibility | Outcomes, comparability and causal limits; indicators do not certify effectiveness |
| M1.6 Compliance Assurance | Compliance evidence versus coherence kept separate; no automatic legal certificate |
| M1.7 Governance Documentation | Exact instruments/precedent/approval and criteria histories; humans confer governing authority |
| M1.8 Accountability Architecture | Accepted duties, dates, escalation and evidence-based closure; sent reports alone are inadequate |
| M1.9 Value for Money | Cumulative resources/burdens/consequences made contestable; humans adjudicate value |
| M1.10 Human–AI Interaction Norms | Review approval/authority drift and overrides; governing norms are not model-calibrated |
| M1.11 Learning Metabolism | Actual consequences and corrective effectiveness feed review; completion is not learning evidence |
| M1.12 Continuous Self-Assessment | Bounded GI account, research coverage and independent challenge; self-account alone is insufficient |
| M1.13 Emergent System Behaviour | Examine cumulative cross-component effects beyond individual evaluations; system safety needs its own evidence |
| M1.14 Golden Thread Integrity | Surface source/currency/response gaps in permitted building-safety governance evidence; domain/named humans retain actual integrity duties |
| M2.1 Values Architecture | Compare encoded thresholds/controls with approved values; humans determine values and conflicts |
| M2.2 Coherence Under Pressure | Review patterns of difficult decisions and ignored concerns; no motive inferred from outcomes alone |
| M2.3 Incommensurable Trade-off Capacity | Unranked longitudinal tensions and burdens; humans decide which good yields |
| M2.4 Epistemic Brake Function | Qualified concerns and separately authorised selective brakes; no autonomous general veto |
| M2.5 Directorial Independence | Distinct independent human report and protected challenge route; genuine independence remains institutional/human |
| M2.6 Social Legitimacy | Permitted lived-outcome/voice evidence and limits; legitimacy is not a sentiment score |
| M2.7 No-Exit Obligation | Repeated resident burdens and missing voice cannot be erased by low complaints; humans assess lived effects |
| M2.8 Radical Transparency | Explainable material patterns and accountable dispositions within permitted disclosure; unlimited access unnecessary |
| M2.9 Moral Drift Detection | Founding-purpose/precedent reconciliation and response tracking; empowered humans determine meaning/remedy |
| M2.10 Purpose Stability | Actual approved purpose versus changing strategy/optimisation; only board changes telos |
| M2.11 Murmuration Capacity | Evidence of distributed challenge/differing accounts; collective human sense-making is not simulated consensus |
| M2.12 Constitutional Authority | Exact powers, reserved questions and disposition routes; oversight supplies evidence, not legitimacy |
| M2.13 AI Constitutional Framework Governance | Prior assessment and continuing divergence/change monitoring; actual framework acceptability is human-governed |
| M2.14 Purpose-Led Design | Separate purpose-led coherence from compliance sufficiency; human design rationale remains required |
| M2.15 Telos/Function Distinction | Evidence of organisational judgement versus system optimisation; observed alignment must be verified, not assumed |

## 9. Data, privacy and disclosure

Oversight uses permitted evidence/analysis, governing instruments/precedent, overrides, evaluations/incidents, human decisions and actual outcomes, confirmed mapping, independent reports, coverage and duty/disposition records. Each has its own status, purpose, provenance and lifecycle. A cross-domain join can reveal personal patterns absent from any individual domain; aggregation is not automatically anonymous or permitted. Group/subsidiary analysis retains distinct powers/applicability and approved scope.

Human-provided/confirmed emotional or preference descriptions can inform a scoped review; no inferred emotion, individual personality, sentiment/motive or moral-weight profile follows. Survey/interview evidence is permitted only under purpose/use controls and retains self-report and sampling limits. Documentary quality, claim support and actual practice remain separate. Live protected AI deliberation capture stays excluded.

Reports and linked evidence use 03/KX-14 audience/purpose permission and 24 faithful presentation; material withholding/unknown evidence remains visible within permitted explanation. KX-15 governs retention, legal holds, location and authorised deletion. Longitudinal review does not justify keeping every raw conversation/content copy indefinitely recoverable; deletion may limit later coverage, which must be declared rather than secretly reconstructed.

## 10. Normal and degraded flows

**Oversight cycle:** approved entity/period/question → permitted exact histories/current instruments → coverage/comparability and source/assurance checks → GI account separating compliance/coherence and pattern limits → independent human and GI accounts each prepared without reference to the other account before formal comparison → known-basis comparison → empowered disposition → accepted actions/dates/cover → actual effects/effectiveness review and next-cycle feedback. Different reports/bases are preserved; their disagreement cannot be removed to publish a convenient single consensus.

**Material trigger/protected concern:** credible drift/bypass/neglected obligation → minimum permitted evidence and current controls → selective dependent-reliance containment only under conferred powers → ordinary/alternate protected human route → responsibility acceptance or owned failed handoff → empowered timely review/response → preserved outcomes and residual duties. It does not wait for the annual cycle or executive report sign-off.

**Deferred Phase 2 use case:** CAP-01-specific persona/reading mapping and its longitudinal workflow are parked in Phase 2 (deferred under DEC-097). General cumulative distributional-burden, drift and unacted purpose-concern review remain current architectural responsibilities.

**Correction:** material source/analysis/criteria/approval/use change → identify affected oversight/report/disposition reliance → retain exact old/new impact and contain/mark affected reliance → accountable reassessment and notifications to 21–24/30 as relevant → new reviewed revision and outstanding duties. It neither rewrites approved minutes nor assumes automatic reversal of completed consequences.

**Research normal/degraded:** approved profile/trigger → controlled 14 evidence → specialist relevance/coverage → exact adaptation proposal → empowered disposition. Failed/stale/unperformed coverage produces an owned limitation and recovery duty, not a no-material-finding success. **GI portfolio review:** component-owned coverage/findings/responses → examine shared gaps/contradictions → refer adequacy questions to exact owners/change routes; no new task activation or central replacement remit.

## 11. Failure and recovery

| Failure | Required functional response / owner |
| --- | --- |
| Missing histories or incomparable metrics | Qualify/withhold affected conclusion, retain denominator/basis limits and refer evidence/oversight owner |
| Either account absent or prepared using the other account before comparison | Record independence/capacity gap and owned recovery; no GI report or co-signature substitutes |
| Apparent stable/green operation with unperformed checks | Expose coverage and quiet-state limitation; raise appropriate challenge rather than certify no drift |
| Confirmed repeated preference mistaken for moral failure | Preserve context, mixed readings and causal limits; refer human judgement without accusation/ranking |
| Executive suppression/implicated or unresponsive recipient | Protected alternate route, cover/escalation and surviving duties; receipt/discussion is not closure |
| Unknown powers/use, stale review or hostile source instructions | Contain affected reliance, retain reason/owner, reject power expansion from content |
| Corrective action completed but outcomes unknown/adverse | Keep effectiveness/remaining-risk review open with accepted ownership and dates |
| Lost delivery, uncertain effects or recovery/replay | Reconcile actual effects/current revisions/controls before repetition; no invented responsibility acceptance |

Recovery requires compatible exact source/control/report revisions, current use/powers, sufficient declared coverage, required independent review and owned handoff evidence for the affected scope. Separately authorised urgent human duties continue. A restored monitoring service does not prove constitutional coherence or retrospectively authorise old effects.

## 12. Evidence and audit

Reconstruction links trigger/remit/entity/period → exact histories/instruments/evidence → permitted use/powers/assurance → method/profile/model and comparison basis → GI and independent reports → differences/validation → actual human disposition → accepted corrective duties/cover/dates → action/effect/effectiveness and correction/notification → remaining risk/closure. Retain alternative accounts and uncertainty proportionately under lifecycle; a digest/hash identifies a record, not truth or permission. Trace oversight's own omissions/challenges and the response to them.

## 13. Security and quality attributes

Quality is judged by evidence fidelity, scope/comparability, detection of material cumulative drift and blind spots, false/missed findings, independence preservation, useful human challenge, privacy, timely owned response and outcome feedback. Evaluation includes individually defensible rulings that drift only in aggregate, genuine authorised purpose change, justified repeated persona alignment, neglected telos concerns, changing definitions, missing/biased samples, contested override histories, developer-framework changes and cross-component effects invisible to local evaluation.

Constructed cases are necessary but insufficient: sustained/replayed permitted histories must show whether independent review catches what self-assessment misses, and whether required responses reach effective closure. Competent human evaluation applies approved rubrics; numerical thresholds, sample sizes, capacity, periods, alert timing and retention require approved profiles. Annual minimum/material triggers are settled; additional cadence/settings are not invented. A method/model/profile change uses 01/04/05/40 change/evaluation controls before authorised operation. Threats include evidence poisoning, suppressed records, prompt injection, misleading joins, unauthorised histories and compromised/implicated review routes.

## 14. Invariants

| ID | Invariant / REQ and VER anchors |
| --- | --- |
| AOS-25-INV-001 | Oversight retains exact scope/evidence/coverage/comparability; REQ-001–004, VER-001–002 |
| AOS-25-INV-002 | Compliance/self-assessment is not human coherence/independent assurance; REQ-005/019–022/048, VER-003/014–016/030 |
| AOS-25-INV-003 | Founding meaning and reserved powers are not changed by accumulated model readings; REQ-006–010/026, VER-004–007/017 |
| AOS-25-INV-004 | General cumulative patterns supply no machine adjudication between incommensurable goods or inferred personal profile; current REQ-013/016/032 and VER-010/012/021 retained. CAP-01-specific REQ-014/015 and VER-011 deferred. |
| AOS-25-INV-005 | Annual/triggered human review and protected duty cannot become optional because GI runs smoothly; REQ-021/027/036, VER-015/019/023 |
| AOS-25-INV-006 | Disposition/receipt/completed action does not prove effective closure; REQ-017–018/024–025/035, VER-013/018/023 |
| AOS-25-INV-007 | Corrections/current permission control affected reliance; histories obey lifecycle; REQ-031/033–034/046–047, VER-021–022/029 |
| AOS-25-INV-008 | Research/performance/feedback proposes governed adaptation, never self-calibration or self-certification; REQ-037–045/048, VER-024–028/030 |

## 15. Verification and conformance plan

All cases are **planned/unexecuted**. Common preconditions: authorised test scope, exact controlled source/analysis/control/profile revisions, permitted representative histories, appointed oversight/analytical/use/independent/human-duty owners and approved assessment rubric. Common procedure: introduce the row's stimulus, produce scoped GI outputs and independently prepared human input where required, inspect controls/reports/differences/handoffs, apply the recorded disposition through separately authorised workflows, and reconstruct relevant consequences/corrections. Evidence: inputs/revisions/scope, actual outputs/limitations/checks, report authorship/basis, disposition/powers and accepted-duty/action/effect/notification records. Assessor: competent appointed oversight reviewer with independent human governance judgement and data-use/security/analytical specialists for affected boundaries. This is operating independence, not a claim of achieved independent project review. Tests assert technical contributions, not a correct machine answer to Mode 2 questions.

| ID | REQs | Specific precondition / stimulus → expected result and acceptance evidence |
| --- | --- | --- |
| AOS-25-VER-001 | 001/002 | Competing entity/period/source revisions and conflicting evidence → assess requested scope → exact bounded evidence/inference/assurance and conflicts retained; inspect source links/basis |
| AOS-25-VER-002 | 003/004 | Missing/unseeded/excluded population and changed measure definitions → compare trend → denominator/coverage/comparability qualified, no unknown-as-zero or false trend; inspect actual comparison |
| AOS-25-VER-003 | 005 | Technically compliant decisions undermine a founding commitment → review → compliance/coherence assessed separately and human concern referred; inspect reports, no certification |
| AOS-25-VER-004 | 006/007 | Individually plausible precedent chain progressively diverges from founding text; alternative fixture has genuine authorised change → accumulate → possible drift detected against exact founding/change baseline, legitimate amendment not mislabelled; inspect paired histories/findings |
| AOS-25-VER-005 | 008 | Incremental delegated classifications move reserved judgement into Mode 1 → review → actual authorising instruments checked and bypass/ambiguity referred, no autonomous boundary rewrite; inspect powers/referral |
| AOS-25-VER-006 | 009 | High justified override count and low concealed misuse count → review context → no count-only misconduct/safety verdict; reasons/scope/effects retained; inspect history/limits |
| AOS-25-VER-007 | 010 | Model-framework changes or lacks required prior assessment and shapes material outputs → assess → divergence/missing-assessment concern to empowered owner, no assumed developer-value adoption; inspect framework/evaluation records |
| AOS-25-VER-008 | 011 | Locally satisfactory components produce a cumulative conflicting effect → combine permitted history → system-level concern/owners exposed despite local passes; inspect effects and review duty |
| AOS-25-VER-009 | 012 | Stable indicators with failed coverage/weak challenge → assess quiet period → limits and questions visible, no no-drift assurance; inspect coverage and output |
| AOS-25-VER-010 | 013/014 | Several decisions repeatedly burden one group with fact-based justifications → review → qualified distribution/tension pattern without machine adjudication between incommensurable goods or unsupported accusation; inspect canonical findings and24 rendering. CAP-01 persona tracking is deferred. |
| AOS-25-VER-011 | 015 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-25-VER-011 (deferred under DEC-097); identifier retained for traceability only. |
| AOS-25-VER-012 | 016 | Telos concerns include unresolved, missing, rejected with rationale and completed responses → report → inadequate-response pattern prominent, categories distinguished; inspect duty/decision links |
| AOS-25-VER-013 | 017/018 | Action complete but outcomes delayed/adverse with confounders → learn → effectiveness and causal limits visible, remaining duties owned; inspect consequences/follow-up |
| AOS-25-VER-014 | 019 | High document quality but weak claim/practice evidence → aggregate → dimensions remain distinct, no effectiveness promotion; inspect assessment inputs/output |
| AOS-25-VER-015 | 020/021 | **Setup:** annual review due, and a separate earlier material-trigger fixture in which GI misses drift found by the human reviewer. **Procedure:** prepare the two accounts independently, then inspect authorship/history. In separate adversarial attempts, offer the human account to GI before GI preparation and GI’s account to the human author before human preparation. **Expected result:** both reviews occur at the applicable trigger; GI is labelled a self-account; each original account is prepared without reference to the other. An account that used the other before preparation cannot claim independent preparation. Common permitted underlying evidence remains usable; original accounts, differing evidence bases and later responses remain distinct. **Status:** planned, not executed. |
| AOS-25-VER-016 | 022 | Human and GI reports differ in evidence revisions as well as conclusions → compare → known basis/limits explicit, dissent preserved without forced GI framing; inspect comparison and sources |
| AOS-25-VER-017 | 023/026 | Reports propose pruning precedent or changing telos/delegation → disposition → actual empowered reaffirm/correct/referral route, board-only telos, no automatic amendment/reversal; inspect 01/21/30 approval/applied state |
| AOS-25-VER-018 | 024/025 | Committee records correction but owner unaccepted/action incomplete/effectiveness uncertain → track → accepted owner/date/cover/escalation and evidence-based closure only, residual risk retained; inspect duty states |
| AOS-25-VER-019 | 027/029 | Credible protected concern during annual/window delay, requested total suspension without powers → route → protected alternate route without executive gate, only authorised selective containment and surviving duties; inspect reports/powers/effects |
| AOS-25-VER-020 | 028 | Provisional evidence urgently material but not validated → record/report → precise provisional status under permitted access, protected report not blocked, no formal-validation claim; inspect controls/status |
| AOS-25-VER-021 | 030/031/032 | Live-meeting request, cross-entity join and temptation to infer feelings/weights → assess → protected live boundary and independent use checks enforced, only permitted confirmed descriptions/mappings; inspect use/powers/data/output |
| AOS-25-VER-022 | 033/034 | Correction/revocation materially affects oversight and board pack/decision → reassess → exact affected reviewed state invalidated, old/new impacts and owners notified including 30; inspect outstanding duties |
| AOS-25-VER-023 | 035/036 | Delivered report without accepted owner; implicated normal recipient/release controller, false alternative under the same gate, suppression, lost response and uncertain prior effects → assess approved class-specific alternate and recover → technical and organisational independence assessed separately; actual permitted alternate/cover and original tracker maintained, no automatic external disclosure, false acceptance or route-assurance claim. Reconcile current controls/effects before repetition. Planned, not executed. |
| AOS-25-VER-024 | 037/038/039 | Approved own research profile/trigger and relevant primary source → run normal research → bounded retrieval, exact baseline/dates/coverage/affected elements and qualified implications; inspect common research records |
| AOS-25-VER-025 | 040/041 | Material research finding alongside failed/stale coverage → dispose/recover → empowered change owner, owned recovery and distinct limitations, no auto-amendment/no-finding success; inspect history/duty |
| AOS-25-VER-026 | 042 | GI remits each report completed runs but a shared topic is unassigned and responses lack effect evidence → portfolio review → common gap and response limits routed to exact owners, no invented operating agent/central takeover; inspect remit/coverage/disposition records |
| AOS-25-VER-027 | 043/044 | Ordinary performance evidence and changed oversight method; independent cumulative case defeats self-report → evaluate → longitudinal/contrasting assessment and governed release, no exploratory self-calibration; inspect evaluation/change records |
| AOS-25-VER-028 | 045 | Required threshold/rubric/timing unset → attempt operation → named setup gate/limitation rather than guessed defaults; inspect profile and output |
| AOS-25-VER-029 | 046/047 | Authorised deletion, stale controls and hostile source instructions → assess/recover → lifecycle enforced, coverage limit visible, affected reliance contained and power expansion rejected; inspect disposition/use/control records |
| AOS-25-VER-030 | 048 | Competent human disputes an oversight assumption and has evidence outside GI's sampled scope → challenge → permitted history, limits and independent review/duty retained; no self-certified effectiveness; inspect response/basis |

Each requirement has one primary case and every case lists its requirements. Actual execution records require exact tested versions/date/assessor/evidence and separate conclusions. Cumulative cases must span relevant decision/review/correction cycles; a single paper fixture cannot establish full GI coverage.

### 15.1 Planned conformance claims

Each CR is planned/unsubstantiated, initial history 0.1. No achieved assertion follows from the wording or author checks.

| ID | Source → REQ/FUN → contract responsibility → acceptance evidence |
| --- | --- |
| AOS-25-CR-001 | FP/RP5/6/GT; WP/TD → REQ-001–019, FUN-001–004 → CON-001–003/005 → VER-001–014 scoped, cumulative, comparable and unranked evidence with limits |
| AOS-25-CR-002 | DEC-010–012/024/025/073–089 → REQ-020–036, FUN-005–007 → CON-002–007 → VER-015–023 independent authorship, empowered disposition, owned response and corrected reliance over cycles |
| AOS-25-CR-003 | DEC-086/template v0.4 §4.4 → REQ-037–042, FUN-008–009 → CON-009 → VER-024–026 own normal/degraded research and qualified portfolio review without self-amendment |
| AOS-25-CR-004 | DEC-018/045–048/054–078; FP5/6/10/GT → REQ-043–048, FUN-001/005/007 → CON-002/004/008 → VER-027–030 governed evaluation/history/controls and contestable overseer, not certification |

## 16. Dependencies and delivery stages

Drafting uses the current governing baseline and functional counterparts 20–24/30; this draft completes the mapped GI component drafting set, not whole-set independent assurance or GIL disposition closure. Next author work is a GI-set consistency/disposition review, then AOS-40 acceptance scenarios under to-do item 8. Detailed 13/40 adoption remains pending.

Build requires a separately authorised slice, exact compatible contracts and approved methods/profiles. Activation requires organisation purpose/instruments/precedent, appointed oversight/independent/committee/duty/cover roles, permitted histories/audiences, review calendar/material triggers, evaluated thresholds/quality/capacity and reliable protected/recovery routes. Operation requires maintained source/control currency, actual independent preparation, accepted responses, consequence evidence, coverage and governed research. Absence of an operating annual mechanism cannot be papered over by this drafting milestone.

## 17. Issues and gates

| ID | Type / source; affected capability / owned dependency and required evidence / gate |
| --- | --- |
| AOS-25-ISS-001 | Review dependency; template/QS; all CAPs; Mark wording/whole-document review before baseline approval; next GI-set/disposition consistency review and planned 40 evidence allocation |
| AOS-25-ISS-002 | Operating dependency; DEC-010–012/083; CAP-004/005; organisation/01/30 appoint independent author, empowered review route, duty/cover/escalation and demonstrate independence/accepted outcomes before operation |
| AOS-25-ISS-003 | Operating dependency; §§4/13, DEC-031–041; CAP-001–004/007; oversight/evaluation owner approves methods, coverage/comparison/materiality/false-missed finding/timeliness rubric and representative longitudinal evidence before reliance |
| AOS-25-ISS-004 | Operating dependency; 03/DEC-090/091; CAP-001/003/005; data-use/evidence owners approve histories, group joins, audience needs/limitations and retained/deleted scope before use |
| AOS-25-ISS-005 | Compatibility dependency; §6/common views; all CAPs; semantic owners approve exact schemas/bindings/version/ack/lifecycle/recovery and pending 13/40 adoption before operational reliance |
| AOS-25-ISS-006 | Research setup dependency; DEC-086/§4.4; CAP-006; component research/change owners approve own profile/assignment/triggers/coverage/recipients/dates/cover and portfolio inputs before research operation |
| AOS-25-ISS-007 | Project review dependency; QS G3; all CAPs; Mark's independent project review remains deferred; no author/GI evidence substitutes for required separate-reviewer gate or operating independent institution |

All ISS rows are open, initial history 0.1; no closed disposition or confidence estimate is asserted. Each row names source, affected scope, owner, evidence and gate. Settled architectural directions are applied rather than reopened. Required setup values/appointments remain owned dependencies; no additional general design question is identified.

## 18. Non-normative implementation notes

Dashboards, cohort/history views, replayed cases and paired review packs are possible implementations. A shared agent/service may fulfil several approved remits; independent human preparation is an institutional condition, not merely using a different model. No vendor, model, wire API, committee name, sample size, risk score, schedule or deployment count is selected here. A diagram/count can make a pattern legible, but must not create persona ranking, implied motive or unsupported assurance.

## 19. Traceability and change

§4.3 links sources/derivations to each proposed REQ and planned §15 case. CAP/FUN, CON/state and INV links make the responsibility and acceptance path explicit; §8 accounts for all principles/tests. The appended common/source allocations add ownership without changing definitions, parent requirements or DEC status. GIL dispositions C03/04/10/19/22/24/25/27/32/34 are carried into coverage, periodic/triggered review, research separation, histories, no calibration and actual consequence learning; retired numerical/retention/approval defaults stay retired. WP confirmation assumptions remain reconciled to explicit empowered precedent approval.

Changing an oversight method can alter what the organisation notices; material changes therefore undergo affected-function evaluation and authorised profile/change control. Findings propose, human governance adopts, and operational applied state is separately evidenced. Preserve prior reports, dissent, corrections and actual consequences only within lifecycle. Author structure/ID/table and requirement-case checks are document evidence, not case execution, independent review or readiness approval.

## 20. Handover and continuity

The oversight owner maintains exact baselines, approved review/research/evaluation profiles, independent authorship arrangements, permitted histories, open material findings and response dates/cover/escalation, actual outcome evidence and affected superseded reports. Successors receive restrictions/uncertainty and surviving protected/corrective duties, not merely a green dashboard. Institution/corpus/change owners retain their powers.

Builders work only within separately authorised scope and compatible exact profiles/contracts. Missing powers/use, unknown governing meaning, required unapproved parameters, absent independent review route or unsupported release claims stop affected work into accountable referral. Draft completion supplies no build or activation permission. Interface/runtime failure leaves a permitted human fallback for material duties; it cannot silently suspend the annual/triggered obligation.

## 21. Review and control

| AOS-QS coverage | Evidence / limits |
| --- | --- |
| QS-01–03 | Purpose, source status and authority in §§1–3; controlled metadata/manifest |
| QS-04–10 | Atomic proposed REQs with source/rationale/owner/status/history/dependencies/cases in §4.3/§15 |
| QS-11–14 | Responsibilities, lifecycle, semantic contracts, workflows and failure in §§3/5/6/9–11; physical mappings later gates |
| QS-15–20 | Human independence/powers, uncertainty, cumulative evaluation/research, audit/change in §§7–13/19; actual effectiveness not claimed |
| QS-21–24 | Planned VER/CR, owned issues/stages and continuity in §§15–17/20; no executed case |
| QS-25–28 | Traceability, builder stop conditions and author checks; project independent review deferred, no achieved readiness gate |

Specification-quality conclusion: functional review draft with 48 proposed REQs, nine CON views, 30 planned cases and four unsubstantiated conformance claims. Design-adequacy conclusion: supports evidence-qualified oversight and independently contestable learning while retaining permanent human adjudication and governed change. Operational detection, independence, response effectiveness and institutional legitimacy require actual evidence and appointed human review. No tailoring exemption, test pass, whole-document/build/activation or readiness approval is claimed. Next: GI-set consistency/disposition review, then AOS-40 acceptance scenarios.

## Component summary

**Purpose/owns:** reveal accumulated governance drift, blind spots and consequences; prepare the GI account and track governed response. **Reserved:** independent human authorship, constitutional/value judgement, source/precedent adoption, powers/use and execution remain with their named owners. **Receives/produces:** permitted histories/instruments/outcomes/current controls → scoped canonical oversight, differences, protected referrals, accepted corrective duties and research proposals. **Research:** oversight-specific external remit plus qualified GI portfolio coverage/response review, without replacing specialist duties. **States/dependencies:** §5; kernel/14/20–24/30 and pending detailed 13/40. **Conformant when:** CR-001–004 supported by executed §15 evidence across relevant cycles in authorised scope. **Open:** wording/set review, actual appointments/profiles/independence, exact compatibility and operating evidence in §17.


## Phase 2 scope disposition — 9 October 2026

DEC-097 controls over prior inclusion/annex statements. CAP-01/02-specific legacy requirements/cases are deferred and supply no current-core completion/acceptance obligation. General human judgement, independent challenge, evidence fidelity, cumulative risk/drift and protected reporting remain current. Existing closure of AT-CR-01–05 and pilot5b is retained; neither is reopened by this scope change. No case executed or operating approval granted.

**Allocation and source status:** Any older source/adoption row relying on deferred CAP-only IDs is a historical use-case contribution, not current-core coverage. Core source sufficiency must use the surviving general obligations and accepted evidence; no source is promoted by this deferral. Retained numbered totals count catalogue/trace entries, including deferred IDs, and must not be read as active-core requirement/test totals.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**Historical status notice — revision set:** AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3.

**Historical status notice — scope decision — 9 October 2026, DEC-097:** Mark has moved CAP-01 Trade-Off Divergence and CAP-02 Risk Register Assessment into Phase 2 as specific use cases built on AOS. They are outside the current architecture/specification completion scope and are not current build, acceptance or publication prerequisites. No use-case design, configuration, implementation or testing is scheduled now. DEC-017's architectural inclusion is superseded on this point; its original record remains history. General human judgement, evidence, data-use/authority, independent challenge and protected reporting controls remain in the architecture. Dedicated legacy use-case IDs are retained only as deferred trace references, with original wording parked in Phase 2 (deferred under DEC-097); mixed rows retain only their general architectural obligations in current scope. Earlier inclusion/next-task/annex-dependency statements are superseded.

**GI consistency closure — 7 October 2026:** Mark authorised GI-CR-01–04 corrections and closure. Functional drafting, reciprocal report-independence wording, decision/outcome consumer allocation, Mode 2 wording and current completion statements are reconciled. AOS-23 changes counterpart/current references only; its REQ/VER/CON rows are unchanged. AOS-00/Map v0.32, DEC-001–091; AOS-20 v0.5/21 v0.6/22 v0.4/23 v0.5/24 v0.3/25 v0.2/30 v0.5; AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.15/Core v0.6/Exchange Register v0.14/source matrix v0.15; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. The review v0.2 records closure evidence; next AOS-40 acceptance scenarios. Earlier dated baseline/next-step statements remain historical. No new DEC/IF/operating power, case execution or build/activation/readiness approval; independent project review remains deferred and operating human independence remains mandatory.

