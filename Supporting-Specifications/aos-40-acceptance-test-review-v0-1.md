# AOS-40 — planned acceptance-test review

Document: aos-40-acceptance-test-review-v0-1 · Source revision or record: v0.3

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**Current revision set:** AOS-00/Map v0.44; DEC-001–097; AOS-10v0.5/20v0.6/22v0.5/24v0.4/25v0.3/40v0.8; other components unchanged; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; acceptance annexv0.2; reviewv0.3.

**Current scope decision — 9 October 2026, DEC-097:** Mark has moved CAP-01 Trade-Off Divergence and CAP-02 Risk Register Assessment into Phase 2 as specific use cases built on AOS. They are outside the current architecture/specification completion scope and are not current build, acceptance or publication prerequisites. No use-case design, configuration, implementation or testing is scheduled now. DEC-017's architectural inclusion is superseded on this point; its original record remains history. General human judgement, evidence, data-use/authority, independent challenge and protected reporting controls remain in the architecture. Dedicated legacy use-case IDs are retained only as deferred trace references, with original wording parked in Phase 2 (deferred under DEC-097); mixed rows retain only their general architectural obligations in current scope. Earlier inclusion/next-task/annex-dependency statements are superseded.

Version: 0.3  
Date: 9 October 2026  
Requested by: Mark Sweeny  
Reviewer: Codex, author document review; not independent human assurance  
Status: review and authorised corrections complete; AT-CR-01–05 author documentary findings closed; all tests remain planned/unexecuted.

## 1. Current conclusion

AT-CR-01–05 closed at functional-document/author-review level. AOS-40 v0.7 retains40 proposed requirements and38 planned parent cases, with108 individually assessable variants in the controlled acceptance annex. All variants remain planned/unexecuted. Architecture/Mapv0.43; Sharedv0.19/Corev0.6/Registerv0.18/SourceMatrixv0.19; DEC001–096 unchanged. Original parent acceptance and local component obligations remain necessary. Exact approved current-core execution scope/endpoints/profiles, human appointments, implementation evidence and independent/institutional assurance remain separate dependencies. Pilot5b remains closed.

See §8 for the exact closure record and the [controlled acceptance annex](aos-40-acceptance-variants-and-coverage-v0-1.md). The original observations below are retained as the v0.1 review record.

### Original v0.1 conclusion — historical

AOS-40 v0.6 provides a sound functional assurance catalogue. Its 38 planned cases cover the main constitutional, authority, privacy, handoff, recovery, evidence and institutional-claim boundaries. All 40 proposed AOS-40 requirements have planned verification links; the 65 forward requirement–case associations agree with the 65 reverse associations. Every assembled case contains the required functional fields. Appendix A accounts for all 29 Governance Intelligence Tests without treating software results as institutional assurance.

The catalogue should be retained and refined. Five findings concern scenario assessment granularity and coverage, the latest Boundary decisions, private Resident participation, the independent GI challenge workflow, and one incorrect contract traceability association. Local component cases already supply much of the necessary behaviour; an assembled assurance plan must say exactly which local cases it inherits and what additional cross-component behaviour it observes.

**Specification quality:** structurally reviewable, with identified gaps in precise assembled allocation and assessable variants. Relevant gaps must be resolved before affected cases can substantiate an integration claim.

**Design adequacy:** the major boundaries are consistent with the agreed architecture. Additional explicit assembled fixtures are needed to demonstrate that the latest directions and specialist workflows survive their full producer/consumer paths. This is an author assessment of planned logic, not proof of technical feasibility or operation.

At the original review, item8 remained open for corrections. Those five remedies are now applied; annex-dependent coverage and later preparation/execution remain open. No G3/G4, legal/institutional conformance, live activation or independent-review conclusion follows. Mark's acceptance of research pilot 5b is retained and is not reopened.

## 2. Scope, baseline and method

Primary reviewed document: [AOS-40](aos-40-acceptance-integration-assurance-and-commissioning.md), v0.6, including all 38 §15 cases, requirements, shared case/evidence rules, issues, Appendix A and current adoption/source addenda.

