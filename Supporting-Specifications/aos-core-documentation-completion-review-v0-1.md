# AOS core documentation — final author completion review

Document: aos-core-documentation-completion-review-v0-1 · Source revision or record: v0.1

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

Version: 0.1  
Date: 9 October 2026  
Requested by: Mark Sweeny  
Reviewer: Codex; author document review, not independent human assurance  
Status: review complete; items6/8/9 closed for functional drafting/planned allocation only.  
Authority: existing DEC-001–097; no new design decision or approval of proposed requirement wording.

## 1. Conclusion and exact completion boundary

The current functional component suite, common logical-contract allocation and planned acceptance catalogue meet the recorded documentary completion criteria for to-do items6,8 and9. Close those drafting tasks at author-review level. This means the proposed architecture is documented for substantive review, with explicit unresolved dependencies. It does not declare every source obligation fulfilled, every implementation interaction covered, complete executable schemas, whole-document approval, achieved G3/G4, independent assurance or permission to operate.

CAP-01 Trade-Off Divergence and CAP-02 Risk Register Assessment are specific Phase2 use cases under DEC-097, outside current architectural completion. The twelve dedicated component requirement entries and seven local case entries remain deferred identifiers, not active-core obligations or acceptance. The two former AOS-00 inclusion requirements038/039 are separate deferred parent identifiers and are not counted in the18-component totals below. General human judgement, evidence, independent challenge and protected reporting remain in core scope.

This review closes the functional workstreams. It does **not** declare the entire documentation/publication programme finished: extension/conformance specification (item12), supplier briefing (12a), AOS Change Constitution (13a), public-package preparation (13) and website publication (14) remain outstanding. Mark's substantive review remains distinct from this author assessment.

## 2. Baseline, scope and method

Reviewed baseline: AOS-00/Mapv0.44, DEC001–097; kernel01–05v0.8; sensing10v0.5/11v0.3/12v0.3/13v0.2/14v0.8; GI20v0.6/21v0.6/22v0.5/23v0.5/24v0.4/25v0.3;30v0.5;40v0.8 with acceptance annex internalv0.2; Sharedv0.20/Corev0.6/Registerv0.19/Matrixv0.20; Coordinationv0.2/KPRv0.1/Profilesv0.1; FPv4/RPv6/GT and AOS-QSv0.1.

Completion reconciliation changes only navigation/status/current baseline statements: AOS-00/Mapv0.45; Sharedv0.21/Registerv0.20/Matrixv0.21. Component requirements, planned cases, contract meanings, source statuses, DEC001–097 and the Phase2 record remain unchanged.

Observed current OneDrive inventories were compared with available current working texts; all matched recorded byte sizes, allowing extraction's terminal-newline normalisation. The recently changed Phase2 and acceptance originals had also been read back and compared in full. Size currency is supporting evidence, not a content-integrity or truth guarantee. The method combined reading of current common/scope/adoption/acceptance records and prior closed kernel/GI/sensing findings, targeted semantic boundary checks, and indexing every numbered requirement and case in the18 component catalogues. It is not an independent exhaustive semantic assessment of every assertion or all possible combinations.

Author checks: active requirement→defined planned case; declared primary links appear in reverse case links; identifiers resolve; Phase2 exclusions preserve general core obligations; current AOS-40 original acceptance plus variant definitions and human/evidence boundaries; common owners, producer/consumer/view navigation and owned dependency gates; task done-when criteria. Numerical requirements/cases below are catalogue entries, not independent tests or implemented functions.

## 3. Documentary task dispositions

| Task | Recorded completion criterion | Evidence and disposition |
| --- | --- | --- |
| 6 — Shared authority, data and agent contracts | Producers/consumers reference the same contracts; unresolved parameters have owners and no invented defaults | Corev0.6 defines REC-E/A/D/X and linked REC-Q; Shared defines original IFs and companion meanings; Register§§4–13 and15–20 plus sensing manifest allocate common views, authoritative owners and reciprocal endpoints; coordination/protected-recovery/research supplements define logical changes/acknowledgements/duties. Parameters remain owned in P/ISS/profile registers. Closed for functional contract definition/allocation; executable schema/compatibility evidence tracked in11a/11b. |
| 8 — Acceptance scenarios | Inputs, expected behaviour, human responsibilities and retained evidence identified | AOS-40v0.8 retains40 requirements/38 parent cases/65 exact reciprocal links; annexv0.2 supplies108 independently assessable variants with inherited original acceptance, methods/assessors, evidence rules and fixed result-vector limits. All29 GT questions have bounded software/human applicability. Active local requirements have planned cases; retained local-only rows are explicitly not assembled evidence. AT-CR-01–05 remain author-closed. Closed for planned functional definition; exact run-scope/endpoint bindings and execution remain11a/11b. |
| 9 — Five domain specifications | Responsibilities, permitted uses/actions, failure behaviour, acceptance criteria and consistent interfaces | All five sensing drafts exist and SENS-CR-01–05 are author-closed. Boundary requirement migration, DEC092–096 adoption, supplier allocation, source dispositions and common adoption exist. Sensing has269 requirement rows/176 planned cases; none deferred by CAP reclassification. Current private Resident, People, Asset, Process and Boundary boundaries checked against shared control owners and AOS-40. Closed for functional drafting/author consistency; Mark review, appointments and actual service/implementation evidence remain separate. |

