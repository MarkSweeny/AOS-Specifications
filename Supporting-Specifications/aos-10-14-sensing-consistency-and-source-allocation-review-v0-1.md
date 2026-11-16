# AOS-10–14 — Sensing-domain consistency and source-allocation review

Document: aos-10-14-sensing-consistency-and-source-allocation-review-v0-1 · Source revision or record: v0.4

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**Current sensing consistency closure — 9 October 2026:** Mark authorised the remaining consistency work. SENS-CR-01–05 are closed at the functional-document/author-review level: all40 logical CON views across10–14 and40 have exact central adoption, producer/consumer/shared-owner and REQ/VER links; all80 controlled FP/RP/GT sources have precise current contributions and owned residual/gate dispositions; current body/control statements are reconciled. Versions10v0.4/11v0.3/12v0.3/13v0.2/14v0.8/40v0.6; Architecture/Mapv0.42; Sharedv0.18/Corev0.6/ExchangeRegisterv0.17/SourceMatrixv0.18; reviewv0.4. DEC001–096 unchanged. Sensing269 proposed REQs/176 planned VERs;40 retains40/38. No new requirement/case/interface, source promotion or execution. Exact compatible wire schemas/profiles, organisation appointments/capacity, independent review, legal/institutional/practice evidence and scoped build/activation remain separate; independent project review remains deferred. Earlier dated notices/addenda are historical. Current controlling allocation is the9October manifest and source addendum below.

**Current approved Boundary directions — 9 October 2026:** Mark agreed all five review recommendations at09:51UK time, qualifying material obligations to distinguish financial exposure from resource impacts. AOS-00-DEC-092–096 records those architectural directions; prior DEC001–091 unchanged. AOS-14 v0.7 incorporates the decisions into existing requirements/cases/contracts and resolves ISS003–007 at architectural-direction level. Exact organisation-specific materiality criteria, outcome evidence, obligation schemas/owners, declared control paths and pattern profiles remain implementation/commissioning gates; federation remains deferred. Architecture/Mapv0.41; Sharedv0.17/ExchangeRegisterv0.16/SourceMatrixv0.17; reviewv0.3. Other component versions unchanged.55 proposed Boundary requirements/34 planned cases; no new REQ/VER/IF, executed test, whole-document or build/operating approval. Earlier dated notices are historical. Next: remaining whole-sensing common/source/status corrections SENS-CR-02–04; independent review remains deferred as previously agreed.

**Current Boundary completion — 9 October 2026:** AOS-14 v0.6 completes the functional proposed core/research/supplier migration:55 requirements/34 planned cases, all80 FP/RP/GT contribution rows and explicit typed determination/contract mapping. Architecture/Map v0.40; DEC-001–091 unchanged. Shared Contracts v0.16/Exchange Register v0.15/Source Matrix v0.16 adopt Boundary-only links; Core v0.6, kernel01–05 v0.8 and10 v0.3/11 v0.2/12 v0.2/13 v0.1/25 v0.2/30 v0.5/40 v0.5 unchanged. Working naming resolved under existing OQ-013; federation deferred OQ-012; other material Boundary questions/commissioning and independent review remain gates. No new DEC/IF, case execution, build readiness or activation approval. Earlier dated baseline/next-step notes are history; no historical source status promoted. Next: Mark's Boundary review and scoped decision dispositions; complete remaining whole-sensing common/source/status remedies from SENS-CR-02–04.

| Document control | Value |
| --- | --- |
| Identifier / version / date | AOS-SENS-REVIEW / 0.4 / 9 October 2026 |
| Status | Completed author consistency review; SENS-CR-01–05 closed at functional-document level; independent/executed assurance separate |
| Project owner / custodian | Mark Sweeny |
| Reviewer | Codex; author review, not independent assessment |
| Scope | AOS-10–14 responsibilities, information exchanges, behaviour and source allocation against the current common infrastructure |
| Authority | Review requested by Mark on 9 October; no authority inferred to adopt new design decisions or amend component requirements |
| Readiness | No case executed; no build, activation, G3/G4, legal or institutional conformance conclusion |

## 1. Conclusion

The five-domain allocation is coherent at the functional level. Asset owns physical condition and completion evidence; Resident owns private assistance and governed resident interaction; People owns workforce support and evidence while personnel judgement remains human; Process owns coordination and duty tracking; Boundary owns external exchange. Constitutional authority, shared evidence semantics, identity/data use, agent lifecycle and runtime enforcement remain with AOS-01–05. Supplier products may implement several logical functions without acquiring their combined authority.

The review identifies five open findings. The most substantial is the incomplete migration of Boundary's original functions into individually traceable requirements and planned cases. The common exchange register and source matrix also lag behind the new domain drafts. One explicit status contradiction remains: Boundary's naming issue is open locally but resolved in the issues register. Other current-versus-historical passages need reconciliation. Inbound determination vocabulary is not mapped explicitly enough for a builder to know how the different labels relate.

This is a qualified positive architectural assessment, not closure of all sensing work. The report supplies a source-contribution inventory for all 80 controlled items, retaining partial and outside-domain obligations. It does not promote the canonical matrix's historical statuses or convert software evidence into an institutional judgement.

## 2. Reviewed baseline and method

The canonical to-do file was read first; its current starting point is this review. Fresh OneDrive text copies were used to read the original Markdown contents. The original files were the source of those copies; the copies are access aids, not a competing canonical suite. The to-do copy's extracted UTF-8 content matches the listed original byte count before the local editor's added final newline. Direct Markdown text extraction and raw download remained unavailable. Connection-test success does not demonstrate the scheduled research agent's access.

| Set | Current versions reviewed |
| --- | --- |
| Sensing | AOS-10 v0.3; 11 v0.2; 12 v0.2; 13 v0.1; 14 v0.5 |
| Architecture and map | AOS-00 and Specification Map v0.39; DEC-001–091 |
| Kernel | AOS-01–05 v0.8 |
| Common | Shared Contracts v0.15; Core Records v0.6; Kernel Exchange Register v0.14; Control Coordination v0.2; Protected Reporting and Recovery v0.1; Operational Profiles v0.1; Contract Model working draft |
| Assurance / human and oversight counterparts | AOS-40 v0.5; AOS-30 v0.5; AOS-25 v0.2 |
| Sources and quality | FP v4; RP v6; Governance Intelligence Tests; preserved source manifest; Source Traceability Matrix v0.15; AOS-QS v0.1; component template v0.4; Architectural Rules working draft |
| Existing question status | Architecture Issues Register including 3 October dispositions and 4 October intake |