| Baseline | Revision / reviewed role |
| --- | --- |
| AOS-00 / specification map | v0.42 / v0.42; approved directions DEC-001–096 and scope boundaries |
| AOS-01–05 | v0.8 each; authority, data semantics/use, lifecycle, runtime and local test registers |
| AOS-10 / 11 / 12 / 13 / 14 | v0.4 / v0.3 / v0.3 / v0.2 / v0.8; domain cases and current reciprocal adoption |
| AOS-20 / 21 / 22 / 23 / 24 / 25 | v0.5 / v0.6 / v0.4 / v0.5 / v0.3 / v0.2; GI case registers, protected independent preparation, presentation and oversight |
| AOS-30 | v0.5; human responsibility, board records, decisions and outcomes |
| Shared / Core / Exchange Register | v0.18 / v0.6 / v0.17; common meanings and current adoption |
| Coordination / Protected Reporting and Recovery / Operational Profiles | v0.2 / v0.1 / v0.1; races, reservations, continuity, human duties and repair fixture rules |
| Source Matrix / quality standard | v0.18 / AOS-QS v0.1; source contributions and QS-14–25 assessment criteria |
| Controlled principles/tests | FP v4, RP v6 and all 29 GT questions, as supplied controlled project sources; no new external conformity assessment |

Current OneDrive folder inventories were checked against the available working texts. Five GI texts not previously available locally were read through fresh plain-text access snapshots. Metadata/text-size comparison covered 32 available current source files, allowing extraction's terminal-newline normalisation. This is a currency check against the observed inventory, not a claim that byte size proves content integrity.

Method: detailed reading of every AOS-40 case; indexing the 18 component verification catalogues; targeted semantic comparison with specialist cases, contracts, decision fixtures, source contributions and QS criteria; mechanical checks of AOS-40 identifiers, required fields and reciprocal requirement links. The component catalogue inventory contains 698 numbered planned cases including AOS-40. These are not 698 independent scenarios: many kernel rows inherit the same shared KXV/KCV/KPV families. The review does not claim an exhaustive semantic audit of every component requirement or every possible combination.

## 3. What is already strong

- Repair criteria separate evidenced incomplete work from unverified completion, preserve the original promise and do not treat contractor closure or resident silence as a successful remedy.
- Receipt, accepted human responsibility, external effect and actual service outcome are distinct.
- Tests inspect observed enforcement/effects rather than accepting a model's refusal text as proof.
- Mode 2, boardroom exclusion, board-only telos change, Chair/board approval and independent reports are protected explicitly.
- Unknown effects, split budgets, revocation races, compound reporting failures and stale restoration have negative and recovery cases.
- Provisional findings, canonical meaning, source correction, uncertainty and bounded claims are retained.
- Probabilistic evaluation and longitudinal human governance assessment remain distinct from deterministic controls.
- Missing fixtures, rubrics, roles or authority are explicit dependencies; no production defaults are invented.

## 4. Original findings and recommended corrections — historical observations

### AT-CR-01 — Make variant results and assembled coverage explicit

**Class:** Major for affected verification scope. **Basis:** QS-21–23; AOS-40 REQ-002/005/009/014/026 and VER-001/002/005/025/036–038.

**Evidence:** The functional cases have inputs, procedures and expected results, but several combine many independently failing behaviours. VER-037 combines employment judgement, training/capability, repeated disclosure, manual professional competence and novelty; VER-038 combines almost the whole repair/control/recovery loop. VER-008 and VER-014 enumerate variants but do not give a per-variant result record. Common rules require scope/fixtures and §18 proposes a matrix; a current complete assembled requirement/component/contract/variant matrix is not supplied. A complete source contribution register is not the same thing as complete integration coverage.

**Risk:** A single scenario pass can conceal an unperformed branch, an assertion without evidence or a failure attributed to the wrong requirement. Referencing a component section does not identify which boundary interaction was actually assessed.

**Correction:** Keep existing VER IDs. Add controlled variant IDs under them, each with exact linked obligations, fixture, steps, observable expected results, assessor role and evidence. Define how variant results determine the bounded parent result: an in-scope required variant cannot disappear into a pass; blocked, failed and inconclusive contributions remain visible. Retain separate execution records when cases are eventually run.

Create a matrix linking the selected requirement → local component case → common view/revision and actual endpoints → assembled variant → evidence criterion → owner/gate. Mark inherited component-only evidence, added cross-boundary observation, exclusion and unresolved coverage separately. Do not force all 698 rows into new AOS-40 cases or duplicate shared test families.

Include contrasting valid/invalid controls. For example, pair prohibited incommensurable optimisation with a permitted commensurable comparison (20-VER-005/22-VER-009), and suspect precedent drift with genuinely authorised change (25-VER-004). For quality tests, approve the task population/rubric and distinguish false/missed findings and variability; an unexplained score or model confidence is not the oracle.

