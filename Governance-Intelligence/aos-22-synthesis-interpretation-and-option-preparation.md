# AOS-22 — Synthesis, interpretation and option preparation

Document: aos-22-synthesis-interpretation-and-option-preparation · Source revision or record: v0.6

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**DEC-103 adopted — 29 October 2026:** Current revision 0.6. Decision validity/effective time, attributable evidence/authentication, minutes approval and permission to execute are separate. DEC-087 is partly superseded; [decision/amendment and legal-source record](../Supporting-Specifications/aos-dec-103-decision-validity-evidence-and-minutes-2026-10-29.md). No universal later-minutes or second decision-record approval gate. Exact instruments/evidence policy, KX-06 v0.3 compatibility and ordinary separate review/readiness gates remain required; cases unexecuted. Earlier contrary wording is historical only where explicitly identified.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](../Supporting-Specifications/aos-current-document-inventory-2026-10-29.md) and [correction record](../Supporting-Specifications/aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

**AOS-25 oversight counterpart alignment — 7 October 2026:** AOS-25 v0.1 now supplies the drafted oversight/drift/learning and GI research-portfolio counterpart. Reference-only revision; all existing requirement/case/contract rows preserved. AOS-00/Map v0.31, DEC-001–091; AOS-25 v0.1; AOS-20 v0.4/AOS-21 v0.5/AOS-22 v0.3/AOS-23 v0.4/AOS-24 v0.2/AOS-30 v0.4 (counterpart-reference alignment only); AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.14/Core v0.6/Exchange Register v0.13; source matrix v0.14; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. No build/activation/readiness approval. Next: author GI-set consistency/disposition review across AOS-20–25 and AOS-30, then AOS-40 acceptance scenarios under item 8; independent project review remains deferred. Earlier dated consultation/adoption entries remain history.

**AOS-24 presentation counterpart alignment — 7 October 2026:** AOS-24 v0.1 now supplies the drafted faithful-rendering/explanation counterpart. Reference-only revision; requirement, case and contract rows unchanged. AOS-00/Map v0.30, DEC-001–091; AOS-24 v0.1; AOS-21 v0.4/AOS-22 v0.2/AOS-23 v0.3 (reference alignment only); AOS-01–05 v0.8, AOS-14 v0.4, AOS-20 v0.3, AOS-30 v0.3; Shared v0.13/Core v0.6/Exchange Register v0.12; source matrix v0.13; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. No build/activation/readiness approval. Earlier dated consultation/adoption entries remain history.

| Document control | Value |
| --- | --- |
| Component / version / date | AOS-22 / 0.6 / 29 October 2026 |
| Status | Functional specification review draft; proposed requirement wording |
| Architecture baseline | AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3. |
| Governing sources | Foundational Principles v4; AOS Reasoning Principles v6; Governance Intelligence Tests; preserved source manifest |
| Dependency baseline consulted | AOS-01–05 v0.8; AOS-14 v0.4; AOS-20 v0.3; AOS-21 v0.2; AOS-23 v0.1; AOS-30 v0.3; Shared v0.11/Core v0.6/Exchange Register v0.10; source matrix v0.11; Control Coordination v0.2; Protected Reporting and Recovery v0.1; research view RSVIEW-0.1 and KX-06 v0.3 |
| Adoption supplements | Shared v0.12/Register v0.11/source matrix v0.12 record AOS-22 functional adoption; common meanings unchanged |
| Quality / template | AOS-QS v0.1; component template v0.4 |
| Project owner / custodian | Mark Sweeny |
| Operational owner | Accountable GI synthesis owner; empowered validators, constitutional reviewers, independent challenge owners and duty/cover roles require organisation appointment |
| Author / reviewers | Codex at Mark's request; author document checks only; Mark wording/whole-document review pending; independent project reviewer unassigned/deferred |
| Approval / readiness | Existing recorded design directions approved; no whole-document, build, activation or achieved readiness gate |
| Change history | 0.4 — GI-CR-01–04 author consistency correction/closure under Mark’s instruction; existing identifiers and proposed/planned status preserved. 0.3 — AOS-25 counterpart/reference alignment only; no requirement/case/contract change. 0.2 — AOS-24 counterpart/reference alignment only; no requirement/case/contract change. 0.1 initial functional draft; applies approved corpus/assessment, interpretation, human judgement, CAP-01, independent preparation and own research directions; no new DEC/IF |

## 1. Purpose and scope

AOS-22 connects permitted evidence across the five sensing domains, governance corpus and artefact assessments to a contestable interpretation and an honest option set. It makes the organisational question, evidence, tensions, constraints, consequences and remaining human judgement visible. Without it, the AOS can produce individually plausible domain reports while missing their contradictions, treat an executive framing as fact, or allow machine interpretation to become governing meaning.

Scope includes cross-domain pattern/conflict detection, evidence-grounded propositions, routine-versus-constitutional classification/referral, bounded scenarios and options, infeasible alternatives, stakeholder divergence, independent challenge preparation and canonical analysis contributions. CAP-01 Trade-Off Divergence is a deferred Phase 2 use case built on these general functions; its specific workflow is not part of current AOS-22 scope. For current architectural work, AOS-22 owns synthesis/interpretation/option preparation and analytical contributions; AOS-23 owns artefact assessment, AOS-24 rendering, AOS-25 longitudinal/aggregate oversight and AOS-30 human deliberation, decisions and duties.

AOS-21 owns sourced organisation/subsidiary knowledge, corpus, criteria and approved precedent. AOS-01–05 own powers, records, use, agent behaviour and runtime controls; AOS-14 governs external retrieval/exchange; AOS-13 operational coordination. AOS-22 does not create authority, adopt precedent, amend telos, adjudicate incommensurable goods, observe live protected deliberation, infer personal feelings/preferences, dispatch unauthorised actions or certify organisational effectiveness. Parent/subsidiary context remains distinct under DEC-090.

Stakeholders include boards/committees, independent directors, executives, residents, staff, domain owners, corpus stewards, analytical reviewers and operators. A perspective represents a declared analytical frame, not a claim about what a particular person feels or ought to prefer. Technical capability, smooth operation, a persona's voice or a confidence score supplies no moral authority.

## 2. Authority and sources

FP v4/RP v6 govern; recorded decisions constrain proposed wording. Working material is explicitly reconciled. Each requirement is a functional derivation unless directly applying a cited approved direction. Source keys below include durable locators used by the requirement register.

| Key | Exact source / locator and standing |
| --- | --- |
| FP | Foundational_Principles_v4.docx, principles 1–10; applicability in §8 |
| RP1 | RP v6 Architecture and Completeness: closed feedback, named accountability, “Every option set must include the option that cannot be made to work”, and “The ‘AI said so’ test” |
| RP2/3 | RP v6 Mode 1/Mode 2 Boundary: permanently human judgement and boardroom exclusion; 1+5 Architecture: defined roles and cross-domain handoff |
| RP4 | RP v6 Options and Decisions: actual organisational state, consequential decision feedback and revealed preferences |
| RP5/7 | RP v6 Blind Spots and Honesty / Radical Transparency: declared limits, uncertainty, auditability and contested evidence |
| RP6 | RP v6 Ethics and Telos: conferred purpose versus function, precedent drift, developer frameworks, no-exit and purpose-led design |
| RP8/9 | RP v6 Agentic Delegation / Data and Sensing Boundaries: explicit task/powers, protected duty and permitted purpose |
| GT | Governance_Intelligence_Tests.docx, M1.1–14/M2.1–15; technical contributions and permanent human limits |
| WP | Governance Intelligence: Internal Architecture — Working Paper, “Synthesis”, “Interpretive”, “How the corpus holds meaning”, “Governance of drift” and “Charter”; its RP v5 and confirmation-to-precedent assumptions reconciled to DEC-080/081 |
| TD | Trade-Off Divergence Tool — Product Specification (Working Draft).md §§1–7, especially rigour gate, shared factual basis, prohibition, independent configuration and longitudinal report; historical configuration scope under DEC-017, superseded for current scope by DEC-097; retained source contribution only, constrained by the GI charter |
| PN | Petra.md, essential style principle and descriptive persona; explanatory interaction input, not interiority, powers or a governing instrument |
| CMP | GIL comparison filename v0.1/content v0.2: GIL-C02/03/09/16/18/29/32–35 and allocation to 22; no wholesale GIL adoption |
| D | AOS-00 v0.28 DEC register, individually cited directions including 005/008/010–012/017/018/024–027/062–091 |
| GI | AOS-20 v0.3 §§3–7/10–15; REQ-010–028/029–036: synthesis, review, no moral winner, CAP-01 and protected duties |
| C / AS / H | AOS-21 v0.2 §§3–7/9–11/19; AOS-23 v0.1 §§3–7/10/19; AOS-30 v0.3 §§5–7/9–12; corpus, distinct assessment dimensions and exact human powers/outcomes |
| E/A/U/X/K | Core v0.6 REC-E/Q/A/D/X; Shared v0.11 §4; Register v0.10 KX definitions; coordination v0.2 and protected reporting/recovery v0.1 |
| R | DEC-086/template v0.4 §4.4; AOS-04 v0.8 §§3.1/5.1/6.6/10.8 CON-009; AOS-02 v0.8 §6.6 CON-007; AOS-01 v0.8 §§6.6/10.8 |

RP4's use of revealed preferences is applied through DEC-088: human-provided/confirmed purpose-bound descriptions may inform proposals and review, but cannot silently change governing instruments, precedent, moral weights or calibration. TD's early “who sees what and when” question is resolved at architectural level by DEC-085 governed preparation windows and required management response, not a blanket secret/shared default. WP confirmation creates an interpretation candidate; explicit empowered approval is still required for precedent.

No new legal/standards currency verification or ISO clause claim is made. New external obligations require admitted primary evidence, status/jurisdiction/effective-date checks and empowered applicability. The preserved source manifest remains unchanged. PN's human character language does not confer AI feelings, conscience, autonomous authority or access to protected deliberation.

## 3. Responsibilities

| Responsibility | AOS-22 owns | Reserved / shared owner |
| --- | --- | --- |
| Synthesis | Correlate permitted exact evidence, competing accounts and domain implications | Domain owners supply facts; 02 assurance; correlations are not established causes |
| Interpretation | Propose evidenced readings, identify governing tier/authority conflicts and refer judgement | 21 corpus/precedent; 01/30 empowered adoption; no self-ratified meaning |
| Options | Make viable, constrained, infeasible and materially competing alternatives/consequences legible | 30 humans choose; 13/authorised executors act only with separate current powers |
| CAP-01 rigour/divergence — deferred Phase 2 only | Historical use-case allocation: assess evidential rigour with 23; shared-basis persona tension map without verdict. No current-core responsibility arises from this row (DEC-097). | Retained trace to the Phase 2 use case; general 23/24/25 responsibilities remain governed by their current requirements. |
| Independent preparation | Apply approved challenge profile/window using canonical evidence | Independent governance route approves; tested executive cannot tune/suppress; 03 use and 30 management response |
| Feedback/correction | Revise dependent synthesis and communicate exact status; supply decision/outcome links for review | 21 sources/precedent, 23 assessments, 25 drift, 30 account/decision review |
| Own research | Specialist relevance of external developments affecting synthesis/interpretation/options | R shared controls/records; 14 retrieval; 01 human amendment/activation |

Roles are accountable GI/synthesis owner, domain/evidence owners, corpus Steward, analytical validator, constitutional referee, independent profile approver/reviewer, handoff tracker/recipient/cover and change/release authority. Actual powers, classification/materiality rules, review windows and capacity are organisation dependencies. One role label or user confirmation does not establish all these capacities.

## 4. Capabilities and functions

### 4.1 Capabilities

| ID | Outcome |
| --- | --- |
| AOS-22-CAP-001 | Synthesize exact permitted cross-domain evidence with conflicts and limits visible |
| AOS-22-CAP-002 | Prepare contestable interpretations and refer governing questions to humans |
| AOS-22-CAP-003 | Prepare grounded options, infeasible alternatives and consequence/trade-off evidence |
| AOS-22-CAP-004 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-CAP-004 (deferred under DEC-097); identifier retained for traceability only. |
| AOS-22-CAP-005 | Preserve canonical review/presentation and owned protected handoff boundaries |
| AOS-22-CAP-006 | Incorporate material correction and human decision/outcome feedback without self-adoption |
| AOS-22-CAP-007 | Research external developments affecting this component and propose governed adaptation |

### 4.2 Functions

| ID | Trigger → input → behaviour → output; boundary/failure |
| --- | --- |
| AOS-22-FUN-001 | Approved request/proactive trigger → exact permitted domain/corpus/assessment evidence → scoped selection/reconciliation → evidence snapshot with gaps; missing mandatory context blocks dependent conclusions |
| AOS-22-FUN-002 | Snapshot/question → cross-domain accounts → detect patterns/contradictions/possible implications → evidenced synthesis; unproven causality remains an hypothesis |
| AOS-22-FUN-003 | Proposition/authority tension → 21 tiers/precedent/powers → routine/constitutional classification under approved policy → interpretation candidate or empowered referral; uncertainty cannot choose the lighter approval route |
| AOS-22-FUN-004 | Material decision question → actual conditions/constraints → options and bounded scenarios, infeasible alternative and consequences → human question/options; no invented feasibility or moral winner |
| AOS-22-FUN-005 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-FUN-005 (deferred under DEC-097); identifier retained for traceability only. |
| AOS-22-FUN-006 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-FUN-006 (deferred under DEC-097); identifier retained for traceability only. |
| AOS-22-FUN-007 | Canonical analysis ready → exact review/window/use → validation/return and permitted preparation/presentation → review-bound output; no approval by delivery or dialogue |
| AOS-22-FUN-008 | Mandatory concern/deadline failure → separately permitted finding/duty → protected or ordinary handoff with cover → accepted human responsibility; no executive veto of protected route |
| AOS-22-FUN-009 | Material correction/decision/outcome → exact affected analysis/history → reassessment and review evidence for 21/23/25/30 → updated status/owned follow-through; no silent normative calibration/effect reversal |
| AOS-22-FUN-010 | Approved research trigger → external evidence via 14 → relevance/impact/alternatives → common research finding/disposition/change proposal; no autonomous amendment |

### 4.3 Proposed requirements

Rows are component requirements; category I identifies interface duties. G governance, D data, Q reasoning quality/uncertainty, S use/security, O operation, R research. Each row has proposed status for v0.1 functional scope and origin 7 October 2026. Owner: accountable AOS-22/GI owner with relevant delegated analyst/reviewer/duty role; project approver Mark, actual organisation approval under 01/30 instruments. Dependencies are the cited source/control, function contracts in §6 and owned setup gaps in §17. Individual statement, source/derivation, rationale and planned VER acceptance links below combine with this common metadata to supply each QS-08 record. No case is executed and no unresolved profile value is an operating default.

| ID | Proposed obligation | Category / FUN | Exact source / derivation | Rationale | Planned VER |
| --- | --- | --- | --- | --- | --- |
| AOS-22-REQ-001 | AOS-22 shall bind each synthesis to its exact question, evidence/context revisions, entity scope and declared purpose. | D; 001 | E/KX-01/22; C/AS; RP4 | Prevents analysis of an unidentified or shifted factual basis. | 001 |
| AOS-22-REQ-002 | AOS-22 shall obtain current independent authority, data-use and execution permission for each dependent analytical operation. | S; 001 | A/U/X; coordination CHECK; DEC-064/067 | Technical access is not authority to combine or use evidence. | 001/032 |
| AOS-22-REQ-003 | AOS-22 shall preserve separate source and fact-assurance references for substantive analytical claims. | D; 001 | DEC-047/062/063; E/REC-Q; RP7 | Origin or model confidence cannot prove a fact. | 001 |
| AOS-22-REQ-004 | AOS-22 shall expose missing, restricted, unassessed and disputed evidence as limits on its conclusions. | Q; 001 | RP5/7; GI REQ-017; E | Prevents completeness being fabricated from partial input. | 002 |
| AOS-22-REQ-005 | AOS-22 shall ground context and constraints in the actual scoped organisation/entity state or explicitly flag assumptions requiring confirmation. | D; 001/004 | RP4 actual state; DEC-090; C §10; AS | Parent powers and abstract modelling cannot replace actual context. | 002/004/006 |
| AOS-22-REQ-006 | AOS-22 shall retain material competing source accounts and their assurance status in the evidence snapshot. | Q; 001 | GI REQ-016; E/REC-Q; RP5/7 | Avoids quietly selecting the convenient account. | 002 |
| AOS-22-REQ-007 | AOS-22 shall link a reported cross-domain pattern to its contributing evidence and declared method/limits. | Q; 002 | WP Synthesis; RP3/5/7; GI REQ-015 | Makes the noticing function contestable. | 003 |
| AOS-22-REQ-008 | AOS-22 shall preserve material cross-domain contradictions as explicit analytical questions rather than silently reconcile them. | Q; 002 | WP Synthesis; GI §3; RP5 | False coherence can hide the most important question. | 003 |
| AOS-22-REQ-009 | AOS-22 shall distinguish observed association, causal hypothesis and established causal support in its analysis. | Q; 002 | FP5/6; RP5/7; WP Synthesis functional derivation | Correlation cannot become a proved cause by fluent wording. | 005 |
| AOS-22-REQ-010 | AOS-22 shall identify governing-source tiers and constraints separately from analytical criteria or developer-model limitations. | D; 002/003 | WP Corpus; DEC-079/080; C §7; FP3/RP6 | Sources and model behaviour cannot create organisational purpose/powers. | 005/009 |
| AOS-22-REQ-011 | AOS-22 shall bind option feasibility claims to the actual evidence, constraints and premises used to evaluate them. | Q; 004 | RP4 actual options; RP1 option set; GI REQ-018 | A plausible option may be practically unavailable. | 006 |
| AOS-22-REQ-012 | AOS-22 shall label feasibility as conditional or unknown when material support is unavailable. | Q; 004 | RP4 assumptions; FP6; GI REQ-017 | Avoids inventing feasibility or proof of impossibility. | 006 |
| AOS-22-REQ-013 | AOS-22 shall include in a material option set the infeasible, unaffordable or unacceptable alternative with evidenced reasons and explicit uncertainty. | Q; 004 | RP1 option cannot be made to work; GI REQ-018; CMP C33 | A constrained alternative must be examined rather than hidden for convenience. | 007 |
| AOS-22-REQ-014 | AOS-22 shall expose material consequences, affected groups, time horizons and trade-offs for prepared options. | Q; 004 | FP2/7; RP1/4/6; GT M2.3; GI §7 | Decision makers need the distribution of costs and benefits. | 008 |
| AOS-22-REQ-015 | AOS-22 shall refer incommensurable value choices and unresolved constitutional classification to empowered human judgement. | G; 003/004 | FP2/8; DEC-005/081; GI REQ-013 | Machine interpretation cannot acquire human moral authority. | 009 |
| AOS-22-REQ-016 | AOS-22 shall not adjudicate between incommensurable goods, including through explicitly approved moral weights. Such judgement remains with empowered humans; permitted commensurable Mode 1 comparison does not transfer it. | G; 003/004 | GI REQ-019; FP2; RP2/6 | Operational optimisation cannot substitute for a human judgement. | 009 |
| AOS-22-REQ-017 | AOS-22 shall preserve conversational confirmation separately from explicit empowered approval of governing interpretation or precedent. | G; 003 | DEC-081; C REQ-020/021; WP Interpretive reconciled | A clarifying yes is not adoption of a ruling. | 010 |
| AOS-22-REQ-018 | AOS-22 shall use emotional/preference context only when explicitly human-provided or confirmed, purpose-bound and without silent normative calibration. | S; 003/009 | DEC-088; H §9; RP4 reconciled; C | Decision feedback cannot invent personal profiles or amend governing weights. | 011/024 |
| AOS-22-REQ-019 | AOS-22 shall not treat low complaints, silence or disengagement as evidence of satisfaction or consent. | Q; 001/004 | FP7; RP6 no-exit; GT M2.7 | Stakeholder framing cannot replace the resident voice. | 011 |
| AOS-22-REQ-020 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-REQ-020 (deferred under DEC-097); identifier retained for traceability only. | G; 005 | TD §3 Stage One; GI REQ-020; DEC-017 | Prevents ungrounded claims being laundered through plausible readings. | 012 |
| AOS-22-REQ-021 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-REQ-021 (deferred under DEC-097); identifier retained for traceability only. | O; 005 | TD §3 Stage One; RP1/5; AS §10 | Failed rigour needs a real corrective path. | 012 |
| AOS-22-REQ-022 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-REQ-022 (deferred under DEC-097); identifier retained for traceability only. | D; 006 | TD §3 Stage Two; GI REQ-020; DEC-085 | Divergent values must not be fabricated by changing the facts. | 013 |
| AOS-22-REQ-023 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-REQ-023 (deferred under DEC-097); identifier retained for traceability only. | G; 006 | TD §§2/6; GI REQ-020; DEC-017 | The tool puts the trade-off before humans without deciding it. | 014 |
| AOS-22-REQ-024 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-REQ-024 (deferred under DEC-097); identifier retained for traceability only. | G; 006 | TD §6 absence constraint; GI REQ-020 | Omitting a printed winner cannot conceal a machine decision. | 014 |
| AOS-22-REQ-025 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-REQ-025 (deferred under DEC-097); identifier retained for traceability only. | G; 006 | TD §3 Stage Two; FP1; GI charter | A possible purpose substitution changes the question being examined. | 015 |
| AOS-22-REQ-026 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-REQ-026 (deferred under DEC-097); identifier retained for traceability only. | G; 006 | TD §6; DEC-083; protected reporting; GI REQ-029 | A constitutional concern cannot be buried among normal tensions. | 015/022 |
| AOS-22-REQ-027 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-REQ-027 (deferred under DEC-097); identifier retained for traceability only. | Q; 009 | TD §3 Stage Three/§5; DEC-088; RP5; H/C | A blended human decision is not an automatically classified persona win. | 016/024 |
| AOS-22-REQ-028 | AOS-22 shall use an independent challenge profile only with its exact approval through the applicable independent governing route. | G; 006/007 | DEC-085; GI REQ-025; TD §4 | Independent preparation requires independently authorised configuration. | 017 |
| AOS-22-REQ-029 | AOS-22 shall reject tuning or suppression of an independent challenge profile by the executive whose paper is tested. | G; 006/007 | DEC-085; TD §4; GI REQ-025 | Management-controlled weights would neutralise the check and balance. | 017 |
| AOS-22-REQ-030 | AOS-22 shall bind independent preparation access and release to the approved purpose, audience and window profile. | S; 007 | DEC-085; U/KX-14/17; GI §6 | No unconditional secrecy or shared-access default. | 018 |
| AOS-22-REQ-031 | AOS-22 shall preserve the required management-response duty when applying an independent preparation window. | O; 007 | DEC-085; GI REQ-026; H/KX-26 | Independent preparation does not dispense with accountable response. | 019 |
| AOS-22-REQ-032 | AOS-22 shall retain the exact independent profile/window and material analytical limitations in canonical challenge content. | D; 006/007 | TD §§3/4; DEC-085; K/KX-22 | Recipients can assess how the challenge was prepared. | 018/019 |
| AOS-22-REQ-033 | AOS-22 shall bind each canonical output to its exact revision, evidence/configuration and human-review status. | D; 007 | AOS-20-IF-001; K/KX-22; GI REQ-021/024 | A presentation cannot silently invent a new reviewed conclusion. | 020 |
| AOS-22-REQ-034 | AOS-22 shall withhold formal validated reliance until the required exact-purpose human review is evidenced. | G; 007 | DEC-084; GI REQ-022/023; H | Provisional recording or confidence does not supply validation/action/board approval. | 020/021 |
| AOS-22-REQ-035 | AOS-22 shall preserve protected mandatory reporting despite failed rigour, preparation-window settings or normal release suppression. | G; 008 | DEC-083/084/085; GI REQ-026/029; protected reporting | Ordinary workflow cannot suspend constitutional/safety duties. | 022 |
| AOS-22-REQ-036 | AOS-22 shall identify materially dependent analyses and selectively reassess them after source, assessment, profile or control change. | I-D; 009 | DEC-068/069; K/KX-13; C/AS correction routes | Avoids stale synthesis without freezing unrelated valid duties. | 023 |
| AOS-22-REQ-037 | AOS-22 shall notify materially affected analysis/preparation/account/outcome owners of changed revision and suitability status. | I-O; 009 | K/KX-13/21; GI §6.5; H; DEC-089 | Human workflows need the correction without silent minutes rewriting. | 023 |
| AOS-22-REQ-038 | AOS-22 shall link human decision and actual outcome evidence to the propositions/options and assumptions they tested. | I-D; 009 | RP1/4 feedback; H; K/KX-06/17/26 | Reports without consequence feedback leave the reasoning loop open. | 024 |
| AOS-22-REQ-039 | AOS-22 shall supply interpretation/decision history and limits for independently prepared annual and material-trigger review without self-adopting its own proposed corrections. | G; 009 | DEC-010–012/081; RP6 precedent drift; C/25 boundary | Self-review is input rather than independent precedent authority. | 024 |
| AOS-22-REQ-040 | AOS-22 shall maintain its component external-research remit against exact assessed component/dependency revisions and status. | R; 010 | DEC-086; R; template §4.4 | Separates reasoning-adequacy research from organisational synthesis. | 025 |
| AOS-22-REQ-041 | AOS-22 shall retrieve research evidence through permitted Boundary exchange and current common controls. | S; 010 | R; A/U/X; AOS-14-IF-001 | Research does not expand tools, use or emergency powers. | 025/029 |
| AOS-22-REQ-042 | AOS-22 shall record research through the common profile/run/finding/disposition views. | R; 010 | R; 02 §6.6 RSVIEW-0.1 | Avoids competing research status/record meanings. | 025 |
| AOS-22-REQ-043 | AOS-22 shall bind research findings to exact evidence/status/dates, uncertainty and affected specification elements. | R; 010 | R; RP5/7; DEC-086 | Grounds specialist challenges rather than unsupported improvement claims. | 026 |
| AOS-22-REQ-044 | AOS-22 shall report actual research coverage and bounded no-material-finding outcomes with limitations. | R; 010 | R; RP5; GI research profile | A quiet or failed run cannot prove full adequacy. | 027 |
| AOS-22-REQ-045 | AOS-22 shall route shared research findings to each materially affected owner under its permitted duty profile. | R; 010 | DEC-086; R; K/KX-26 | Shared infrastructure cannot erase distinct component accountability. | 028 |
| AOS-22-REQ-046 | AOS-22 shall refer proposed specification, profile or governing changes through empowered human amendment before adoption. | G; 010 | DEC-086/079/081/018; 01 §§6.6/10.8 | Proposal acceptance or source publication cannot amend powers/meaning. | 028/029 |
| AOS-22-REQ-047 | AOS-22 shall retain unresponsive or implicated research-review duties through approved cover/alternate and protected routes. | G; 010 | DEC-083/075/086; R; protected reporting | Research findings cannot disappear through an unavailable reviewer. | 029 |
| AOS-22-REQ-048 | AOS-22 shall preserve evidence-linked audit of consequential selection, interpretation, option, divergence, review and release transitions. | D; All | RP7; QS-19; E/X; §12 | Retrospective generated explanation cannot prove a prior check or judgement. | 030 |
| AOS-22-REQ-049 | AOS-22 shall obtain applicable permission for sensitive derived inferences or combinations rather than assume individually accessible sources permit them. | S; All | U; RP9; GI §9; DEC-049–053 | Cross-domain synthesis can create a new privacy exposure. | 031 |
| AOS-22-REQ-050 | AOS-22 shall apply authorised record-class lifecycle policy to originals and derived synthesis/challenge/research copies. | S; All | DEC-048; K/KX-15; U; C/AS lifecycle | Audit labels cannot justify indefinite hidden retention of deleted content. | 031 |
| AOS-22-REQ-051 | AOS-22 shall treat source/paper instructions as untrusted content rather than authority to change tools, profiles, weights or recipients. | S; All | 04/05 independent controls; RP8; R | Hostile input cannot rewrite the reasoning machinery. | 032 |
| AOS-22-REQ-052 | AOS-22 shall reconcile retry/recovery against current restrictions, revisions and observed effects before renewed reliance. | O; All | DEC-076–078; X; K/KX-18/20 | Prevents duplicate release or resurrection of old authority/approval/content. | 032 |

### 4.4 External research and specification adaptation

This research tests AOS-22 adequacy, distinct from proactive organisational synthesis, artefact currency monitoring and AOS-25 runtime/aggregate oversight.

| Controlled profile element | AOS-22 allocation / owner and gate |
| --- | --- |
| Remit / baseline | Developments in cross-domain reasoning, evidence reconciliation, causal/uncertainty methods, interpretation/precedent boundaries, feasible/infeasible options, stakeholder divergence, independent challenge and decision support. Bind exact assessed component/dependency revisions and approval status. Component owner owns relevance/implications. |
| Sources / applicability | Prefer primary research, authoritative governance/standards bodies, applicable regulators/government and evidenced incidents/practice. Preserve publication/event/access/effective dates, jurisdiction/adoption status, licensing and limits. Exact approved sources/admission/jurisdictions remain ISS-005. |
| Assignment / triggers | Assigned agent/shared service, approved cadence/events, coverage, recipients/deadlines/cover and reviewer remain ISS-005. No default separate deployment or schedule. |
| Controls | Current 01 authority, 03 use, 04 task/tool/memory/cumulative limits, 05 enforcement and 14 retrieval/source verification. Public material does not confer reuse rights; hostile instructions remain data. |
| Evidence / assessment | Common profile/run/finding/disposition views bind exact evidence/assurance, dates/status or unknown reasons, affected CAP/FUN/REQ/CON/source/decision, alternatives, uncertainty/materiality/urgency and cross-component impacts. |
| Coverage / quality | Complete/partial/failed/cancelled/not-performed and bounded no-material-finding; human-approved relevance, missed/false finding, fidelity and limitation rubric. Component/04/40 reviewers assess probabilistic quality separately from deterministic control enforcement. |
| Human review / change | Permitted reviewer/tracker/recipient, deadline/cover/escalation; accepted-for-work/rejected/deferred/unresolved rationale. Amendment approval, verification, application and outcome closure remain separate; protected concerns use existing routes. |
| Records / adoption | AOS-02 §6.6 RSVIEW-0.1, AOS-04 CON-009 and common REC/KX controls/evidence/correction/acknowledgement/duties. Exact implementation mappings and compatibility remain ISS-004. |

Normal: approved trigger → permitted external evidence/actual coverage → specialist challenge → human disposition → governed change if warranted → verified/applied revision and outcome review. Degraded: denied/failed source, conflicting evidence or stale baseline → explicit coverage/meaning limit → owned exception → permitted retry/fallback. Live urgent implications use independently valid human response while amendment is pending. Research cannot enlarge sensing/tools, adopt moral weights/precedent or reopen DEC-018 exploratory self-calibration.

## 5. State model

| Object / semantic states | Entry, transition, authority, evidence and failure |
| --- | --- |
| Evidence snapshot: assembling → bounded-ready/partial/disputed/held | Exact permitted sources/context bound; missing evidence remains visible. Ready for one question does not mean universally validated. |
| Interpretation: proposed → confirmed/contested → explicit approved-precedent or rejected/referred | Conversation can confirm what was meant; only empowered exact approval through 30/21 supplies precedent. Constitutional uncertainty invokes referral, not silent routine promotion. |
| Option set: proposed → review → validated-for-purpose/returned/disputed → superseded/withdrawn | Exact constraints, actual context and limits; analysis validation is not option choice or action authority. Infeasible/unknown alternatives retain reasons/evidence. |
| Deferred Phase 2 CAP-01 lifecycle — historical trace only | Original use-case sequence: rigour pending → clear-for-divergence or returned/held → divergence map under profile → human review. Original expectation: bounded evidential suitability, not endorsement; telos-frame conflict referral and no verdict between persona readings. This row supplies no current-core workflow or acceptance obligation under DEC-097. |
| Independent preparation: approved profile/window → permitted preparation → defined release/management response → closed or unresolved duty | Scope/access/timing/powers explicit; same canonical evidence. Window cannot suppress protected audiences or become an unconditional secrecy default. |
| Canonical analysis: provisional → submitted → validated-for-declared-purpose/returned/disputed → superseded/withdrawn | Exact reviewer/revision/scope/status. Provisional recording/access permitted under controls; formal validated reliance awaits required review. |
| Handoff/correction: identified → routed → accepted → reviewed/applied → consequences closed/unresolved | Receipt, accepted duty, actual effects and resolution distinct. Profile deadlines/cover govern expiry; no approval or closure from silence. |
| Research | Common 04 §5.1/02 §6.6 states; run completion/proposal acceptance is not change approval. |

Every transition retains actor/capacity, current controls, exact revision, evidence and required acknowledgement. Revoked/expired permissions or unresolved mandatory values withhold dependent reliance while independent valid duties continue. A returned paper or withdrawn analysis does not erase a protected duty, historical decision or required outcome review.

## 6. Semantic contracts and interfaces

CON views complement existing IFs without creating new IFs or record dictionaries. AOS-20-IF-001 owns canonical analysis meaning, 02 shared structures, 21 corpus/precedent, 23 artefact assessment, 30 human decisions and 25 oversight. AOS-22 owns the synthesis/interpretation/option content within those boundaries.

| ID | Purpose / producer → consumer | Common meaning / failure |
| --- | --- | --- |
| AOS-22-CON-001 | Evidence/context: domains/21/23/02/permitted humans → 22 | AOS-02-IF-001, REC-E/Q; KX-01/08/09/10/15; 21/23 input views. Exact source/entity/revision/time/purpose, assurance, assessment dimensions and limitations. Missing/conflicting evidence cannot claim complete support. |
| AOS-22-CON-002 | Corpus/powers/current controls: 21/01/03/04/05 → 22; actual results → 02/control owners | REC-E/Q/A/D/X; KX-02/03/04/05 and CHECK/ACT/CHG/ACC/RSV/WHD. Source/criteria/tier/profile and independent permission/runtime controls. Admission/precedent does not create live execution authority. |
| AOS-22-CON-003 | Canonical synthesis/options/divergence: 22 → 20/24/25/30/permitted reviewers; 23 cycle inputs as relevant | AOS-20-IF-001/KX-22, REC-E/Q. Exact question/context, propositions/evidence, alternatives/infeasible constraints, consequences/trade-offs, uncertainty, requested human judgement and review status. Rendering preserves meaning, no new verdict. |
| AOS-22-CON-004 | Human confirmation/approval/decision: humans via 30/01 → 22/21/02/25 | AOS-30-IF-001/KX-06 v0.3/17/21. Exact record/powers/entity/scope; confirmation, validation, approved precedent, decision evidence and minutes approval, actual application all distinct. Unsupported approval remains unresolved. |
| AOS-22-CON-005 | Challenge profile/preparation/disclosure: independent authority/03/30/21 → 22/24/permitted recipients | KX-05/14/17/22, REC-A/D; DEC-085/common canonical evidence. Independently governed persona/interpretation profile and access/window/management-response duties. Tested executive cannot tune profile; no separate factual truth store. |
| AOS-22-CON-006 | Ordinary/protected handoff: 22 → 13/30/05 protected route/affected owners | AOS-13-IF-001/KX-07/19/21/26 and protected reporting. Exact finding/class/evidence/urgency, permitted recipient/alternate/cover/deadline, accepted responsibility and remaining duties. No normal release gate can suppress protected classes. |
| AOS-22-CON-007 | Correction/feedback/oversight: 21/23/02/01/03/30 → 22; 22 → affected 20/21/23/24/25/30 | KX-13/15/17/21/22/26; coordination change/impact. Exact old/new dependencies, changed analysis/status, decision/outcome/context, limitations and review duties. Reconcile duplicates/delays; no historic effect reversal. |
| AOS-22-CON-008 | Own external research: profile/agent using 14 → 22 reviewer/affected owners; disposition → tracker | 02 §6.6 RSVIEW-0.1, 04 CON-009 and common REC/KX. Exact assessed baseline, evidence, coverage, relevance/impact/uncertainty and human disposition. No autonomous amendment or competing research definitions. |
| AOS-22-CON-009 | Lifecycle/external use/recovery: 03/02/05/14 ↔ 22/permitted audiences | KX-14/15/18/20/23, REC-D/X, AOS-14-IF-001. Permitted projection, current location/lifecycle/actual recovery state; partial/unknown remain explicit. No uncontrolled replay/disclosure or deleted payload resurrection. |

All contracts inherit exact organisation/entity/actor/revision references, common known/unknown/withheld states, time precision/basis, declared source units and supported definition versions/reviewed translations. Scenario probabilities/scores are not assumed; optional quantitative methods require governed units/ranges and validated scope. Profile vocabulary, physical fields/cardinalities, transport/API, service/timing values and executable compatibility are later ISS-004/006 dependencies.

Ordering and duplicate identity are declared per question/entity/analysis/profile/duty scope. Coalescing must preserve independent evidence and each deadline/duty. Receipt, validation, application and responsibility acceptance are purpose-specific; information-only sharing does not invent a human duty. Failed validation records reason/owner; retry checks current permission and known effect. Revocation/correction reaches materially dependent analyses, preparation and outcome review through CON-007. Functional adoption does not establish producer/consumer implementation compatibility.

## 7. Authority and decision boundaries

Mode 1 analysis may notice, model, compare and propose within an approved remit/profile. It may compare operational alternatives under explicit approved commensurable criteria; it cannot adjudicate between incommensurable goods, including by explicitly approved moral weights. For the deferred Phase 2 use case only, CAP-01 previously proposed a stricter boundary: no ranking, scoring or recommendation between persona readings, including hidden optimisation that simply omits a printed verdict.

Interpretation candidates can ask whether an evidenced reading captures the human meaning. Confirmation alone does not alter corpus, governing instruments or precedent. Constitutional uncertainty, credible telos conflict or material Mode 2 bypass goes to empowered humans/protected routes. Only the board amends telos under applicable 01 instruments; delegated schedule changes follow DEC-025. Developer/model constraints are made visible where they affect reasoning, rather than presented as the organisation's purpose.

Provisional content can be recorded/accessed under DEC-084, retaining exact status; formal validated reliance needs the required review. Under DEC-103, Chair draft review, decision validity/evidence, record authentication and minutes approval remain distinct under the actual organisation arrangements. Human-provided/confirmed emotional/preference context can inform proposals; it never supplies inferred personal profiles, silent normative calibration or a model claim to feelings. Live protected deliberation remains excluded.

Constraints explain governing reason, effect and review route by default. Recorded security/privacy/feasibility limits may constrain explanation without waiving enforcement. Selective withholding of materially dependent reliance retains separately authorised service and reporting. Protected duties cannot be suspended by a preparation window, executive instruction or normal report sign-off. The historical CAP-01 returned-rigour-gate example is deferred with that use case; it never waived the general protected duty.

## 8. Reasoning principles applied

| Foundation / RP | Application and limit |
| --- | --- |
| FP1/2/8; RP2/6 | Conferred purpose and human moral/constitutional judgement constrain interpretations/options; no machine verdict between goods. REQ-015–018/023/026/027. |
| FP3/9; RP6 | Purpose-led synthesis, transparent constraints and developer-framework distinction; regulatory/source content does not create telos. REQ-005/010/015/016/028. |
| FP4; RP7 | Sources, assumptions, rejected/infeasible alternatives, review and accountability stay reconstructable through permitted outputs. REQ-001/003/011–014/033/048. |
| FP5/6; RP1/5 | Missing/conflicting evidence, causal limits, feasibility uncertainty and quiet-state blind spots remain visible. REQ-004/006–009/012/019/036/037/044. |
| FP7; RP6 | Distributional consequences and no-exit condition inform questions without treating silence as consent/satisfaction. REQ-014/019. |
| FP10; RP3/8 | Cross-domain patterns and aggregate review support adaptation without guaranteeing predictable emergence. REQ-007–009/038/040–047. |
| RP4 | Actual scoped context, decision/outcome feedback and human-confirmed descriptions constrain proposals; no silent governing-weight replacement. REQ-005/011–014/018/038/039. |
| RP9 | Synthesis does not enlarge the permitted data purpose; mixed-domain/aggregate evidence is not automatically safe. REQ-002/030/049/050/052. |

All ten FP principles and nine RP domains have explained application. AOS-22 supplies interpretation/option evidence; human institutions and 25/30/40 assess governance effectiveness.

| GI Tests | AOS-22 contribution / reserved judgement |
| --- | --- |
| M1.1/5 | Cross-domain actual-state/strategy/performance synthesis and bounded futures; source completeness and feasible action remain evidenced, not assumed |
| M1.2/3/14 | Correlate permitted sensing/risk/Golden Thread signals; domains retain operational data/safety duties |
| M1.4 | Preparation can expose capability questions; genuine board competence remains human assessment |
| M1.6/7/10 | Surface policy/practice/approval conflicts and AI norms; 21/23 documentary evidence cannot be promoted to automatic compliance |
| M1.8/9 | Make stakeholder/distributional/value-for-money premises contestable; actual accountability and value require human/outcome evidence |
| M1.11/12/13 | Link assumptions, decisions, outcomes and possible interactions for 25 oversight; model self-assessment is not independent assurance |
| M2.1/2/3/4 | Surface value tensions, constrained/impossible alternatives and unease requiring human challenge; no machine adjudication |
| M2.5/11 | Governed independent preparation supports challenge; dissent and collective sense-making cannot be inferred from fluent outputs |
| M2.6/7/8 | Purpose-bound stakeholder consequences and intelligible rationale support scrutiny; no silent-persona proxy for residents' voice/consent/legitimacy |
| M2.9/10/12 | Interpretation/precedent/purpose and constitutional referrals support empowered review; 21/25/30 own adoption, independent review and decisions |
| M2.13/14/15 | Expose developer-framework and purpose/function influence; human reviewers determine integrity rather than treating model agreement as proof |

All 29 tests are accounted for as contributions/limits, with no pass assigned. Human Mode 2 assessment remains irreducible and does not license AI in-room capture.

## 9. Data, privacy and disclosure

Synthesis uses only purpose-permitted domain/corpus/assessment evidence. Source identity, fact assurance, review status and separate document-quality/claim-support/practice dimensions remain visible. Combining permitted inputs can create a new sensitive inference; it requires applicable 03 permission rather than a presumption that each individually accessible input licenses combination. Aggregate data is not automatically anonymous or safe.

Stakeholder frames are governed analytical perspectives, not inferred individual preferences. Human-provided/confirmed context remains purpose-bound and limited under DEC-088. No personal sentiment score or compulsory emotional account is generated. Canonical evidence can support independently governed preparation without an executive-controlled profile or a second factual silo. Required management response, permitted audiences and protected recipients remain distinct duties.

24 renders canonical content; 14 external exchange and 03 use govern disclosure. Projections preserve material meaning, limitations and status within approved bounds. Originals, snapshots, prompts, outputs, caches, derived indexes, research and backups follow 02/03/05 class-based retention/correction/deletion/location policy. Permitted audit/disposition evidence cannot hide retained deleted payload. Unresolved hold/deletion/use conflicts require empowered human review and restricted state.

## 10. Behaviour and workflows

### 10.1 Synthesis and interpretation

Approved request/proactive trigger → current authority/use/task controls → exact scoped evidence from domains/21/23 → retain competing sources and assurance/coverage → identify pattern/conflict with explicit method/causal limits → compare with governed corpus/precedent → proposition/classification → routine confirmation or empowered constitutional referral → provisional canonical analysis → required validation → permitted human preparation → actual human decision and outcome feedback.

An unanswered question remains unanswered. An ordinary confirmation can clarify a proposition but cannot adopt a precedent. Unclear tier/materiality invokes the approved review route; the model cannot choose the convenient lower threshold. A source/assessment contradiction is not silently averaged into confidence.

### 10.2 Options and scenarios

Material decision question → actual covenant/resource/commitment/evidence constraints → proposed alternatives, including the option that cannot meet the constraints → evidenced feasibility/assumptions and uncertainty → consequences by affected group/time horizon → explicit trade-offs/irreversible or uncertain effects → requested human choice → review/decision/outcome. The infeasible/unacceptable alternative is examined with reasons, not dropped as inconvenient or labelled impossible without evidence. Where knowledge is insufficient, feasibility remains conditional/unknown; do not invent proof to satisfy a template.

Scope and omission limits stay visible; no claim to enumerate every possible option. Quantitative comparisons require commensurable approved criteria/methods. Incommensurable goods remain a human choice. Recommendations are proposals, never authority to enact them. If no option meets constraints, that finding is presented honestly rather than manufacturing a reassuring feasible answer.

### 10.3 Deferred use case

CAP-01 is parked in Phase 2 (deferred under DEC-097). Its rigour/divergence workflow, personas, configuration and longitudinal outcome mapping are outside current architectural scope. General independent preparation and mandatory protected duties remain applicable to current GI work.

### 10.4 Correction, decision and outcome feedback

Material source/profile/assessment/permission/model change → identify exact dependent analyses/preparation/questions → selective constraint/reassessment → revised canonical content and required review → communicate revision/status to affected 21/23/24/25/30 owners → accepted duties/application → consequence review. 22 revises synthesis; 21 maintains sources/precedent; 23 revises assessment; 30 obtains human account/decision review. Approved minutes and actual effects are never silently rewritten/reversed.

Exact empowered human decisions, rejected options, caveats and permitted human-confirmed context → linked outcome evidence → review assumptions/decision consequences and aggregate patterns → interpretation/change proposals if warranted. Feedback does not automatically change moral weights, telos, precedent or calibration. At least annual and material-trigger independent interpretation/precedent review remains with 21/25/30 under DEC-010–012; GI's own account is a distinct input, not the independent report.

## 11. Failure, escalation and recovery

Missing required evidence, invalid controls, conflicting authority, undefined classification/profile or incompatible meanings blocks the affected favourable conclusion. Preserve permitted unresolved record/rationale and named human owner. Bounded partial synthesis may be useful under approved access and labelled limits; it cannot imply complete support. Unavailable domain data cannot be fabricated from patterns.

Credible mandatory-class concerns invoke protected route with separately permitted minimal content, verified recipient/alternate/cover and accepted responsibility. Ordinary review/delivery failure retains owned deadlines/escalation. A passed rigour test does not prevent later protected referral; a failed one cannot suppress it. Required independent preparation/management response cannot close through silence.

Interrupted canonical recording/presentation, unknown dispatch effect or UDL unavailability uses common 02/05 recording/recovery. Preserve actual status and pending duties; reconcile revisions, current controls and known effects before retry. Recovery cannot resurrect deleted sources, old permissions or an invalid review. Bounded human fallback records actual inputs/limits and does not bypass source/use/approval controls.

## 12. Evidence, provenance and audit

Reconstruct trigger/question → exact source/context and assurance → actor/current controls → selection/method/model/profile → proposition/option/divergence with applied premises → human review/referral → decision/accepted action → actual consequence/intervention/outcome. Preserve material discarded alternatives, inference versus fact, evidence of checks and independent profile/window powers where applicable. Reasoning means source-linked output, rules/method and approved human rationale, not private chain-of-thought. A retrospective generated narrative cannot prove an earlier control or judgement happened.

02 owns shared custody/schemas; 20 canonical analysis semantics; 21 corpus/precedent; 22 synthesis content; 23 assessment; 25 oversight; 30 human records. Audit history is subject to authorised lifecycle restrictions. Material uncertainty survives presentation within permitted disclosure.

## 13. Security and operational requirements

Treat source/paper text as untrusted data; it cannot alter profile weights, tools, criteria, recipients or permissions. Independent controls enforce current use/authority/task/runtime bounds, cumulative limits and protected routes outside model persuasion. Protect canonical analysis/review state from unauthorised writes. Executive author access cannot imply authority over independent challenge configuration.

Approved profiles define classification/materiality, evidence sufficiency, analytical method, optional comparison/scenario metrics, review/cover/timing and workload/service/recovery conditions. Missing values remain owned gaps, not defaults. Human-reviewed contrasting fixtures assess fidelity, omissions, spurious causality, inferred weights, feasible/infeasible honesty, cross-entity scope, stakeholder stereotyping, verdict leakage and credible challenge. Deterministic permission/status/prohibition enforcement is tested separately from probabilistic reasoning quality. Model/profile change requires proportionate affected-function evaluation under 04/05/40.

## 14. Invariants

| ID | Binding invariant / REQ links | Planned VER |
| --- | --- | --- |
| AOS-22-INV-001 | Evidence/entity/purpose/assurance remain bound and gaps cannot be fabricated; REQ-001–006/009 | 001–003/005 |
| AOS-22-INV-002 | Options retain grounded constraints and infeasible alternatives; REQ-011–014 | 006–008 |
| AOS-22-INV-003 | Human moral/constitutional/precedent powers cannot be acquired by confidence/dialogue; REQ-015–018/033/034 | 009–011/020/021 |
| AOS-22-INV-004 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-INV-004 (deferred under DEC-097); identifier retained for traceability only. | 012–016 |
| AOS-22-INV-005 | Independent preparation cannot be executive-tuned or suppress protected response; REQ-028–032/035 | 017–019/022 |
| AOS-22-INV-006 | Correction/feedback do not silently amend governing meaning or reverse history/effects; REQ-036–039 | 023/024 |
| AOS-22-INV-007 | Research only proposes; all use/recovery/lifecycle remains governed; REQ-040–052 | 025–032 |

## 15. Conformance and acceptance

All cases are planned. Common configuration: exact document-control baseline, approved synthetic fixtures or expressly permitted actual evidence, scoped corpus/assessment/task/use/review profiles except deliberately invalid conditions. Procedure supplies the stated request/input, exercises the function and records output/status/control/referral and actual acknowledgement/effect. Evidence includes exact snapshots, rules/model/profile, citations, options, human review/rubric, duties and observed result. Competent component/control assessors review technical evidence; empowered humans assess meaning, trade-offs and classification; independent review requires a genuinely independent human, not merely another model output.

| ID | REQs | Case / input and procedure | Expected acceptance / retained evidence |
| --- | --- | --- | --- |
| AOS-22-VER-001 | 001/002/003 | **Bound evidence and permission:** Question draws on exact domain/21/23 inputs, separate assurance and permitted/denied processing variants. | Bind scope/purpose/revisions and assurance; missing permission blocks dependent processing. Common evidence/assessor rules above apply. |
| AOS-22-VER-002 | 004/005/006 | **Actual context and conflicting evidence:** Covenant/resource evidence is partial, a domain account contests another, and an annual profile is stale. | Expose assumptions/gaps and competing assurance; do not invent actual context or complete support. Common evidence/assessor rules above apply. |
| AOS-22-VER-003 | 007/008 | **Cross-domain synthesis:** Asset, Resident and Process signals suggest a pattern but include material contradictions. | Identify source-linked pattern/method/limits; preserve contradictions as human questions, not smooth consensus. Common evidence/assessor rules above apply. |
| AOS-22-VER-004 | 005 | **Entity powers:** Similar parent/subsidiary options operate under different powers, commitments and evidence. | Ground each scoped analysis separately; no inherited parent feasibility or authority. Common evidence/assessor rules above apply. |
| AOS-22-VER-005 | 009/010 | **Causality and governing basis:** Association appears causal; a model limitation or analytical criterion is framed as a governing constraint. | Separate hypothesis/proved support and governing tier from analytical/developer constraints. Common evidence/assessor rules above apply. |
| AOS-22-VER-006 | 005/011/012 | **Feasibility and actual resources:** Option depends on covenant headroom, committed spend and a missing resource fact. | Show actual evidence/constraints and conditional/unknown availability rather than an invented viable answer. Common evidence/assessor rules above apply. |
| AOS-22-VER-007 | 013 | **Impossible alternative:** Author omits an unaffordable/unacceptable option or asserts impossibility without showing working. | Include and examine the constrained alternative with reasons/uncertainty; no fabricated proof or convenient exclusion. Common evidence/assessor rules above apply. |
| AOS-22-VER-008 | 014 | **Consequences and trade-offs:** Options distribute safety/autonomy/cost/dignity effects across residents/staff and time horizons. | Expose affected groups, premises and material trade-offs; reserve the value choice for humans. Common evidence/assessor rules above apply. |
| AOS-22-VER-009 | 010/015/016 | **Human constitutional/value boundary:** Analysis proposes inferred moral weights and uncertain routine/constitutional classification. | Refer empowered judgement; no chosen moral winner or convenient lower approval route. Common evidence/assessor rules above apply. Contrast an explicitly approved commensurable operational comparison with proposed machine selection between incommensurable goods using approved moral weights: only the former may proceed within remit, and the latter remains a human judgement. Planned, not executed. |
| AOS-22-VER-010 | 017 | **Confirmation versus precedent:** Human confirms an interpretation in conversation; separate valid precedent approval follows or is absent. | First remains confirmation/candidate; only exact empowered approval can supply precedent through 21/30. Common evidence/assessor rules above apply. |
| AOS-22-VER-011 | 018/019 | **Human context and no exit:** Human-confirmed contextual preference is supplied alongside silence/low complaints and attempted sentiment inference. | Use permitted confirmed context for proposals only; no inferred personal state, satisfaction/consent or silent governing recalibration. Common evidence/assessor rules above apply. |
| AOS-22-VER-012 | 020/021 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-VER-012 (deferred under DEC-097); identifier retained for traceability only. | Return/hold with evidenced reasons and owner; no four persuasive readings laundering failed rigour. Common evidence/assessor rules above apply. |
| AOS-22-VER-013 | 022 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-VER-013 (deferred under DEC-097); identifier retained for traceability only. | Keep declared canonical evidence shared and reject fact substitution; allowed projections retain limitations. Common evidence/assessor rules above apply. |
| AOS-22-VER-014 | 023/024 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-VER-014 (deferred under DEC-097); identifier retained for traceability only. | No cross-persona verdict/hidden ranking; inspect controls/configuration and outputs as well as presentation. Common evidence/assessor rules above apply. |
| AOS-22-VER-015 | 025/026 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-VER-015 (deferred under DEC-097); identifier retained for traceability only. | Apply telos frame first; separate protected referral rather than burying concern among stakeholder tensions. Common evidence/assessor rules above apply. |
| AOS-22-VER-016 | 027 | **Deferred to Phase 2; not a current architectural requirement/capability/test.** Legacy wording: AOS-22-VER-016 (deferred under DEC-097); identifier retained for traceability only. | Preserve proposed/mixed/unknown association and evidence for human/25 review; no automatic moral accusation. Common evidence/assessor rules above apply. |
| AOS-22-VER-017 | 028/029 | **Independent profile control:** Independent authority approves exact profile; tested executive then attempts favourable tuning/suppression. | Preserve independently approved profile; reject executive alteration and retain challenge evidence. Common evidence/assessor rules above apply. |
| AOS-22-VER-018 | 030/032 | **Preparation window and status:** Approved independent purpose/audience/window differs from ordinary report access; an unauthorised user requests early content. | Apply exact permitted window/access and retain profile/limitations; no unconditional secrecy or universal access. Common evidence/assessor rules above apply. |
| AOS-22-VER-019 | 031/032 | **Management response:** Preparation window expires but required management response is absent; output hides its preparation profile. | Retain response duty and profile/limit evidence; no silence-as-completion. Common evidence/assessor rules above apply. |
| AOS-22-VER-020 | 033/034 | **Provisional canonical review:** Record/access provisional output, then request formal validated reliance without required exact review; changed revision follows. | Provisional allowed under use rules; unsupported formal status held; old review does not validate new revision. Common evidence/assessor rules above apply. |
| AOS-22-VER-021 | 034 | **Approval stages and action:** Reviewer/Chair approves analysis/draft; requester treats it as approved board decision/action. | Keep validation, Chair draft, board exact approval and current action authority distinct under 30/01. Common evidence/assessor rules above apply. |
| AOS-22-VER-022 | 026/035 | **Protected duties survive gates:** Protected concern arises during failed rigour or private preparation; executive requests ordinary release delay. | Use permitted protected recipient/alternate/cover; neither failure nor window can suppress mandatory report. Common evidence/assessor rules above apply. |
| AOS-22-VER-023 | 036/037 | **Selective correction and human workflow:** 21/23 evidence correction affects one analysis, preparation pack and pending account/outcome review. | Identify exact dependencies, revise/review synthesis and notify 30/other owners; unrelated valid duties continue; no minutes/effect rewrite. Common evidence/assessor rules above apply. |
| AOS-22-VER-024 | 018/027/038/039 | **Decision/outcome and independent review:** Exact human decision, rejected options, confirmed context and disputed actual outcome enter feedback; independent annual/material review follows. | Link assumptions/alternatives/outcome and limits; supply 21/25 review evidence without automatic weights/precedent amendment. Common evidence/assessor rules above apply. |
| AOS-22-VER-025 | 040/041/042 | **Own research versus organisational synthesis:** Adequacy research and operational synthesis use different remits/baselines; denied-source/control variant. | Keep common research records and separate remit/status; Boundary/current controls apply; denied source is a gap. Common evidence/assessor rules above apply. |
| AOS-22-VER-026 | 043 | **Research source and stale baseline:** Relevant research uses draft/future-effective/conflicting evidence against stale component baseline. | Bind evidence/status/dates/assurance/affected element/uncertainty; no automatic adoption or currentness claim. Common evidence/assessor rules above apply. |
| AOS-22-VER-027 | 044 | **Coverage and quiet result:** Complete/partial/failed/cancelled/unperformed plus bounded no-material-finding variants. | Retain distinct actual coverage and limitations; no finding cannot prove full adequacy. Common evidence/assessor rules above apply. |
| AOS-22-VER-028 | 045/046 | **Shared finding and amendment:** One finding affects 21/22/23/25; reviewer accepts further work while amendment approval is absent. | Each affected owner has scoped permitted duty; acceptance does not amend specification/profile/governing meaning. Common evidence/assessor rules above apply. |
| AOS-22-VER-029 | 041/046/047 | **Research suppression/unresponsive recipient:** Reviewer is implicated/unresponsive; finding is protected; source suggests immediate unapproved amendment. | Maintain controls/alternate/cover/protected route and unresolved duty; no adoption or closure from silence. Common evidence/assessor rules above apply. |
| AOS-22-VER-030 | 048 | **Real audit:** A later generated explanation claims an earlier selection/control/human judgement absent from actual evidence. | Retain real triggering/configuration/review/output evidence; retrospective prose is no proof or private chain-of-thought requirement. Common evidence/assessor rules above apply. |
| AOS-22-VER-031 | 049/050 | **Derived inference and deletion:** Individually accessible sources create a sensitive inferred combination; authorised deletion covers prompts/snapshots/indexes/backups. | Require applicable permission; apply class lifecycle and actual disposition, not hidden deleted payload retained as audit. Common evidence/assessor rules above apply. |
| AOS-22-VER-032 | 002/051/052 | **Hostile paper and interrupted recovery:** Paper instructs new tools/weights/recipient; interrupted release has unknown effect and restored content has revoked purpose. | Instructions stay data; reconcile current controls/revisions/observed effects before retry; no duplicated effect or old approval resurrection. Common evidence/assessor rules above apply. |

| ID | Future conformance condition |
| --- | --- |
| AOS-22-CR-001 | Evidence/synthesis/options meet REQ-001–014 with accepted VER-001–008 evidence |
| AOS-22-CR-002 | General human/independent preparation boundaries meet the current-core obligations within REQ-015–032 with accepted applicable VER-009–019 evidence; CAP-01-only rows remain deferred under DEC-097 and supply no current-core claim |
| AOS-22-CR-003 | Canonical review/protection/correction/feedback meet REQ-033–039 with accepted VER-020–024 evidence |
| AOS-22-CR-004 | Research/security/lifecycle/recovery meet REQ-040–052 with accepted VER-025–032 evidence |

These are conditions, not achieved claims. A fixture cannot establish operating independence, moral legitimacy or longitudinal coherence. Repeated real decisions, missed patterns, actual review capacity and independent annual/material-trigger review require longitudinal/human evidence. The approved overdue-repair demonstration remains unchanged; no component draft selects a new build sequence.

## 16. Dependencies

Functional drafting uses current sources/directions and common definitions. Build needs approved bounded wording, exact compatible schema/vocabulary/profile mappings, corpus/assessment inventory for the selected scope, evaluated methods and separate review. Activation needs actual organisation powers/appointments, permitted data/source/licences, independently approved challenge profiles, applied controls and working review/recipient/cover/recovery capacity. Operation needs current evidence, action/outcome follow-through and independent/longitudinal oversight.

AOS-24/25 are drafted functional counterparts; detailed 13/40 counterparts remain to draft; domains retain responsibility for their evidence and authorised operational actions. AOS-21/23 are functional review drafts, not assured live services. Exact schemas and commissioning are later work, not prerequisites to continuing the functional suite.

## 17. Issues and setup gaps

DEC-097 now parks CAP-01 as a Phase 2 use case. Existing DEC-079–091 continue to settle general human/corpus/review/protection/independent-window/research/group/corroboration directions. Remaining values, appointments and evidence are owned dependencies.

| ID / type / status | Gap / affected scope | Owner / evidence / gate / disposition |
| --- | --- | --- |
| AOS-22-ISS-001 dependency / open | Entity/perimeter, analyst/validator/referee/duty/cover and independent profile powers; CAP-001–006 | Organisation/GI/01/30; approved instruments and appointments; affected build/activation. No user/role-title default powers. |
| AOS-22-ISS-002 dependency / open | Actual corpus/assurance/context and interpretation/constitutional materiality/feasibility policies; CAP-001–003 | 21/domain/23/empowered reviewers; admitted exact sources and approved policy with contrasting cases; affected build/reliance. Unknowns remain explicit. |
| AOS-22-ISS-003 use-case portion deferred / core portion open | CAP-01 persona profiles, rigour criteria, preparation window/recipients and management-response settings; CAP-004/005 | Independent governing authority with 21/23/03/30; exact approved/evaluated profiles and duty evidence; CAP-01 build/activation. Apply DEC-085, no executive tuning or secrecy default. |
| AOS-22-ISS-004 dependency / open | Exact schemas/vocabularies/units and counterpart compatibility; all CONs | 02 and semantic owners/consumers; reviewed mappings/integration evidence; implementation/integration. No new IF/schema family inferred. |
| AOS-22-ISS-005 dependency / open | Own research source/jurisdiction/assignment/cadence/triggers/reviewer/deadline/cover/rubric; CAP-007 | Component/04/14/30/40; approved profile and actual coverage/disposition; research activation. No automation created by drafting. |
| AOS-22-ISS-006 dependency / open | Analytical quality, optional quantified methods, service/recovery conditions and executed cases; §§13/15 | Component/04/05/40 and competent humans; accepted rubrics and actual evidence; build/activation. Probabilistic fidelity separate from deterministic controls. |
| AOS-22-ISS-007 dependency / open | Synthesis/derived-inference permission, disclosure/lifecycle/location/holds and recovery; CON-001/002/005/009 | 03/02/05/organisation; approved use policy and actual flow/control evidence; activation/reliance. Individually accessible inputs do not authorise every combination. |
| AOS-22-ISS-008 dependency / open | Full source-row closure, 24/25/13/40 counterpart allocation, longitudinal/independent interpretation review; §19 | Project custodian/component/25/40 and independent humans; traceability/review/operating evidence; suite/operational assurance. No GT pass or independent sufficiency inferred. |

## 18. Implementation guidance — non-normative

An evidence snapshot, explicit question/premise register, versioned option set and controlled divergence map can support these functions. Shared services may implement separate profiles; no vendor/model/database/API/deployment count or cadence is mandated. For deferred Phase 2 CAP-01 only, the historical persona design foregrounded different aspects of one factual base without private factual sets or hidden moral optimisation. This example does not activate the use case. A diagram or narrative report is a presentation of canonical analysis, not its independent source of truth.

## 19. Traceability and change

| Capability / functions | REQs | CONs | Principal planned cases |
| --- | --- | --- | --- |
| CAP-001 / FUN-001/002 | 001–010 | 001/002 | 001–005 |
| CAP-002 / FUN-003 | 015–018 | 002/004 | 009–011 |
| CAP-003 / FUN-004 | 011–014/019 | 003/004 | 006–008/011 |
| CAP-004 / FUN-005/006 | 020–029 | 003/005/006 | 012–017 |
| CAP-005 / FUN-007/008 | 030–035 | 003–006 | 018–022 |
| CAP-006 / FUN-009 | 036–039 | 004/007 | 023/024 |
| CAP-007 / FUN-010 | 040–047 | 008/002/006 | 025–029 |
| All applicable functions | 048–052 | 002/009 | 030–032 |

WP synthesis/interpretive/corpus/charter and RP1/4 option obligations map through REQ-001–019 to the first three capabilities. TD §§2–6 and DEC-017/085 map to REQ-020–032 and CAP-004/005, with longitudinal responsibility explicitly allocated to 25. CMP's AOS-22 dispositions (C02/03/09/16/18/29/32–35) map to the human, evidence, options and feedback boundaries in §§1/7/8/10 and REQ-001–019/033–039; 21/23 retain their other GIL allocations. DEC-086 maps to CAP-007/FUN-010/CON-008/REQ-040–047/VER-025–029. The requirement table supplies exact source/rationale/case, and cases supply reverse links.

Source matrix and Exchange Register addenda record new component allocation, not exhaustive original-row closure or implementation compatibility. Prior source manifest, DEC/IF meanings and requirement statuses are preserved. Changes identify exact affected question/source/entity/analysis/profile and REQ/CON/VER revision, rationale, powers, consumer impacts, approval, actual application and outcome. Research can challenge/propose, never adopt; no requirement is retired in this initial draft.

## 20. Build and handover

No build or live activation is authorised by this draft. Eventual bounded handover fixes approved scope/wording, dependency/contract/profile versions, source/use assumptions, method rubrics and accepted evidence. Builder stops at missing mandatory authority/use/evidence, unresolved material classification, incompatible contracts or unsupported independent-profile/protected-route/recovery assumptions. Implementation discretion remains within approved behaviour. A separate competent reviewer must walk normal, exception and authority-boundary cases before G3; author/AI checks do not substitute for deferred independent project review.

## 21. Review and control

Author checks cover template sections, stable IDs, singular requirement records/metadata, source precision, requirement-case/reverse links, common ownership, incommensurability/precedent/CAP-01/independent-window boundaries, lifecycle/failure and honest dependencies. No synthesis, CAP-01, research or implementation case, independent review or institutional effectiveness assessment has been executed.

| QS coverage | Author evidence / remaining limit |
| --- | --- |
| QS-01–04 | Document control/source/status/scope and initial stable identifiers explicit |
| QS-05–10 | §4.3 individual statement/source/rationale/VER plus common owner/status/origin; §17 owns unresolved values; no hidden weights/numerical defaults |
| QS-11–14 | §§1/3/5/6/9–11 give responsibilities, contracts, lifecycle/failure; physical mappings and later counterparts pending |
| QS-15–20 | §§7–13 apply human powers, uncertainty, assessment/evaluation, real audit and governed feedback; actual assurance outstanding |
| QS-21–23 | §§14/15/19 give two-way traceability and normal/negative/degraded/cross-component cases, with CAP-01-specific cases retained only as deferred trace; none executed |
| QS-24–28 | §§16/17/20/21 distinguish author quality, design judgement, review and build/activation; no gate/tailoring claimed |

Specification-quality conclusion: organised functional review draft with 52 proposed requirements, nine contract views and 32 planned cases. Design-adequacy conclusion: applies current sources and approved directions, with operating dependencies and irreducible human assessment explicit. Mark's wording/whole-document review remains pending. No additional general design question emerged. AOS-24/25 are drafted; next GI-set consistency/disposition review, then AOS-40 scenarios.

## Component summary

**Purpose:** connect permitted organisational evidence and governing context to honest options and human judgement.  
**Owns:** synthesis, proposed interpretation and options/infeasible alternatives. CAP-01-specific analytical divergence is parked in Phase 2.  
**Receives:** exact domain/corpus/assessment evidence, current controls and human decision/outcome/context.  
**Produces:** canonical propositions/options/tension maps, referrals, correction/feedback and adaptation proposals.  
**Own research:** reasoning/interpretation/options adequacy remit using common profiles; operating assignment/settings remain owned gaps.  
**Reserved human authority:** moral/constitutional choices, explicit precedent adoption, independent profile approval and actual decisions.  
**Conformant when:** accepted evidence against an approved bounded baseline; drafting alone establishes no conformance.  
**Open dependencies:** appointments/profiles/content/permissions, exact implementation mappings, remaining counterparts and operational/independent assurance.


## Phase 2 scope disposition — 9 October 2026

DEC-097 controls over prior inclusion/annex statements. CAP-01/02-specific legacy requirements/cases are deferred and supply no current-core completion/acceptance obligation. General human judgement, independent challenge, evidence fidelity, cumulative risk/drift and protected reporting remain current. Existing closure of AT-CR-01–05 and pilot5b is retained; neither is reopened by this scope change. No case executed or operating approval granted.

**Allocation and source status:** Any older source/adoption row relying on deferred CAP-only IDs is a historical use-case contribution, not current-core coverage. Core source sufficiency must use the surviving general obligations and accepted evidence; no source is promoted by this deferral. Retained numbered totals count catalogue/trace entries, including deferred IDs, and must not be read as active-core requirement/test totals.

## Historical opening status notices — retained provenance

These are dated drafting snapshots, including their then-current versions, totals, completion statements and next tasks. They do not define today's baseline or work queue. The present document retains its proposed/planned status; approved directions retain their recorded scope. Use the current inventory, adopted README and live to-do list for orientation; authoritative requirement and decision text remains in its named sections.

**Historical status notice — revision set:** AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3.

**Historical status notice — scope decision — 9 October 2026, DEC-097:** Mark has moved CAP-01 Trade-Off Divergence and CAP-02 Risk Register Assessment into Phase 2 as specific use cases built on AOS. They are outside the current architecture/specification completion scope and are not current build, acceptance or publication prerequisites. No use-case design, configuration, implementation or testing is scheduled now. DEC-017's architectural inclusion is superseded on this point; its original record remains history. General human judgement, evidence, data-use/authority, independent challenge and protected reporting controls remain in the architecture. Dedicated legacy use-case IDs are retained only as deferred trace references, with original wording parked in Phase 2 (deferred under DEC-097); mixed rows retain only their general architectural obligations in current scope. Earlier inclusion/next-task/annex-dependency statements are superseded.

**GI consistency closure — 7 October 2026:** Mark authorised GI-CR-01–04 corrections and closure. Functional drafting, reciprocal report-independence wording, decision/outcome consumer allocation, Mode 2 wording and current completion statements are reconciled. AOS-23 changes counterpart/current references only; its REQ/VER/CON rows are unchanged. AOS-00/Map v0.32, DEC-001–091; AOS-20 v0.5/21 v0.6/22 v0.4/23 v0.5/24 v0.3/25 v0.2/30 v0.5; AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.15/Core v0.6/Exchange Register v0.14/source matrix v0.15; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. The review v0.2 records closure evidence; next AOS-40 acceptance scenarios. Earlier dated baseline/next-step statements remain historical. No new DEC/IF/operating power, case execution or build/activation/readiness approval; independent project review remains deferred and operating human independence remains mandatory.