Method: inspect ownership and trust transitions; walk normal, unknown, conflicting, partial, rejected and changed-permission paths; compare shared semantic owners and lifecycle rules; check requirement/case links and identifiers; review source contributions against the 10 FP principles, 41 RP principles and 29 GT tests. AOS-25/30 were inspected as specific counterparts; this is not a repeat review of the entire GI suite. Books and external sources cited by the drafts were not freshly researched or legally validated in this review.

### 2.1 Structural results

| Component | Proposed numbered REQs | Planned numbered VERs | GT applicability rows | Result |
| --- | ---: | ---: | ---: | --- |
| AOS-10 | 49 | 34 | 29 | All 21 main template sections; unique sequential REQs/cases; forward and reverse requirement/case links agree |
| AOS-11 | 55 | 33 | 29 | Same structural result |
| AOS-12 | 53 | 35 | 29 | Same structural result |
| AOS-13 | 57 | 40 | 29 | Same structural result |
| AOS-14 | 9 | 7 | No full 29-row applicability appendix | Counts cover research and supplier allocation only; original Boundary obligations remain in CAP/FUN/CON/INV/CR form |
| Total sensing | 223 | 149 | Four complete contribution appendices | Counts do not establish full functional verification coverage |
| AOS-40 counterpart | 40 | 38 | 29 | Reviewed assembled cases and domain-adoption addenda; not executed |

The reciprocal-link check for AOS-10–13 found zero declared-link mismatches across 214 requirements and 142 cases. Boundary's abbreviated research tables were checked separately: REQ-001/007→VER-001; 002→002; 003→003; 004/008→004; 005→005; 006→006; supplier REQ-009→VER-007. These links agree. These are document checks, not tests of implementation, source sufficiency or independent assurance.

## 3. Responsibility and exchange assessment

| Meaning / responsibility | Producer or accountable function | Consumer / control boundary | Assessment and exact anchors |
| --- | --- | --- | --- |
| Physical observation, condition, promise and completion | 10, with attributable source and competent human stewards | 02 records; 13 coordination; 11 explanation; 14 supplier intake | Coherent: 10 REQ-003–020, CON-001–004; 13 REQ-003/004/030–035; 11 REQ-010/011/025/026 |
| Private resident assistance and selected sharing | 11 | Current 03 purpose/identity checks; selected enterprise request to 13 | Coherent: 11 REQ-001–009/031–034; 12 REQ-036 and 13 REQ-042 preserve private content exclusion |
| Resident channel and contact delivery | 11, consuming current human owner/team details | 14 dispatch; 13 tracked communication duty; 30 human accountability | Coherent: 11 REQ-017–024; 13 REQ-036/037; 30 REQ-021–024/031–033; neither dispatch nor silence establishes acceptance |
| Workforce capability/listening/workload | 12; operational context may come from 13 | 03 sensitive-use/disclosure; permitted 25/30 governance review | Coherent: 12 REQ-001–031/035/036; 13 REQ-040/042; workforce activity does not become individual surveillance or an employment decision |
| Process definition, attempt, accepted duty and actual outcome | 13 with separate empowered human owner | 04 task semantics; 05 runtime/account; 30 human decisions; 02 custody | Coherent: 13 REQ-011–029/043–049; KX-07/21/26; COORD CHECK/ACT/CHG/ACC/RSV/WHD/BRK |
| External admissibility/disclosure/commitment/effect | 14 | Shared 01/03/04/05 determinations and enforcement; 02 records; recipient domain meaning | Allocation coherent; complete numbered obligations and disposition mappings remain findings SENS-CR-01/05 |
| Specialist external research | Each component owns its remit/implications | 14 collection; 04 behaviour; 02 RSVIEW-0.1; 13 duty; 30 disposition; 01 amendment | All five explicitly adopt the common pattern; no substantive research monopoly moves to Boundary |
| Domain risk versus aggregate drift | Domains supply bounded risk/coverage signals | 25 assesses cross-component/system patterns; humans decide | Coherent direction; 14 ISS-003 still requires an exact pattern allocation before affected implementation |
| Supplier realisation | One or several products may fulfil logical functions | Explicit source/case masters and actual control locations | All five now provide mappings, arrangements, examples and response matrices; no product selected or certified |

The newer domain views consume shared meanings rather than invent substitute grants, private cumulative budgets, implicit consent or separate acknowledgement definitions. The missing central adoption rows are a documentation gap, not evidence that every local domain view is semantically incompatible.

## 4. Behaviour walkthroughs

### 4.1 Overdue repair

10 supplies the communicated promise, approved comparison meaning and attributable completion evidence. 13 compares the approved boundary with current time. Evidenced outstanding promised work supports overdue-incomplete; missing completion evidence supports completion-unverified after the promised date. Missing/contradictory promise evidence creates an owned evidence exception. Internal targets and promise revisions cannot erase the original commitment or breach history.

13 tracks an empowered human through 30. Receipt, validation, application and acceptance of responsibility remain distinct. 11 sends the current named-owner and accountable-team contacts through the agreed channel; 14 handles the external exchange using shared controls. Rejection, absence, unavailable owner contact or failed communication retains the appropriate residual duty. Actual physical work, disputed/partial scope, human disposition and service communication remain separate closure evidence.

Anchors: 10 REQ-013–021/032 and VER-010–018; 11 REQ-017–030 and VER-010–016; 13 REQ-030–039 and VER-022–027; 30 REQ-021–033/036; 40 VER-007–010/038 and its latest Process adoption addendum. No contradiction found in these meanings. Older body passages saying Process is still undrafted are addressed in SENS-CR-04.

### 4.2 Changed permission, unknown effect and recovery

Each new consequential attempt needs current exact-operation checks. Source/permission/channel changes selectively reassess affected pending work. Unknown prior dispatch or effect is reconciled before repetition; compensation has separate authority. Cancellation or a technical terminal state does not erase continuing human/service duties. Recovery establishes current restrictions and reconciles effects and lifecycle before scoped continuation.

Anchors: 10 REQ-012/031/035/036; 11 REQ-018/024/040–046; 12 REQ-033/034/037/041/042; 13 REQ-011–015/021–027/043/045/046; 14 §§5/7/11 and supplier VER-007; common controls and 40 VER-020–025/038. The shared meaning is coherent; exact mechanisms remain build/activation dependencies.

### 4.3 Welfare, privacy and workforce judgement

Physical asset signals cannot silently become resident behavioural inference. Private assistance does not become enterprise training or workforce-support input. Optional property notifications/welfare referrals require their separate approved tiers, audience and human route. Declining optional use does not remove core services or independently governed safety duties. People evidence supports substantive human employment decisions; signatures and proxy scores alone are insufficient. Protected concerns use a permitted alternative to an implicated recipient.