**Owner:** AOS-40 author with component/common-contract owners; Mark for any new material behaviour choice. **Closure evidence:** versioned matrix and variant definitions supporting every included assertion, with reciprocal links checked. Numeric settings and actual execution remain later gates.

### AT-CR-02 — Exercise DEC-092–096 across the assembled Boundary path

**Class:** Major for affected external-exchange scope. **Basis:** DEC-092–096; AOS-14 VER-008/018/020/021/025; AOS-40 VER-014/020/022/024/027/038.

**Evidence:** AOS-14 now defines the required decision fixtures, but AOS-40's listed assembled inputs do not explicitly reproduce them. Generic consequential classification, aggregate controls, unknown-effect and drift cases contribute, but do not themselves establish that financial/resource distinctions, obligation ownership and dynamic control-path meaning survive the assembled exchange.

**Correction:** Add explicit assembled variants or a separately identified assembled case inheriting the current Boundary cases:

| Direction | Required assembled contrast / observation |
| --- | --- |
| DEC-092 | Low monetary cost with substantial staff/capacity commitment; high financial exposure with little staff time; unknown and accumulated impacts. Preserve financial and resource measures separately; no monetary-only classification or unknown-as-zero. |
| DEC-093 | Sending, delivery, acceptance and fulfilment each have their own evidence. Include an empowered closure of investigation retaining an explicitly unknown outcome and accepted residual duty; do not label that fulfilment. |
| DEC-094 | Boundary recognises an obligation; the domain interprets its substance; 02 preserves common meaning; 13 tracks it; 30/humans accept/dispose of the duty. Preserve applicability, owner, deadlines where applicable and fulfilment evidence; contested obligations reach the empowered human. |
| DEC-095 | A supplier's delegated internal operation and its onward external disclosure have different controlled paths. Hosting or product boundaries alone cannot determine the organisational boundary. |
| DEC-096 | Repeated disclosure, financial/resource accumulation, unusual counterparties, split-action evasion and excessive restriction produce bounded Boundary evidence; 25 performs wider cross-domain oversight. Limits/accounting and human policy changes retain their own authority. |

Observe actual sender/consumer/control/outcome transitions through 14/02/domain/13/30/25, as applicable, with current 01/03/04/05 checks. The criteria are already approved architectural directions; the recommendation does not introduce new materiality thresholds, schemas or powers.

**Owner:** Boundary/domain, shared-record, Process, human-workflow and assurance owners. **Closure evidence:** exact current local-to-assembled case links, positive/negative fixtures and independently observable cross-boundary results. Keep profile approval and execution prerequisites explicit.

### AT-CR-03 — Demonstrate private Resident sharing and optional refusal end to end

**Class:** Major for affected private-assistance/enterprise-use scope. **Basis:** DEC-049–053 and domain limits; 03-VER-011/016/017; 11-VER-003–005/008/009/017/018/024; 13-VER-030; 24-VER-013/015/016. Existing AOS-40 VER-010/015/017/038 contribute.

**Evidence:** AOS-40 tests agreed channels, withdrawal, undeclared inference and a private-domain bypass. The explicit assembled fixtures do not fully specify a resident private session, exact selected sharing, subsequent downstream use and refusal without adverse core-service treatment. Local Resident cases contain this behaviour; generic privacy enforcement is not evidence that every consuming component retained it.

**Correction:** Define a positive exact-sharing route and negative full-transcript/cache/derived-use attempts. Carry the selected content, exact recipient, purpose and status through 02/13 and any permitted GI presentation/analysis recipients; exclude the remainder. Cancel or amend sharing before effect, change the agreed channel, refuse optional analytics and attempt a refusal-derived service penalty. Include an accessible human or representative route and preserve its verified scope. Show that independently valid core-service duties continue while refused optional use stops.

Judge both observable controls and human usability. Representative assessors must examine whether the resident understands what was shared and can challenge it; a successful message send is not accessible participation. Select exact resident/provider paths in the scope manifest, rather than assuming they all pass from one fixture.

**Owner:** Resident, privacy/use, Process, presentation and assurance owners. **Closure evidence:** explicit assembled variant definitions and consumer/effect evidence criteria linking the local cases. Actual usability and service outcomes remain unexecuted.

### AT-CR-04 — Demonstrate the independent GI challenge workflow through release and response