## 4. Component requirement and planned-case coverage

| Component | Retained requirement rows | Current-core requirement rows | Retained case rows | Current-core case rows | Primary planned allocation check |
| --- | --- | --- | --- | --- | --- |
| AOS-01 | 68 | 68 | 44 | 44 | No uncovered active requirement or missing primary case link |
| AOS-02 | 73 | 73 | 49 | 49 | No uncovered active requirement or missing primary case link |
| AOS-03 | 68 | 68 | 51 | 51 | No uncovered active requirement or missing primary case link |
| AOS-04 | 77 | 77 | 57 | 57 | No uncovered active requirement or missing primary case link |
| AOS-05 | 76 | 76 | 64 | 64 | No uncovered active requirement or missing primary case link |
| AOS-10 | 49 | 49 | 34 | 34 | No uncovered active requirement or missing primary case link |
| AOS-11 | 55 | 55 | 33 | 33 | No uncovered active requirement or missing primary case link |
| AOS-12 | 53 | 53 | 35 | 35 | No uncovered active requirement or missing primary case link |
| AOS-13 | 57 | 57 | 40 | 40 | No uncovered active requirement or missing primary case link |
| AOS-14 | 55 | 55 | 34 | 34 | No uncovered active requirement or missing primary case link |
| AOS-20 | 57 | 56 | 38 | 38 | No uncovered active requirement or missing primary case link |
| AOS-21 | 48 | 48 | 30 | 30 | No uncovered active requirement or missing primary case link |
| AOS-22 | 52 | 44 | 32 | 27 | No uncovered active requirement or missing primary case link |
| AOS-23 | 52 | 52 | 32 | 32 | No uncovered active requirement or missing primary case link |
| AOS-24 | 40 | 39 | 26 | 25 | No uncovered active requirement or missing primary case link |
| AOS-25 | 48 | 46 | 30 | 29 | No uncovered active requirement or missing primary case link |
| AOS-30 | 48 | 48 | 31 | 31 | No uncovered active requirement or missing primary case link |
| AOS-40 | 40 | 40 | 38 | 38 | No uncovered active requirement or missing primary case link |

Totals: **1,016** retained component requirement rows, **1,004** current-core rows; **698** retained numbered cases, **691** current-core numbered cases. Twelve CAP-only component REQs and seven local cases are deferred. All1,004 active requirements have at least one primary planned case outside the deferred set. No declared primary requirement→case link lacks its reverse association; no referenced primary case or reverse requirement identifier is unresolved. The691 cases include38 AOS-40 parents; the108 variant records are additional granularity, not108 new parent cases. Shared KXV/KCV/KPV inheritance and overlapping cases are not independent samples.

AOS-01/02/04/05/20 cases additionally list54 existing requirement associations beyond their requirement tables' primary case columns. Those are supplementary case coverage, not broken primary links or54 new requirements. Their identifiers resolve. The source/case registries deliberately support many-to-many navigation; no false claim of identical primary and supplementary lists is made. AOS-40 itself has exactly65 forward/reverse associations.

This check demonstrates planned allocation and identifier coherence. It does not prove each linked test sufficiently assesses every normative assertion. Original component acceptance, common method/evidence prerequisites, competent human assessment and selected execution-scope validation remain necessary. Every unbound local-to-assembled row stays owned and supplies no assembled coverage; mandatory in-scope bindings cannot be waived by this documentary closure.

## 5. Responsibility, contracts and key scope boundaries

AOS-01 owns action/constitutional authority;02 common evidence/record identity/assurance/correction structure;03 identity/representation, lawful use/purpose/disclosure;04 agents/tasks/effect semantics/evaluation;05 independent runtime/check/accounting/recovery; domains own substantive service interpretation;13 tracking/accepted operational duty;14 external exchange;20–25 GI corpus/synthesis/assessment/presentation/oversight;30 empowered human decision/responsibility;40 evidence-supported assurance. No local CON view creates a competing semantic owner.