Anchors: 10 REQ-011/028–030; 11 REQ-005–009/014–016/031–039; 12 REQ-005–007/017–024/026/029–036; 13 REQ-019/040/042; 30 REQ-025/026/032/033; 40 VER-015/016/021/037/038. Any separately proposed behavioural-inference purpose remains outside this commissioned scope; the RP source's possibility of separately governed consent-based inference does not itself authorise one.

### 4.4 Research and supplier change

One retrieved source may inform several specialist findings, but coalescing it cannot erase distinct owners, reviews or deadlines. Future-effective or wrong-jurisdiction material cannot become a current operational rule. Acceptance for further work is distinct from amendment, verified application and actual outcome. Product-internal flows preserve the same boundaries as inter-product flows; manual fit cannot claim automatic enforcement. All five contain these directions and planned checks. Common producer/consumer and source-allocation recording must catch up.

## 5. Historical v0.1 findings and remedies — current dispositions in v0.4 closure below

### SENS-CR-01 — Boundary's core obligations lack the current requirement/verification structure

**Priority:** high. **Type:** known specification gap. **Status:** open. **Owner:** Boundary specification custodian with shared semantic and assurance owners; Mark approves material dispositions.

**Evidence:** AOS-14 §§4/14/15/19/20 retain original CAP-001–008, FUN-001–009, INV-001–008 and CR-001–010. Its nine REQs/seven VERs expressly cover research/supplier work only. There is no full FP/RP/29-GT applicability treatment comparable to 10–13. Template v0.4 §§4.3/14/15/19/21 and AOS-QS require binding obligations/invariants to have a requirement and planned-verification chain. Supplier VER-007's broad walkthrough does not replace individual exchange-obligation tests.

**Remedy:** migrate the retained functions into proposed numbered REQs and cases, preserving REQ-001–009/VER-001–007 and old identities as derivation links. Explicitly allocate current checks, source standing, obligations, actual-effect uncertainty, bypass, privacy, accepted duties, correction and recovery. Add controlled source/GT applicability with human and longitudinal boundaries. Keep unresolved design choices as owned issues rather than invented defaults.

**Closure:** every binding original function/invariant/criterion has a defensible REQ→CON/state/control→VER chain or explicit scoped unresolved disposition; reciprocal links and all 80-source applicability are accounted for. A document-level closure does not constitute operating conformance.

### SENS-CR-02 — Central common-contract adoption records lag behind the domain drafts

**Priority:** medium. **Type:** cross-document completeness gap. **Status:** open. **Owner:** exchange/shared-record custodians with each domain and consumer owner.

**Evidence:** Exchange Register v0.14 and Shared Contracts v0.15 current notices stop at the 7 October GI closure. The register's research-adoption table records 01–05/14/20 and later GI/30 sections, but not the new 10–13 domain view/REQ/VER allocations. Domains now declare 10 CON-001–007, 11 CON-001–007, 12 CON-001–007 and 13 CON-001–008; 40's adoption addenda describe their assembled contribution. Shared §4.7 still says the 14 CON-001–004 mapping remains to be incorporated.

**Remedy:** add exact domain version/view→shared REC/KX/IF/profile mappings, producers/consumers, acknowledgement/rejection/retry/change/recovery semantics and research allocations. Include reciprocal domain and 40 links, preserving semantic owners and existing IF identities. Distinguish logical adoption from approved wire-schema compatibility and actual execution.

**Closure:** one current adoption manifest accounts for every domain CON and affected shared exchange, with exact counterpart obligations/cases and explicit gaps. No duplicate common field dictionary is introduced.

### SENS-CR-03 — The controlled source matrix has no current sensing/AOS-40 allocation addendum

**Priority:** high for source-complete handover; medium for continued drafting. **Type:** source-allocation gap. **Status:** open. **Owner:** source-traceability custodian with domain and assurance stewards.

**Evidence:** Matrix v0.15 retains the historical 80-row 17 confirmed/28 partial/35 unresolved accounting and GI closure addenda. It has no current exact 10–13 or 40 allocation addendum. Domains' §8 RP-domain summaries and 29-row GT contribution appendices provide useful evidence, but do not supply a full current individual-RP source→REQ→VER disposition. Boundary's core migration remains incomplete. Example available chains: RP3 Golden Thread→10 REQ-024–026/047→VER-020–022→40 VER-036; RP9 sensing boundaries→10 REQ-028/029→VER-024 and 11 REQ-031/033→VER-017/018; workforce purpose→12 REQ-026/036→VER-016/024 and 13 REQ-042→VER-030.

**Remedy:** use Appendices A–C as a review inventory to create an exact current allocation/disposition addendum for all 80 sources. Preserve historical accounting, source versions and manifest. Separate domain contribution, cross-component completion, institutional/human evidence and future execution. Never mark a source confirmed merely because a themed case exists.

**Closure:** each source item has current links or an explicit residual finding/non-applicability reason with owner/gate; approved direction, proposed requirement, planned case and actual result have distinct standing. No aggregate coverage score implies statutory or institutional assurance.

### SENS-CR-04 — Current status and historical baselines need explicit reconciliation

**Priority:** medium. **Type:** one status contradiction plus document-control ambiguity. **Status:** open. **Owner:** specification and issues custodians; no new naming choice required.

**Evidence:** AOS-14 ISS-002 says Boundary terminology/OQ-013 is open. The issues register's 3 October disposition resolves working naming/allocation under DEC-005. AOS-14 ISS-001 describes federation as open whereas OQ-012 explicitly defers the federated model; current controlled external exchange remains in scope. AOS-14 §15 still says partial conformance is undefined pending AOS-40, though 40 v0.5 §§5/15 now defines scoped claims and unperformed/blocked/inconclusive distinctions. 10–13 document-control/body passages cite earlier 14/40 and architecture versions while later notices/addenda cite current versions; 40 VER-007/008 body still says the Process counterpart is pending although its final addendum adopts it. 10–12 ISS/next-work passages similarly retain drafted-counterpart dependencies.

**Remedy:** publish a concise current baseline and explicit supersession/disposition pointers. Resolve naming locally by reference to the existing disposition; label federated-model work deferred, retaining actual exchange obligations. Replace obsolete pending-draft/partial-conformance statements with exact current counterpart references and the remaining executable/operating dependencies. Keep historical entries as history rather than silently erasing them. Do not close wire-schema, capacity or executed-evidence dependencies merely because drafting is complete.

**Closure:** no builder must choose between two apparently current states. OQ-013 is not resubmitted; OQ-012 is not activated. Common/source histories and original IDs remain intact.

### SENS-CR-05 — Boundary determination vocabulary needs an explicit cross-view mapping