**Class:** Major for affected independent-preparation scope. **Basis:** 20-VER-010/012/013; 22-VER-017–019/022; 23-VER-018/019/022; 24-VER-019; 25-VER-019/020; 30-VER-015/024. AOS-40 VER-012/021/028 contribute.

**Evidence:** VER-028 clearly tests independently prepared annual/material-triggered human and GI reports. That is distinct from the independently governed preparation profile/window, executive tuning, presentation/release and management-response workflow. VER-021 tests protected reporting generally, but does not explicitly assemble the preparation-window conflict and its downstream duty states.

**Correction:** Use an independently approved exact preparation profile. Attempt executive retuning and unpermitted early access. During the preparation window, produce a mandatory protected concern and fail ordinary delivery; the separately permitted protected path must survive without creating extra disclosure powers. At the applicable release/response point, retain exact profile/status, missing management response, named accepted ownership and actual corrective-outcome duties. Report delivery or window expiry cannot complete the response duty.

Retain the separate annual/triggered independent-report test. A preparation window is neither unconditional secrecy nor universal early access; apply the actual approved purpose, audience and powers. A paired authorised normal path is necessary so the test does not pass merely by denying all release.

**Owner:** GI synthesis/assessment/presentation/oversight, human-workflow and assurance owners. **Closure evidence:** profile-to-production-to-release-to-response cross-boundary scenario with exact local links, evidence and failed-path ownership.

### AT-CR-05 — Correct the finding/review-duty traceability association

**Class:** Minor documentary association error; becomes a coverage blocker if used as the sole assessment allocation. **Basis:** QS-21; AOS-40 §6 CON-003, §4.3 and current reciprocal adoption table.

**Evidence:** The current adoption row for AOS-40-CON-003 “Finding and review duty” lists only AOS-40-REQ-014 → VER-001 in its local requirement/case column. REQ-014 is trace navigation. Its supporting-cases column lists VER-006/021, which actually exercise finding, remedy and protected duty behaviour, yet the corresponding local obligations are not in that column.

**Correction:** Reconcile the row with the contract's actual semantics and the existing requirements, including REQ-012/013 for finding/retest and REQ-016/022 where accepted responsibility/protected duties apply; retain REQ-014 for trace navigation. Update the single authoritative adoption manifest and its derived local/common/source projections together. Preserve all existing identities and meanings. Validate precise links rather than mechanically adding every nearby requirement.

This finding is a narrow association defect exposed by the acceptance review, not a withdrawal of all previously completed sensing consistency work. No failed implementation or new power is alleged.

**Owner:** AOS-40 and common adoption-register/source stewards. **Closure evidence:** coherent master/projection rows with exact reciprocal requirement/case links.

## 5. Per-case assessment record

All cases below were read. “Retain” means retain the functional definition for further planned work, not that the case has passed. AT-CR-01 applies to case/variant preparation throughout; the table highlights particular work without renumbering cases.

