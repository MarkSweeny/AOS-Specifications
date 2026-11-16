# FAR-001 reconciliation with the controlled AOS architecture

Document: far-001-reconciliation-v0-1 · Source revision or record: FAR-001 reconciliation v0.1, 3 October 2026

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

| Document control | Value |
|---|---|
| Record | FAR-001 reconciliation, version 0.1 |
| Date | 3 October 2026 |
| Scope | FAR-001's 12 propositions, ten architectural rules, component template v0.2 and OQ-001–014 |
| Controlling architecture | AOS-00 draft v0.6 and specification map draft v0.3, 28 September 2026 |
| Governing sources | Foundational Principles v4; AOS Reasoning Principles v6; Governance Intelligence Tests |
| Working quality standard | AOS-QS v0.1, 18 September 2026 |
| Project owner and current approver | Mark Sweeny |
| Review | Assistant author analysis and project-owner decision; no independent review performed |
| Status | Reconciliation record; editorial/template corrections applied, one new design direction confirmed by the project owner; detailed requirements and mechanisms remain proposed |

## Outcome

FAR-001 is compatible with the controlled architecture when its proposals are interpreted within the existing source hierarchy and responsibility allocation. It supplies useful drafting refinements, not a replacement architecture. The review found three defects in the component template: the lack of an explicit requirement register, incomplete quality-standard review/handover coverage, and traceability wording that could omit requirements and planned verification. The reconciled template corrects these defects.

The ten architectural rules can remain as drafting guidance, subject to the qualifications recorded below. The system-wide enforcement function remains in AOS-01/03/05 with the AOS-04 agent contract; AOS-14 remains Boundary Intelligence and external exchange. No additional intelligence domain, deployment unit or universal technical enforcement mechanism is introduced.

The owner confirmed that semantic explanations should be a required default, with recorded exceptions for security, privacy or feasibility. This is the sole new substantive design direction resolved during this reconciliation. Its implementation requirements and acceptance cases are still to be drafted and approved.

## 1. Evidence and authority

| Material examined | Locator and use |
|---|---|
| FAR-001, 29 September | All 12 propositions, source-section index, critical reconciliation and record-integrity rule |
| Architectural Rules working draft, 29 September | Rules 1–10 and allocation note |
| Component template v0.2, updated 30 September | Document control, sections 1–19 and component summary |
| AOS-00 v0.6 | §§1–3 scope, authority and 19 responsibilities; §§4/4.1 proposed REQ-001–049; §9 planned VER-001–022; §10 DEC-001–026; status and review limits |
| Specification map v0.3 | Suite structure, ownership, D01–D13 and reconciliation state |
| AOS-QS v0.1 | QS-01–28, G1–G4, Appendix A and review checklist |
| FP v4 | Printed principles 1–10; especially purpose/function, permanent human Mode 2, structural integrity, transparency, imperfection, humility and emergence |
| RP v6 | Nine domains and 41 principle records; the complete supplied text, including tests, failure modes and implementation references |
| Governance Intelligence Tests | M1.1–M1.14 and M2.1–M2.15, as operational and human governance assessment obligations |
| Architecture Issues Register | OQ-001–014 and research-agent intake allocation |
| Source Traceability Matrix v0.1 | Existing source-item allocation record; no row status is changed by this reconciliation |

The evidence supports conceptual alignment and document corrections. It does not prove that the proposed mechanisms are secure, technically sufficient, implemented or legally conformant. No new legal interpretation, supplier evaluation or external-standard conformity claim was made. FAR-001 is an indexed synthesis; its cited original twenty-section conversation was not independently retrieved in full during this review. Substantive adoption therefore rests on the reviewed controlled sources and explicit owner decisions, rather than unseen passages.

REQ and VER identifiers below have the full prefixes **AOS-00-REQ-** and **AOS-00-VER-**. They identify existing proposed requirements and planned cases. A link may provide partial coverage; thematic alignment is not a complete traceability chain.

### Decisions confirmed in this session

| Local record | Decision | Authority and effect |
|---|---|---|
| FAR-R-001 | Use AOS-QS v0.1 as the project working standard for now; independent review is deferred because Mark is the sole human project participant. | Mark's instruction, 3 October. Record author/project review accurately. Do not waive QS-24/25/28 or claim G3 where the required separate review is absent. Organisational independent review of GI interpretation under DEC-010–012 is unaffected. |
| FAR-R-002 | Constraint explanations are a required default: meaning, authority basis and escalation route; exceptions for security, privacy or feasibility need a recorded reason and review. | Mark selected this option on 3 October. Allocate to AOS-01/03/04/05, applied by AOS-14. Explanation cannot itself grant permission or replace independent enforcement. Exact requirement wording remains draft. |