**Priority:** medium. **Type:** semantic ambiguity. **Status:** open. **Owner:** AOS-14 semantic owner with 02 and receiving-domain owners.

**Evidence:** AOS-14 FUN-002 returns admit/admit-with-conditions/quarantine/reject/escalate/unresolved; FUN-003 returns permit/constrain/deny/escalate/unresolved; CON-002 lists permit/constrain/deny/quarantine/escalate/unresolved. Shared §4.1 evidence admission uses accepted/accepted-with-restrictions/rejected/unresolved; §4.7 treats quarantine as restricted evidence state and escalation as non-authorising. No explicit map states which operation/direction a determination authorises, how conditional admission becomes governed evidence acceptance, or which vocabulary is a decision versus an object state. These may be compatible views, but compatibility is not yet specified.

**Remedy:** document typed determination meanings and an explicit mapping, retaining original decision, conditions and uncertainty. Keep boundary admission separate from evidence acceptance and recipient-purpose permission. Quarantine/escalation must not be coerced to permission; admission must not become truth. Add positive and adversarial round-trip cases, including conditions unmet, wrong direction/purpose, denied/unresolved state and late change. No new operating permission is required to clarify these semantics.

**Closure:** exact producers/consumers interpret every declared result consistently or reject unsupported meanings; no permissive default or silent state coercion. Wire enumerations remain separately commissioned.

## 6. Existing decisions and implementation dependencies

No new material architectural decision was required to perform this review. SENS-CR-01–05 are proposed corrections/completions, not approved changes. Existing unresolved Boundary choices remain: cumulative 14-versus-25 pattern allocation (ISS-003), consequentiality (004), actual-effect/closure criteria (005), obligation ownership/lifecycle (006) and mixed-control boundary definition (007). Federation retains its recorded deferral; naming has an existing resolution. These questions must be resolved or tightly scoped with an approved profile before the affected build/activation claim, not guessed by a coding agent.

Across all five, exact schemas and mappings, date/clock/units, evidence/currentness/completion and disclosure profiles, roles/cover/capacity, provider/model evaluations, approved operating authority and executed/independent evidence remain open. Research-watch baseline access/delivery remains item 5b. Item 6 common implementation, item 8 case/annex/execution coverage, item 9 domain adoption and item 12a supplier briefing are not closed by this author review.

## 7. Recommended next sequence and disposition

1. Complete AOS-14 migration and explicit disposition mapping, using the existing approved boundaries and recording unresolved general choices.
2. Reconcile current versions/status/dependencies, including the already resolved naming issue and deferred federation.
3. Update common adoption and exact source-allocation addenda; rerun reciprocal document checks and close individual findings only with evidence.
4. Present any genuinely unresolved material Boundary choices to Mark as a bounded set with recommendations; retain separate build/operating setup and independent review gates.

The review itself is complete. Five findings remain open; the sensing consistency workstream is not yet closed. The next canonical starting point should be AOS-14 requirement/test/source migration, followed by targeted common/source/status corrections. This request did not authorise adoption of a new design settlement, and no component/common/source requirements have been amended by this report.

## Appendix A — Foundational source contributions

The following are candidate current contribution links verified against the reviewed drafts. They are not replacements for the matrix, approved requirements or institutional conclusions. In link shorthand, `10 R003→V002` means AOS-10-REQ-003→AOS-10-VER-002. Each item retains human/cross-domain obligations beyond the listed example.

| FP v4 source | Current contribution | Residual boundary |
| --- | --- | --- |
| 1 Telos/conferred purpose/function | 10 R001→V001; 13 R001→V001; 25 R006→V004 | Humans/01/20 retain conferred purpose and adjudication |
| 2 Permanently human Mode 2 | 12 R005/006→V004; 13 R024→V017 | Actual substantive judgement and whole institutional boundary |
| 3 Architectural integrity | 13 R011/013/049→V008/009/035; 12 R031→V021 | Boundary core migration and independent enforcement/assessment |
| 4 Radical transparency | 10 R003→V002; 13 R048→V035 | Permitted source access and actual reconstructability |
| 5 Bounded rationality/imperfection | 10 R004/035→V003/029; 13 R057→V040 | Unknown perimeter, novel cases and actual fallback |
| 6 Epistemic humility | 10 R006/009→V005/007; 11 R011→V006 | Human challenge and uncertainty in practice |
| 7 No-exit obligation | 10 R030→V025; 11 R014/016→V008/009; 12 R018→V011 | Actual burden, accessibility, resident/worker experience |
| 8 Constitutional mediator | 13 R012/029→V008/021; 30 R002→V002 | Empowered human constitutional judgement |
| 9 Compliance as consequence | 13 R010→V007; 10 R027→V023; 25 R005→V003 | Full purpose-led design and competent legal/practice evidence |
| 10 Complexity/emergence | 12 R022→V014; 13 R013/025→V009/018; 25 R011→V008 | Cross-system and longitudinal evidence; no assured-whole claim from assured parts |

## Appendix B — Individual RP v6 source review

All 41 source principles are considered below in the source matrix's existing order and opening-phrase identification. Row numbers are local review indexes, not invented RP source IDs. `Contribution` identifies available links; `Counterpart` indicates that the central obligation belongs elsewhere and the domain supplies supporting evidence or preserves a boundary. `Partial` retains a specific gap. Exact scope/legal/institutional sufficiency is not inferred.