| AOS-40-VER | Assessment / next preparation |
| --- | --- |
| 001 | Retain scope/omission checks; supply the actual assembled coverage matrix under AT-CR-01. |
| 002 | Retain missing-prerequisite/false-pass cases; assess each invalid prerequisite separately. |
| 003 | Retain isolated effects and data lifecycle; include permitted and denied destinations with actual observation. |
| 004 | Retain truthful results; distinguish an observed control breach from an inconclusive missing observation. |
| 005 | Retain probabilistic/institutional separation; controlled evaluation variants/population/rubric under AT-CR-01. |
| 006 | Retain remedy/retest and original failure; correct CON-003 mapping under AT-CR-05. |
| 007 | Retain complete repair loop; evidence each contact, accepted duty and actual outcome separately. |
| 008 | Retain promise/date/completion contrasts; produce independent boundary and disputed/unknown variants. |
| 009 | Retain receipt/acceptance/absence/duplicate distinctions; separate each duty/deadline result. |
| 010 | Retain resident challenge/contact; expand private/optional/accessible path under AT-CR-03. |
| 011 | Retain document quality versus practice; pair missing/corrupt content with permitted valid inputs. |
| 012 | Retain canonical correction; join independent preparation/release path under AT-CR-04. |
| 013 | Retain impossible option and permanent human judgement; pair permitted commensurable comparison and blocked moral winner; CAP-01-specific detail deferred to Phase2 outside current core. |
| 014 | Retain authority/bypass matrix; add explicit Boundary/private route observations under AT-CR-02/03. |
| 015 | Retain withdrawal and no undeclared inference; complete selective private sharing/refusal path under AT-CR-03. |
| 016 | Retain minute-taker/steward/Chair/board states and exact changed revision. |
| 017 | Retain all supported capture/inference routes, including indirect/delayed capture; preserve permitted post-meeting input. |
| 018 | Retain board-as-body telos approval; distinguish record eligibility and applied state. |
| 019 | Retain formal schedule change and restricted reinstatement; no restart shortcut. |
| 020 | Retain concurrent limits/races; include approved financial/resource Boundary classifications under AT-CR-02. |
| 021 | Retain suppression/compound failure; add preparation-window protected duty under AT-CR-04 and map CON-003 under AT-CR-05. |
| 022 | Retain unknown/no-effect/partial-effect variants; add distinct Boundary outcome-stage/residual closure under AT-CR-02. |
| 023 | Retain isolated restoration/currentness/deletion/independent release; observe both denied and valid unaffected scope. |
| 024 | Retain entity/action-class separation; add operation-control rather than hosting classification under AT-CR-02. |
| 025 | Retain reciprocal meaning/correction; exact endpoint/variant selection and invalid-value dimensions under AT-CR-01. |
| 026 | Retain provider/location/framework/rollback; use exact approved variants without treating quality score as control proof. |
| 027 | Retain drift/quiet/emergence; pair authorised change with drift and Boundary/25 roles under AT-CR-01/02. |
| 028 | Retain both directions of report-preparation independence and human assessment; preparation-window workflow remains separate AT-CR-04. |
| 029 | Retain scoped gates and deferred separate reviewer; document checks supply no G3/G4. |
| 030 | Retain commissioned roles/capacity/accessibility/continuity; inherit explicit local measurements and human rehearsals through the matrix. |
| 031 | Retain own approved remit/profile and missing setup; does not reopen accepted pilot 5b. |
| 032 | Retain hostile-source/denied retrieval; observe attempted effect and resulting coverage/duty. |
| 033 | Retain status/jurisdiction/date/stale-baseline distinctions; no new legal conclusion from this review. |
| 034 | Retain no-finding/failed/partial/unperformed variants; separate false/missed-finding quality from enforcement. |
| 035 | Retain shared duties/urgency/human change; assess each owner and accepted-for-work versus amended state. |
| 036 | Retain building-information handover; split inventory, audience, transport/usability, correction and residual duty variants. |
| 037 | Retain People safeguards; split judgement, competence, disclosure and novelty variants; longitudinal deskilling remains separate. |
| 038 | Retain assembled Process repair loop; decompose duty/control/effect/outcome/recovery assertions and link exact Boundary variants. |

## 6. Component coverage navigation

This original review table identifies contribution areas. The controlled annex now supplies the parent/variant matrix and retained local inventory; actual execution-scope bindings and exclusions remain explicit gates.

| Component family | Numbered planned cases indexed | Main AOS-40 contributions / remaining distinction |
| --- | --- | --- |
| Kernel 01/02/03/04/05 | 44 / 49 / 51 / 57 / 64 | 003/014/015/018–026/030–035/038; exact identity, enforcement, lifecycle, credentials, failover, runtime observation and measured recovery remain local cases to inherit explicitly. |
| Sensing 10/11/12/13/14 | 34 / 33 / 35 / 40 / 34 | 007–010/013–015/020–027/036–038; AT-CR-02/03 address explicit assembled specialist paths. |
| GI 20/21/22/23/24/25 | 38 / 30 / 32 / 32 / 26 / 30 | 011–013/016/017/021/024–028/031–035; AT-CR-04 separates preparation-window challenge from independent annual/drift reports. |
| Human workflows 30 | 31 | 007–010/016/018/019/021/028–030/038; accepted scope, capacity/cover, actual outcomes and substantive judgement remain essential. |
| Assurance 40 | 38 | 40 requirements; 65 reciprocal local REQ/VER associations; cases supplement and do not replace component tests. |

## 7. Declared dependencies, not new defects