These local record IDs are reconciliation locators, not new AOS-00 DEC identifiers. FAR-R-002 needs incorporation into the controlled architecture decision register during its next revision, preserving source and approval evidence. No existing decision is superseded.

## 2. FAR-001 proposition dispositions

“Retain” means retain the proposition within the stated existing constraints. It does not approve a new mechanism or every phrase of the original conversation.

| FAR proposition | Disposition | Controlling basis and existing coverage | Remaining obligation |
|---|---|---|---|
| 1. Legitimate objective, illegitimate means | Retain | FP1/2/3; RP Agentic Delegation and Data/Sensing; DEC-003/005/007; REQ-005–007/025/031/040; VER-003/004/013/017 | Purpose and authority must be assessed separately; action cannot proceed on telos alignment alone. |
| 2. Telos, ethics, authority, knowledge and transparency | Retain with precision | FP2–6; RP Ethics/Telos, Blind Spots, Transparency, Delegation; QS-16–19; REQ-005–007/012/014/040 | No mandatory serial reasoning pipeline or recoverable private reasoning is implied. AOS-04/20/22 define observable assessments and escalation. |
| 3. Semantic boundaries plus independent enforcement | Retain with owner-confirmed default | FAR-R-002; DEC-005; REQ-006/007/023/040; VER-004/013/017 supply partial coverage | New explanation fields, exception governance, version alignment and acceptance cases required in AOS-01/03/04/05. |
| 4. Character, constraint and accountability | Retain as rationale | FP3–6; RP Ethics/Telos, Transparency and Delegation; QS-18/19/23 | “Character” describes intended behaviour, not moral authority. Threat modelling must assess combined control failures. |
| 5. Organisational legibility | Retain with evidence qualification | FP4; RP consequential decision records and transparency; QS-13/19; REQ-010/012/014/024; VER-006/008/018 | Evidence must distinguish observations, model outputs, approved human rationale and retrospective explanation; lawful access, retention and minimisation remain explicit. |
| 6. Cumulative, population, emergent and capability effects | Retain as assurance concern | FP10; RP emergence and Mode 2 pressure; GT M1.13; QS-18/23; REQ-019/034; VER-010/015 | Partial coverage only. AOS-04/25/40 must define indicators, populations, horizons and change triggers. Does not reopen deferred self-calibration DEC-018. |
| 7. Cross-organisation duties/federation | Retain existing exchange duties; defer federated model | DEC-005/014/016/020; REQ-011/035–037/040; VER-007/015/016 | OQ-012 stays open. No new duty to notify externally, shared instance or federation protocol is assumed; explicit authority and verified obligations are prerequisites. |
| 8. Functional prescription and contract hierarchy | Retain with corrected traceability | DEC-001/005/015/019; QS-07/12/21/22; REQ-001/003/020/021/030/036; VER-001/002/012/015 | Capability/function/contract views complement requirement records. Preserve requirements and planned verification, even when no capability/function decomposition is needed. No product mandate or sector-independent rescoping. |
| 9. Publication package and normative foundation | Retain existing sequence | FP/RP hierarchy in AOS-00 §2.2; DEC-021–026; 28 September publication decision; REQ-017/041; VER-011/019 | First package is architecture draft, manifesto and bounded overdue-repair example. Reference implementation follows separately. No publication approval follows from this record. |
| 10. Observe → Challenge → Evolve | Retain proposal-only research; defer amendment process | QS-20/26; DEC-007/024/025; REQ-015/025/045–048; VER-009/017/020/021 | Agents observe and propose; approved humans decide. Organisation telos authority is distinct from authority to amend the AOS specification. Change Constitution remains to be drafted. |
| 11. Transferable governance | Retain role-based design | DEC-009; QS-01/08/16; REQ-033; VER-014 | Mark currently holds project roles. Appointment, succession and conflict handling belong in the Change Constitution; no fictional independent role is filled. |
| 12. Living Specification as recursive demonstration | Defer later RI-001 scope; reject first-example substitution | DEC-021–026 and existing publication direction | OQ-014 stays open for later implementation design. RI-001 does not replace the overdue-repair first example. |