| Review row | RP domain / source opening | Review contribution / current boundary |
| --- | --- | --- |
| 1 | Architecture and Completeness: Every governance process must close its feedback loop. | Contribution: 13 R027/028→V020/021; 10 R021→V018; 30 R036→V022. Actual outcome remains distinct from dispatch. |
| 2 | Architecture and Completeness: Every human accountability layer must be explicitly named, sequenced, and time - bounded before any process is consid... | Contribution: 13 R016–018→V011/012; 30 R021/022/048→V013/031. Names, windows and capacity are commissioned dependencies. |
| 3 | Architecture and Completeness: Every option set must include the option that cannot be made to work. | Counterpart: 30 R005→V003; 10 R023→V019 supplies constraints. Full option preparation remains 22; not a Boundary decision. |
| 4 | Architecture and Completeness: The ‘AI said so’ test must be passable at every decision point. | Contribution: 12 R005/006→V004; 30 R016→V010. An operative model result plus signature fails the human-rationale test. |
| 5 | The Mode 1 / Mode 2 Boundary: Mode 2 is permanently human. | Contribution: 12 R005→V004; 13 R024→V017; 30 R002→V002. Permanent human judgement retained. |
| 6 | The Mode 1 / Mode 2 Boundary: Every Mode 1 boundary is a governance instrument, not a technical setting. | Counterpart: 01 authority and 30 R019→V012; 13 R001/002→V001/002 consumes approved/applied definitions. No numeric defaults. |
| 7 | The Mode 1 / Mode 2 Boundary: The boardroom is a Mode 2 deliberative space. | Contribution: 30 R006/007→V004; all domains preserve the protected-boardroom boundary in §8/Appendix A. |
| 8 | The Mode 1 / Mode 2 Boundary: The Mode 1/Mode 2 boundary is under continuous pressure from AI capability growth. | Counterpart: 25 R008→V005 and 30 R038→V023; domains research capability claims but cannot reclassify Mode 2. |
| 9 | The 1+5 Architecture: Every proposed governance mechanism must be tested against the 1+5 structure to confirm which layer it belongs to and... | Contribution: domain §§1/3 identify all five boundaries; 13 R024→V017 preserves coordination versus adjudication. DEC-005 controls placement. |
| 10 | The 1+5 Architecture: Risk is intrinsic to each intelligence layer, not a separate domain. | Partial: 10 R022→V008; 12 R029→V019; 13 R009/010→V007; Boundary CAP008/FUN009 lacks full numbered allocation (CR01). |
| 11 | The 1+5 Architecture: Every intelligence layer boundary where welfare - adjacent or safety - adjacent signals may arise must have an explic... | Contribution: 10 R011/020→V008/017; 11 R039→V021; 12 R029→V019; 13 R016–020→V011–014. Exact route/window/cover remains commissioned. |
| 12 | The 1+5 Architecture: The Golden Thread obligation under the Building Safety Act 2022 is not a technical data management requirement. | Contribution: 10 R024–026/047→V020–022; 40 V036. Board governance and statutory dutyholders remain distinct; legal applicability not validated here. |
| 13 | Options and Decisions: Options generated by the architecture must be grounded in the organisation’s actual state — actual covenant condition... | Contribution: 10 R023→V019; 12 R025/027→V016/017 supplies actual constraints. 30 R005→V003 preserves full options; 22 remains preparation owner. |
| 14 | Options and Decisions: Every consequential decision must feed back into the Unified Data Layer as a structured record — not only the decisio... | Contribution: 13 R028/048→V021/035; 30 R013/014/036→V008/009/022. DEC088 requires human-provided/confirmed context, not inferred deliberation. |
| 15 | Options and Decisions: Revealed preferences from real decisions take precedence over stated preferences in policy documents when the archite... | Counterpart: 30 R014/015→V009; 25 R015→V011. Descriptive preferences do not authorise calibration; DEC018/088 retained. |
| 16 | Blind Spots and Honesty: The architecture must name what it cannot see. | Contribution: 10 R004/048→V003; 13 R005→V004; 25 R003/012→V002/009. Boundary overall coverage remains CR01/03. |
| 17 | Blind Spots and Honesty: The dynamic risk perimeter question must be asked at board level as a standing agenda item: not only ‘what are our ri... | Partial/counterpart: 25 R003/012→V002/009 supplies perimeter evidence; Boundary gap/risk sensing and actual board standing-agenda treatment need exact allocation, not just a quiet feed. |
| 18 | Blind Spots and Honesty: The interaction of intelligence layers produces system - level behaviours that no individual layer would produce alone. | Contribution: 12 R022→V014; 25 R011→V008; 40 V027/037/038. Actual cross-system evidence remains absent. |
| 19 | Ethics and Telos: Every process must demonstrate a traceable relationship to the organisation’s ethical commitments and social purpose. | Contribution: 13 R001→V001; domain §8 purpose/ethics applications; full individual-process purpose derivation remains source-allocation work CR03. |
| 20 | Ethics and Telos: The architecture must be capable of detecting purpose drift — the condition where operational processes have graduall... | Counterpart: 25 R006/007→V004; domains supply actual outcomes, e.g. 10 R021→V018 and 13 R028→V021. |
| 21 | Ethics and Telos: Diversity, inclusion, and equitable outcomes are not separate compliance obligations. | Contribution: 11 R014/016→V008/009; 12 R016/028/031→V010/018/021; 25 R013→V010. Actual equitable outcomes need human/longitudinal evidence. |
| 22 | Ethics and Telos: Where the organisation’s welfare obligation to residents and its consent architecture pull in opposing directions, th... | Contribution: 11 R035–039→V019–021; 30 R002/003→V002. No invented emergency power or silent consent override. |
| 23 | Ethics and Telos: AI systems have function, not telos. | Counterpart: 25 R006→V004; 13 R029→V021 preserves function versus purpose. Human constitutional mediation remains 01/20/30. |
| 24 | Ethics and Telos: Where the organisation's purpose is interpreted through an accumulating body of AI-mediated rulings rather than appli... | Counterpart: 25 R007→V004; 30 R037/038→V022/023. Domain operational memory creates neither approved precedent nor telos amendment. |
| 25 | Ethics and Telos: Every AI system deployed by the organisation carries an embedded constitutional framework established by its developer. | Counterpart: 25 R010→V007; 12 R038/039→V025/026 supplies provider/model evidence; full developer-framework assessment remains shared/GI ownership. |
| 26 | Ethics and Telos: The no - exit condition is a constitutive feature of the organisation’s moral architecture, not background context. | Contribution: 11 R014–016/030→V008/009/016; 12 R018/028→V011/018. Listening or proxy satisfaction does not prove legitimacy. |
| 27 | Ethics and Telos: Compliance is the output of sound governance design, not its objective. | Contribution: 13 R010→V007; 10 R027→V023; 25 R005→V003. Competent legal and actual practice evidence remains separate. |
| 28 | Radical Transparency: If you cannot audit it and be held accountable for it, it cannot be done. | Contribution: 10 R037→V018; 12 R043→V029; 13 R048→V035; core REC evidence. No private chain-of-thought required. |
| 29 | Radical Transparency: The architecture must be more transparent than the document - based governance it replaces, not less. | Partial: the above reconstructability links and 11 R013/014→V008 support scrutiny; comparative transparency versus prior document governance is not proved by documentation alone. |
| 30 | Radical Transparency: Transparency obligations extend to the architecture’s uncertainty. | Contribution: 10 R009/010→V007; 11 R011→V006; 12 R024→V015; 13 R008→V006. Actual fidelity/recipient comprehension remains evaluated. |
| 31 | Agentic Delegation: Agents operate under explicitly delegated authority, not implied authority. | Contribution: 13 R011/012→V008; 10 R012→V009; 12 R037→V025; Boundary commitment functions require numbered migration. |
| 32 | Agentic Delegation: Agent authority is domain - specific, context - specific, and condition - specific simultaneously. | Contribution: 13 R003/011/012→V003/008; 12 R003→V003. Exact task, domain, recipient, context and conditions travel to enforcement. |
| 33 | Agentic Delegation: Agents cannot commit the organisation to external obligations, initiate unsolicited contact with external parties, or... | Contribution: 14 FUN004/INV002/CR002 and 13 R011/012→V008; shared 01/03 controls. Boundary core numbered allocation remains CR01. |
| 34 | Agentic Delegation: Internal escalation — routing a signal within the architecture to a human reviewer or to a receiving intelligence lay... | Contribution: 10 R020→V017; 13 R016–020→V011–014. Separately permitted internal routing remains distinct from unsolicited external contact. |
| 35 | Agentic Delegation: The agentic delegation framework is a governance document reviewed by the board, not a technical configuration manage... | Counterpart: 30 R019→V012; 01 authority instruments; 13 R001/002→V001/002 consumes them. Agent capability is not governance approval. |
| 36 | Agentic Delegation: Every agent action must satisfy the ethics and telos test and the radical transparency test independently of the proc... | Contribution: 13 R001/048→V001/035 and domain authority/purpose constraints. Full ethics/telos and transparency source chains remain CR03. |
| 37 | Agentic Delegation: Certain classes of finding must reach their required audience regardless of any instruction to suppress or delay them. | Contribution: 12 R030→V020; 13 R019→V013; 30 R025/026→V015; common protected-reporting route. Actual independent delivery not yet demonstrated. |
| 38 | Data and Sensing Boundaries: Sensing must not exceed its declared purpose. | Contribution: 10 R028/029→V024; 11 R031/033→V017/018; 12 R001/026→V001/016; 13 R042→V030. Boundary data use inherits 03. |
| 39 | Data and Sensing Boundaries: The boundary between observing an asset and monitoring a behaviour is an absolute architectural boundary, not a matte... | Contribution: 10 R028/029→V024; 11 R033→V018; 12 R036→V024. Asset observation is not behavioural permission. |
| 40 | Data and Sensing Boundaries: Where behavioural inference from sensing data is genuinely necessary to serve the resident’s interests — energy pover... | Boundary retained, not activated: 10 R029→V024; 11 R033/035–039→V018–021. Separate behavioural-inference purpose needs its own explicit governed scope/necessity/consent/review; current drafts authorise none. |
| 41 | Data and Sensing Boundaries: The purpose limitation principle applies across all intelligence layers, not only to resident - facing sensing. | Contribution: 12 R026/036→V016/024; 13 R042→V030; 10/11 purpose controls. Product-internal integration cannot broaden purposes; Boundary full allocation remains CR01. |