- Executable wire contracts, approved clocks/fixtures, scopes, thresholds, rubrics, assessors and implementation observability remain AOS-40 ISS-001–004/008. Their absence during drafting is not a failed system test.
- Institutional effectiveness, genuine independent reports, long-term drift, legitimacy and professional deskilling need permitted human/longitudinal evidence under ISS-005; synthetic examples cannot close them.
- Own research setup remains ISS-006; the completed pilot acceptance and each future component commissioning profile are distinct.
- CAP-01 and CAP-02 are parked Phase 2 use cases under item10/DEC-097; their dedicated requirements/tests no longer gate current architecture. General human judgement and risk/oversight controls remain current; ISS-007 retains only core applicability/detail gaps.
- Identity merge/split, HACT mapping, agent delegation/memory/retirement, provider failover, credential rotation, supplier exit, measured recovery and real human capacity already have local cases. The assembled plan must inherit and observe applicable interactions, rather than label these absent from the entire suite.
- Current document revisions and the 9 October controlling addenda govern. Earlier dated baseline references are historical; fix any stale active-reference labels during the next reconciliation without erasing history.

## 8. Corrections and author closure — 9 October 2026

Mark instructed application of all five corrections. The functional plan now incorporates the controlled annex and corrected master/projection associations.

| Finding | Status / exact remedy and closure evidence |
| --- | --- |
| AT-CR-01 | Closed, author documentary level: annex §§2–6 fixes108 unique variant IDs for all38 parent cases, fixtures/procedures/oracles, independent assertion/results and parent roll-up; exact65 parent REQ/VER joins, six common evidence views and660 retained local cases with exact local REQ links and owned scope gates. Original local cases and parent conjuncts remain necessary; unbound/local-only rows contribute no assembled pass. |
| AT-CR-02 | Closed, author documentary level: VER-038-B01–B08 explicitly exercise DEC092–096 financial/resource classification, outcome stages/unknowns, obligation ownership, operation/data-use control and Boundary/25 learning distinction, using exact AOS-14/13/25 counterparts. |
| AT-CR-03 | Closed, author documentary level: VER-015-R01–R06 cover private Resident selection/downstream use, optional refusal without core-service penalty, representative/human/accessibility channel, pre-effect cancellation and derived/cache leakage with exact local counterparts. |
| AT-CR-04 | Closed, author documentary level: VER-021-G01–G05 covers independent preparation/window/profile, faithful presentation/release, accountable response/actual outcome, executive tuning/early access and continuing protected duties/cover. Independent annual/material-trigger reports remain distinct in VER-028. |
| AT-CR-05 | Closed, author documentary level: master Registerv0.18/current AOS-40 projection corrected to AOS-40-REQ-012/013 → AOS-40-VER-006; AOS-40-REQ-014 → AOS-40-VER-001; AOS-40-REQ-016 → AOS-40-VER-009/021/038; AOS-40-REQ-022 → AOS-40-VER-021; Sharedv0.19/Matrixv0.19 reference that same definition. |

Validation: all40 original requirement rows and38 parent definitions/acceptance conditions preserved;65 reciprocal links unchanged;108 unique variants span all38 parents; every declared specialist local counterpart resolves in the current catalogues; the local inventory retains660 exact case/REQ rows. Master/current CON-003 projections agree. Architecture/Mapv0.43 records document allocation without changing DEC001–096. These are document and link checks, not executed acceptance.

**Remaining work:** CAP-01/02 use cases deferred under Phase 2/item10 and excluded from current-core prerequisites; approved scoped run matrix and exclusions, exact compatible wire contracts/endpoints and organisation profiles, fixture/rubric/assessor appointments, implementation and permitted execution, human/institutional evidence and empowered release/operating decisions. Item8 remains open for those later dependencies, not these five remedies. Independent project review remains deferred; pilot5b remains closed.

**Finding status:** AT-CR-01–05 closed at author functional-document level. **Execution status:** all cases/variants planned and unexecuted. **Review status:** author correction review complete; no independent assurance, G3/G4 or operational approval.

## Phase 2 scope disposition — 9 October 2026

DEC-097 controls over prior inclusion/annex statements. CAP-01/02-specific legacy requirements/cases are deferred and supply no current-core completion/acceptance obligation. General human judgement, independent challenge, evidence fidelity, cumulative risk/drift and protected reporting remain current. Existing closure of AT-CR-01–05 and pilot5b is retained; neither is reopened by this scope change. No case executed or operating approval granted.

**Allocation and source status:** Any older source/adoption row relying on deferred CAP-only IDs is a historical use-case contribution, not current-core coverage. Core source sufficiency must use the surviving general obligations and accepted evidence; no source is promoted by this deferral. Retained numbered totals count catalogue/trace entries, including deferred IDs, and must not be read as active-core requirement/test totals.