## 3. Ten architectural-rule dispositions

| Rule | Result | Reconciliation and destination |
|---|---|---|
| 1 Functional prescription | Retain | DEC-019 and QS-07; technical choices may be required before the relevant build but must remain separately authorised and justified. |
| 2 Purpose does not confer authority | Retain | DEC-003/005/007 and RP Delegation; no change to scope or authority. |
| 3 Independent constraint | Retain with wording correction | Prevent unilateral change to effective authority. An actor may interpret evidence or ask for clarification, but its interpretation cannot activate broader permission. Threat-model independence remains OQ-003/D08. |
| 4 Organisational legibility | Retain with wording correction | Align “reasoning” with QS-19: captured evidence, model output, applied rules and approved human rationale. No private chain-of-thought requirement or unrestricted disclosure. |
| 5 Defence in depth | Retain as design direction | QS-18/23 and FP5/10; test failure combinations rather than claim invulnerability. Physical/control-plane separation is not yet prescribed. |
| 6 Semantic boundaries | Strengthen per FAR-R-002 | Required explanatory default with reasoned/reviewed exceptions. Exception does not waive the constraint. Exact schema and approver roles belong in component specifications. |
| 7 Governed evolution | Retain | Project specification amendment governance is separate from each organisation's protected telos/schedule amendments. DEC-018 remains deferred. |
| 8 Cross-architectural coherence | Retain | QS-21/26; impact assessment must expose unknown dependencies rather than claim complete automatic discovery. |
| 9 Transferable governance | Retain | Role definitions may outlive founder; independent project review remains explicitly unfilled/deferred. |
| 10 Conformance through contracts | Retain with scope qualification | QS-22/23/25; declare component/profile scope and evidence. Conformance is not established by product choice or contract existence alone. OQ-011 remains open for the claim model. |

The corrected rules remain a working drafting aid. The controlling FP/RP, recorded decisions and AOS-QS govern where their wording differs. No rule is silently converted into a stable component requirement.

## 4. Component-template reconciliation

| Template coverage | AOS-QS Appendix A / rules | Result and correction |
|---|---|---|
| Document control | QS-01/03; Appendix A control fields | Add author, reviewer/vacancy, working QS version, gate/evidence, release scope and manifest. Separate custodian from approval authority. |
| §§1–3 purpose, sources, responsibilities | Appendix A 1–3; QS-10/11/17 | Retain; add explicit architecture/context view and FP/RP/GT applicability. Source hierarchy is precedence, not a mandatory approval step for every derived record. |
| §4 capabilities/functions | Appendix A 4; QS-04–09 | Add §4.3 explicit requirement register with all QS-08 attributes. CAP/FUN IDs are useful decomposition, not replacements for REQ IDs. |
| §5 state model and §10 workflows | Appendix A 6; QS-14/16 | Retain. Required state detail is applicable where persistent/governed state exists; explain non-applicability. |
| §6 contracts | Appendix A 5; QS-12 | Add complete interface attributes: schemas, units, timing, receipt, ordering, duplicates, retries and revocation, or reasoned non-applicability. Cross-reference authoritative shared contracts. |
| §§7–9 authority, principles, data | Appendix A 2/5/6/7; QS-13/16–20 | Retain; add new semantic default, complete three-source applicability and distinction between sensing/authority/capability. |
| §§11–13 failure, evidence, qualities | Appendix A 7–8; QS-14/15/18/19 | Retain; clarify evidence meaning, distinguish deterministic enforcement from probabilistic inference, require model-change review and evaluated limits. |
| §14 invariants | QS-05–08/21/22 | Retain as optional decomposition where useful. Each binding invariant needs a REQ record or explicit linkage to one. |
| §15 conformance | Appendix A 9; QS-22/23 | Add VER records and all QS-22 attributes. CR claims and VER cases are distinct; execution evidence is separately versioned and dated. |
| §§16–17 dependencies/issues | Appendix A 10; QS-09/25 | Retain, with requirement impact and explicit review gate; no default answers. |
| §18 implementation guidance | QS-04/07 | Retain non-normative status; approved implementation choices belong in a separately controlled implementation baseline. |
| §19 traceability/change | Appendix A 12; QS-21/24/26 | Restore REQ and VER in traceability; distinguish derivation path from universal sequence. |
| New §20 build and handover | Appendix A 11; QS-25/28 | Specify allowed scope, exclusions, fixed contracts/configuration, discretionary implementation choices and builder stop conditions. |
| New §21 review and control | Appendix A 12; QS-24–28 | Include QS checklist/evidence, separate quality/design conclusions, findings/tailoring, reviewer/approver and gate evidence. Record independent review as deferred. |