## Appendix C — All 29 GT contributions and human boundaries

The four complete domain appendices supply the following planned-case contributions. Case references use the component prefix, e.g. `10 V019`. This table reproduces the declared applicability rather than asserting the adequacy of every case. Exact REQ links are recoverable through each cited case's Requirements field and the reciprocal register check. Boundary has no full 29-test appendix: its core applicability remains SENS-CR-01/03. AOS-40's Appendix A retains the institutional assessment framework.

Every institutional GT status remains **not assessed**. Human board/independent judgement, actual operating consequences and longitudinal evidence cannot be supplied by a passing software case or by this review.

| GT / controlled title | Asset planned contribution | Resident planned contribution | People planned contribution | Process planned contribution |
| --- | --- | --- | --- | --- |
| M1.1 Strategic Coherence | Condition/investment scenarios; 019 | Participation/actual service context;016/033 | Capability/workforce change outcomes;018/034 | Purpose/actual consequences; 001/020/040 |
| M1.2 Sensing Architecture | Observation scope/coverage/failure; 001–007/029 | Private/enterprise/coverage scope;003/006/017 | Role/listening scope/coverage;001/012/017 | Population/coverage/perimeter; 003/004/006 |
| M1.3 Risk Intelligence | Physical concern and owned referral; 008/017/019 | Permitted human welfare route;019–021 | Workload/safety/protected route;016/019/020 | Obligation/divergence/accepted route; 007/011–014 |
| M1.4 Composition and Capability | Competent inspection/assessor role dependencies; 006/020/028 | Accessibility/competent human dependencies;008/025 | Framework/literacy/manual competence;006–009 | Human acceptance/role dependencies; 011/012/028 |
| M1.5 Performance Legibility | Condition/work/outcome distinction; 004/018/019 | Delivery versus service/remedy;012/015/033 | Activity/capability/outcome distinction;007/034 | Actual versus intended/outcome; 005/020/026 |
| M1.6 Compliance Assurance | Applicable source/category/standing; 020–023 | Current source/applicability profiles;014/029 | Current standard/profile/provider scope;006/035 | Obligation/source/claim distinction; 007/040 |
| M1.7 Governance Documentation | Current version and lineage; 002/021/026 | Versioned selected record/outcome;023/027 | Exact framework/charter/policy versions;006/010/035 | Versioned definition/rationale/history; 001/021/035 |
| M1.8 Accountability Architecture | Accepted duties and challenge; 016/017/022 | Both contacts/accepted routes/challenge;011–016 | Human owner/challenge/protected route;004/005/020/022 | Tracker/cover/contact/challenge; 011/012/025–028 |
| M1.9 Value for Money | Condition/resource alternatives; 019 | Service burden/outcome evidence;008/015/033 | Human development/workload alternatives;007/016/018 | Actual constraints/capacity/alternatives; 009/017 |
| M1.10 Human-AI Interaction Norms | Action/human boundaries; 009/019/024/033 | Boundaries and human alternative;003/008/021/022 | Substantive human professional/personnel judgement;003/004/008 | Exact delegation/human roles; 008/017/028 |
| M1.11 Learning Metabolism | Actual outcome versus forecast; 007/018/028 | Actual remedy/feedback;015/016/033 | Actual learning/capability consequences;007–009/034 | Outcome/near-miss/memory; 020/021/026 |
| M1.12 Continuous Self-Assessment | Coverage and research; 003/031–033 | Coverage/research limits;017/028–031 | Coverage/dependency/research review;009/017/030–032 | Coverage/independent/research; 004/036–040 |
| M1.13 Emergent System Behaviour | Aggregate gaps/distribution/compound failure; 003/019/029 | Shared-product and unequal access effects;017/026/032/033 | Repeated disclosure/dependency/unequal effects;014/021/028 | Concurrency/partial/cumulative effects; 009/015/018/033 |
| M1.14 Golden Thread Integrity | Inventory/currency/usable transfer; 020–022 | Grounded property explanation;006/013 | Competent staff/provider support evidence;006/035 | Source-domain safety/actual work; 022–026 |
| M2.1 Values Architecture | Purpose/use/no-exit boundaries; 009/024/025 | Private/no-exit controls;003/009/024 | Purpose/listening/refusal barriers;001/010/011 | Purpose/protected/continuity controls; 008/013/014/030 |
| M2.2 Coherence Under Pressure | Safety uncertainty and competing constraints; 008/019 | Uncertainty/safety and consent;006/019/021 | Protected concern under pressure;019/020 | Suppressed concern/edge case; 013/014/040 |
| M2.3 Incommensurable Trade-off Capacity | Preserved alternatives; 019 | No automatic moral adjudication;021/033 | Development/transition alternatives;007/018 | Technical ordering preserves human priority; 017/028 |
| M2.4 Epistemic Brake Function | Gaps/conflict/unknown completion; 003/005/007/014 | Gaps/fidelity/referral;006/007/025 | Novelty/quiet output/uncertain benchmarks;009/017 | Missing/novel/unknown evidence; 004/007/015/040 |
| M2.5 Directorial Independence | Unfiltered uncertain asset evidence; 019/021 | Unfiltered resident challenge;014/016/033 | Independent review and dissent;005/020/021 | Independent required audience; 013/029/040 |
| M2.6 Social Legitimacy | Resident challenge/manual route; 016/025 | Accessible feedback and actual remedy;008/014–016 | Worker/tenant input and actual action;010/012/035 | Resident challenge/actual remedy; 025–027 |
| M2.7 No-Exit Obligation | No optional-sensing penalty; 024/025 | Optional refusal/non-digital help;008/009/016 | Optional refusal/access/protected routes;011/020/022 | Continuing service/private/worker scope; 014/027/028/030 |
| M2.8 Radical Transparency | Evidence/inference/limitations; 002–007/018/021 | Selected/private and meaningful reasons;005/010/027 | Source/rationale/suppression limits;002/015/029 | Actual source/check/effect/reasons; 003/005/035 |
| M2.9 Moral Drift Detection | Distribution/outcomes and research; 018/019/028/031 | Distribution/coverage/actual outcomes;017/033 | Dependency/unequal consequences;009/021/034 | Cumulative/divergence/learning; 009/021/034/040 |
| M2.10 Purpose Stability | Purpose-bound physical evidence; 001/024/033 | Purpose and permission separation;003/017/022 | Purpose-bound people uses;001/025/032 | Purpose/current permission/change; 001/008/010/038 |
| M2.11 Murmuration Capacity | Permitted evidence to independent human review; 019 | Permitted inputs to independent humans;016/033 | Permitted human inputs/dissent;010/020/034 | Permitted independent human inputs; 013/017/029 |
| M2.12 Constitutional Authority | No authority by inference; 009/019/033 | Human welfare/amendment boundary;021/022/031 | Human judgement/charter change controls;004/025/032 | No powers from workflow; 008/017/038 |
| M2.13 AI Constitutional Framework Governance | Model-change and permitted-inference evidence; 024/028 | Provider paths/model change;003/024/025 | Provider/bias/change evidence;021/025–027 | Model/runtime/quality/change; 008/032/034 |
| M2.14 Purpose-Led Design | Source/purpose derivation and limitations; 001/019/030 | Source/purpose/supplier mapping;001/032 | Source/purpose/supplier derivation;001/033 | Source/purpose/supplier derivation; 001/039 |
| M2.15 Telos / Function Distinction | Physical optimisation versus human allocation; 019 | Service outcome versus proxy optimisation;015/033 | Workforce optimisation versus actual purpose outcomes;018/034 | Efficient process versus actual purpose outcome; 020/026/040 |