The33 original kernel CON views are mapped to common definitions, with common research views additionally inherited. Register§§12/13/15–20 gives GI/human/research adoption; the sensing/current40 manifest gives40 local CON views across10–14/40 with producer/consumer/shared owner and requirement/case contribution. GI/human tables use scoped short CON IDs under their component headings; absence of a fully prefixed string is not a missing definition. Actual endpoint compatibility, wire profiles, enums/cardinalities, clocks, confidentiality and independently observed application remain build/execution prerequisites.

Targeted boundary checks retained: financial versus resource materiality; send/deliver/accept/fulfil; Boundary recognition versus domain substantive obligation and02/13/30 duties; operation/data-use boundary versus hosting; Boundary patterns versus25 oversight; private Resident selection/refusal/accessibility/cancellation/derived leakage; People judgement and permissible disclosure; independent GI preparation/release/response/protected duties; exact Chair/board standing; permanent human Mode2; scope-specific reconciliation/recovery; outcome rather than administrative closure. These are checks of proposed documentary coherence, not observed system behaviour.

The80 controlled FP/RP/GT source items retain their existing allocated/partial/unresolved histories and current contributions. All29 GT questions retain actual human/institutional evidence boundaries. Source sufficiency and sector/legal applicability are not promoted by completion or Phase2 deferral. A deferred CAP-only source contribution cannot substantiate current-core coverage. Source manifest unchanged.

## 6. Findings and remedies completed in this review

| Finding | Remedy / author closure |
| --- | --- |
| FC-01 — To-do items6/8/9 still combine completed drafting, obsolete next steps and future implementation evidence | Replaced live task entries with current completion scope and evidence; preserved former entries in dated history; separated Mark review and11a/11b implementation/verification prerequisites. Closed, author documentary level. |
| FC-02 — Shared-contract initial-scope/adoption passages can appear to be current despite later completion supplements | Corrected current control/scope/next-action notices and labelled initial-review/adoption passages as historical; current register/common supplements govern. No contract dictionary or proposed requirement amended. Closed, author documentary level. |
| FC-03 — Navigation still needs a clear current-core completion versus Phase2/programme boundary | Added this review and exact completion disposition to README/architecture/map/source navigation; item10 remains parked, other architectural governance/publication work remains open. Closed, author documentary level. |

No new blocking functional-document defect was established by this bounded review. This does not mean all implementation, operational or substantive-assessment risks have been resolved. No previously closed acceptance/sensing/GI finding or pilot5b is reopened.

## 7. Remaining work and accountable gates

| Remaining work | Owner / gate | Why it remains |
| --- | --- | --- |
| Mark's substantive review/disposition of the core draft | Mark, item5d; exact proposed wording and affected decisions | Author completion is not project-owner whole-document approval. |
| Extension/conformance specification and supplier alignment | Project drafting owner/semantic owners; items12/12a, before claiming extension/product conformance or public supplier readiness | Core responsibilities exist; explicit extension obligation and claim model plus standalone supplier briefing remain programme work. |
| AOS Change Constitution | Project owner/governance drafting, item13a; before relying on proposed AOS change rights/process | Organisational control decisions do not by themselves complete governance of the architecture's own change process. |
| Bounded implementation slice | Mark/empowered organisation, item11; before build | Exact scope, omissions, technology/location, organisation instruments, threat assumptions and stop conditions require authorisation. |
| Implementation-specific contract and run matrix | Component/semantic/control/service owners with40, item11a; before dependent build/execution/reliance | Fixed compatible wire profiles/endpoints, approved values/clocks/roles/rubrics/fixtures/observability and mandatory variant/local-case bindings are needed. |
| Actual verification and commissioning | Competent appointed assessors, responsible organisation and service owners, item11b; before affected acceptance/release/activation | Cases are planned; actual effect, recovery, human capacity/accessibility, adverse scenarios and retest evidence remain absent. G3/G4 and operating approval stay separate. |
| Independent and institutional assurance | Separately empowered reviewers/organisation; required gate before claimed assurance/operation | Independent project review deferred; actual governance, legal/practice, safety, long-term outcomes and legitimacy cannot be certified through these document checks. |
| Publication package and website | Mark, items13/14, after selected package approval | Complete public status labels, licensing/contribution rules, release/exit criteria and approved publication still required. |
| CAP-01/02 use cases | Mark, Phase2/item10 only on explicit resumption | Outside current architecture; no date, current work or prerequisite. |

**Recommended next documentary task:** item12, extension and conformance specifications; then align the supplier briefing and AOS Change Constitution/publication package. This recommendation does not authorise a build, test execution or publication.

## 8. Final status

Items6/8/9: complete for functional drafting/planned allocation/author consistency. Components remain proposed review drafts. FindingsFC-01–03: author-documentary remedies closed. Tests: unexecuted. DEC001–097, source histories and manifest unchanged. Independent project review deferred. No whole-document approval, G3/G4, legal/institutional certification or live activation inferred.