Identifiers CAP, FUN, CON, INV and CR introduced by the working template do not retire the existing REQ/IF/DEC/VER conventions. A contract may be referenced through an interface; either way identity and semantic ownership must remain unambiguous. This reconciliation supplies no new contract ownership approval under the still-open DEC-002.

## 5. Open-question disposition

| Issue | Current disposition | Owner specification / next evidence |
|---|---|---|
| OQ-001 ethics representation | Open detailed design | AOS-04/20 with AOS-01; novel cases and RP applicability. No simplistic ethical score adopted. |
| OQ-002 boundary classes | Direction constrained; classification open | AOS-01/03/05/30; identify non-waivable core versus authorised operational parameters and lawful exceptions. |
| OQ-003 constraint independence | Open technical assurance | AOS-01/04/05/40; threat model, privileges, bypass/race/restart cases. Logical allocation alone is insufficient evidence. |
| OQ-004 ethical conflicts | Human Mode 2 settled; process open | AOS-20/22/30; authorised recipients, dissent, timing and unresolved outcomes. |
| OQ-005 human-reserved decisions | Core settled; organisation schedule open | AOS-01/04/30; DEC-004/021/024/025 and organisation classification, never hidden thresholds. |
| OQ-006 material-action records | Open operational definition | AOS-02/04/30/40; proportionality, source obligations and versioned evidence schema. |
| OQ-007 cumulative/emergent effects | Open design | AOS-04/25/40 with domain contributors; scenarios, indicators, horizons and false positives. AOS-14 covers external signals only. |
| OQ-008 dependency discovery | Existing change duty; mechanism open | AOS-00/02/40; contract registry, manual/automated discovery limits and change-impact cases. |
| OQ-009 change evidence/challenge | Open constitutional procedure | Change Constitution; proposal evidence, dissent, authority and closure. |
| OQ-010 protected AOS constitution | Open project governance | Change Constitution/AOS-00; distinguish specification changes from organisation telos. |
| OQ-011 conformance claim model | Open detailed design | AOS-40/02; scope, assessor, evidence, expiry and partial claims. |
| OQ-012 federation | Deferred beyond existing exchange obligations | AOS-14/01/02/03; explicit future scope and verified duties before adopting any federated mechanism. |
| OQ-013 Boundary naming/allocation | Resolved for working terminology | Use “Boundary Intelligence and external exchange” for AOS-14; “shared authority and data-use enforcement” for systemwide controls. DEC-005 remains controlling. D08 mechanisms remain open. |
| OQ-014 RI-001 sequencing | First-example question resolved; later scope open | Overdue repair first; later RI-001 scope/acceptance remains deferred. No new implementation authorisation. |

Additional drafting obligation: semantic explanation schema and exception approval remain to be specified under FAR-R-002. Material choices in these open items return to Mark as the component work progresses. They are not inferred by this record.

## 6. Changes and readiness

Applied document corrections: Architectural Rules revised to identify working guidance, precise evidence and authority wording, and FAR-R-002. Component template advanced to v0.3 with requirements, planned VER records, complete QS coverage, build handover and review. Issue register records terminology disposition and the semantic-default direction. To-do items 5 and 5a record the owner instruction and completed reconciliation, while detailed design obligations remain with the component work and Change Constitution.

AOS-00 v0.6, its REQ/VER catalogue, the 19 specification boundaries and the source fingerprints are preserved. The next architecture revision should incorporate FAR-R-002 into its decision register and update source references; exact component requirements and tests require their normal approval. There is no claim that any component passes G2/G3, or that a constraint is impossible to bypass. No source-traceability row is promoted to confirmed here.

**Specification-quality conclusion:** the reconciliation identifies and corrects template omissions and makes residual gaps explicit; populated specifications must still be reviewed individually against AOS-QS.  
**Design-adequacy conclusion:** the FAR proposals align within the recorded qualifications; semantic explanation default is owner-confirmed, while enforcement sufficiency, federated governance and change mechanisms remain open.  
**Independent review:** deferred and unperformed.  
**Next work:** review the AOS-14 research pilot (item 5b), then draft the shared authority/data/agent contracts together (item 6), using the reconciled template and source matrix.