Institutional residuals include strategy and purpose coherence; board composition and genuine independence; ethical trade-offs and constitutional judgement; resident/worker legitimacy and lived burden; actual legal and building-safety fulfilment; independent human sense-making; capability, learning and cumulative effects over time. These remain explicit in the domains' third appendix columns and AOS-40's institutional assessment boundary. Golden Thread software custody, competent statutory dutyholders and board governance accountability are distinct.

## Appendix D — Retrieval and validation record

All reviewed document contents were retrieved from the identified OneDrive source items on 9 October 2026. Fresh reading copies retain the original contents and names with `.txt` extensions in the access-workaround folder. Historical notices were interpreted using current document-control/addendum standing; contradictions were retained as findings rather than resolved by assumption. The access aids must be refreshed from the canonical originals after subsequent changes.

The review performed identifier/count, main-section, 29-GT-row and declared reciprocal-link checks. AOS-14's abbreviated numeric tables were considered within their expressly limited research/supplier scope. Human/executable configuration, legal source verification, source-byte fingerprints against the original manifest, assurance-case execution and independent assessment were not performed. No diagram, narrative walkthrough or structural result is execution evidence.

## 9 October Boundary remedy assessment — report v0.2

The original review body describes the v0.1 assessed baseline and remains historical evidence. Mark subsequently requested AOS-14 completion. Codex migrated the core into55 proposed REQs/34 planned VERs preserving original001–009/001–007; all80 source items now have Boundary contribution/residual rows. Added typed disposition mapping, complete logical contract duties, owned gates, exact retained-anchor migration, manual/combined/supplier paths and assembled repair case. Supporting records updated as in the current opening notice. Total sensing is now269 proposed REQs/176 planned numbered cases (10–13 unchanged214/142); counts establish document coverage only.

| Finding | Current author disposition / evidence | Residual boundary |
| --- | --- | --- |
| SENS-CR-01 | Corrected at functional-document level;14 §§4.6/15.5/19.2/AppendixA;55/34/80 and retained-anchor/reciprocal checks | Substantive independent review, scoped decisions and implementation evidence remain; no operating conformance |
| SENS-CR-02 | Partial Boundary remedy; Shared4.7 and both9October adoption addenda | Other10–13 view and whole-suite counterpart completeness remain open |
| SENS-CR-03 | Partial Boundary remedy; Matrixv0.16 individual80-source addendum | Other domains/current original allocation and source sufficiency remain open; historical statuses preserved |
| SENS-CR-04 | Partial Boundary remedy; OQ013 resolved naming, OQ012 deferral, current40 scoped claims and historic notices clarified | Other components obsolete status/baseline passages remain open |
| SENS-CR-05 | Corrected at functional-document level;14§6.1 authoritative typed mapping mirrored common adoption | Concrete approved enum/schema/profile/compatibility validation and actual enforcement remain commissioning gates |

These are author document remedies, not separate quality/design assurance. Remaining material Boundary issues are owned/gated in14§17.1. No40 requirement/case, prior architectural decision or scheduled pilot was changed; no case executed.

## Approved Boundary decision adoption — 9 October 2026

| Approved decision / subject | Direction / rationale | Affected Boundary records | Approval and standing |
| --- | --- | --- | --- | --- |
| AOS-00-DEC-092 — Consequential external exchange | An external exchange is consequential when it can create or change an organisational commitment, disclose protected information, affect rights or service, trigger external action, or create a material obligation or risk. Materiality considers financial exposure and resource impact separately: payments, expenditure, liabilities or contingent exposure; and staff time, workload, capacity, equipment, facilities or other resource commitments and displacement of existing duties. Low monetary cost does not establish low resource impact. Record known quantities with their units/time basis and uncertainty; no invented money-to-time conversion or universal threshold. Apply organisation-approved criteria, including cumulative commitments. Routine public-information retrieval may use a lighter approved route only where its actual purpose, content and effects meet that profile. Uncertain classification goes to an accountable reviewer and cannot silently use the lighter route. | ISS-004; REQ-010–012/020–022/027/051; VER-008/012/016 | Mark;9October2026; Q1 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-093 — Outcome-specific exchange evidence | Define the required outcome and sufficient evidence for each exchange type. Sending, delivery, recipient acceptance and actual fulfilment remain distinct facts. Contractor receipt does not prove completed work. Where the required effect remains unknown, retain that standing and reconcile before retrying. An authorised person may close further investigation under the approved profile only with an explicit unknown outcome and retained owner/status of every outstanding duty; closure cannot become confirmed success. | ISS-005; REQ-029–032/036/053; VER-018/019/021/031/034 | Mark;9October2026; Q2 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-094 — Common external-obligation ownership | Use a common obligation record carrying source, applicability, exchange, responsible human owner, deadline where applicable, fulfilment evidence and current status. Boundary recognises exchange-associated obligations; relevant domain stewards determine substantive meaning and applicability under their authority; AOS-02 owns common record semantics; AOS-13 tracks accepted responsibility and fulfilment; AOS-30 supports accountable human disposition. Preserve financial and resource impacts separately where applicable, including unknown values. Uncertain or conflicting obligations go to an empowered human; automated recognition does not create legal authority or settle substantive meaning. | ISS-006; REQ-033–036; VER-020/021 | Mark;9October2026; Q3 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-095 — Operation-specific organisational boundary | Determine the boundary from organisational authority and control over the particular operation and data use. Hosting location alone is insufficient. A supplier system may carry out a delegated internal function while its onward disclosure or independent action crosses the external boundary. Each arrangement declares controlling parties, authority, operation/data-use scope, actual governed exchange points and independent shared-control enforcement. Ambiguous or missing control allocation remains an owned gap and withholds dependent consequential action. | ISS-007; REQ-010/011/026/047; VER-008/015/027 | Mark;9October2026; Q4 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |
| AOS-00-DEC-096 — Boundary patterns and system oversight | Boundary detects cumulative external-exchange patterns, including repeated disclosures, accumulating commitments, unusual counterparties, excessive restriction and attempts to evade controls by splitting actions. AOS-25 combines permitted Boundary signals with other domains to assess wider drift and emerging/system risks. Shared AOS-01/03/04/05 controls enforce approved limits and accounting; empowered humans decide policy/limit changes. Boundary cannot create a private budget, waive restrictions or adjudicate systemwide governance. | ISS-003; REQ-027/043–046; VER-016/025/026 | Mark;9October2026; Q5 agreed (Q1 with financial/resource clarification); approved architectural direction, exact component wording remains proposed |

These directions do not appoint organisational officers, select numerical thresholds, convert resource impact into money or certify external obligations legally. Shared owners retain their meanings and independent enforcement. Proposed component requirements and planned cases retain stable identities; an approved direction is distinct from G3/build or operating approval. The organisation-specific profile must state criteria and aggregation windows for financial and resource materiality; exchange-type expected effect/evidence and authorised unresolved closure; obligation field types/cardinalities/lifecycle and owners; operation/data-use authority and control points; and Boundary-versus25 pattern routing/triggers. Missing or invalid mandatory settings withhold dependent effects/reliance and retain an owned gap. No deferred federation activation or new source-status promotion is implied.

SENS-CR-02–04 remain open for the remaining whole-sensing common/source/status corrections. CR01/05 functional remedies remain recorded. Approved Boundary principles resolve the local general-design blockers; exact profiles and real evidence remain unverified. No historical assessment rewritten as contemporary execution.

## Final author sensing consistency closure — 9October2026 / reportv0.4

Baseline and authority: Mark requested remaining consistency corrections after approving Boundary DEC092–096. Current exact document versions appear in the opening notice. Inspected responsibilities, common masters and all CON definitions; traced repair promises/unknown-completion/accepted human duty/agreed-channel contacts/actual outcomes; challenged current authority/bypass/private and workforce uses, unknown external effects/retry/recovery and research ownership. No further material design decision was needed.

| Finding | Closure evidence / author conclusion | Remaining separate gate |
| --- | --- | --- |
| SENS-CR-01 | Closed:14v0.8 retains55/34, all original anchors and complete80-source navigation; core migration and approved directions preserved | Exact profiles, substantive/source sufficiency and independent/executed evidence |
| SENS-CR-02 | Closed: one current40-CON manifest in Registerv0.17, reciprocal component and Sharedv0.18 pointers, exact owner/producer/consumer/master/localREQ/VER/40 counterparts | Wire schemas and actual endpoint/control/acknowledgement compatibility |
| SENS-CR-03 | Closed: Matrixv0.18 all10FP/41RP/29GT current exact domain/Boundary/40 chains or explicit residual, accountable stewards and gates; all six component reverse navigation | Original source statuses preserved; statutory/institutional/source sufficiency and practice unassessed |
| SENS-CR-04 | Closed: current control fields/body pending-counterpart/source-allocation phrases corrected in10–13/40;14 current directions/issue standings retained; original notices and observations labelled historical | CAP01/02, commissioned capacity/schema/profile and actual evidence remain open |
| SENS-CR-05 | Closed: retained14 typed direction/operation mappings; shared/current manifest distinguishes custody/admission/truth/use/permission/escalation/quarantine and rejects invalid values | Exact wire enum/profile and actual control cases |

Coverage: all269 sensing proposed requirement and176 planned case identities retained;40 retains40/38; all40 logical views and80 source dispositions accounted for. Normative requirement statements and existing case acceptance conditions preserved; current references and added source/counterpart records do not create new permissions. Automated preservation/reference/reciprocal checks plus author semantic walkthrough support closure. Closure reviewer Codex9October, author review only. Independent review remains deferred, no cases executed, no G3/G4 or whole-suite legal/institutional conformance. Remaining setup, pilot5b, common executable work/item6, annex/case execution/item8, operating adoption/item9, supplier briefing12a and publication/reference-build tasks remain separate.

