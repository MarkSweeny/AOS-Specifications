# AOS-30 — consistency and coherence review against the kernel and GI

Document: aos-30-kernel-and-gi-consistency-review-v0-1 · Source revision or record: v0.2

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

Date: 7 October 2026  
Version: 0.2  
Status: author functional-architecture review with authorised amendment disposition; CR30-01–03 closed.  
Requested by: Mark Sweeny. Independent project review remains deferred.

## 1. Conclusion

AOS-30 is coherent with AOS-01–05 and AOS-20 at the functional architecture level. No fundamental contradiction, missing governing power or competing component responsibility was identified in the reviewed material. The approved minute-taker/Company Secretary/Chair/board distinction is faithfully expressed in AOS-30 v0.2.

The initial review identified three limited documentary alignment points, now resolved by authorised amendments described in §7. They concern carrying AOS-30's settled meaning into earlier documents and making the correction-feedback connection explicit. They do not require executable schemas, detailed code lists, technology choices or organisation-specific appointments to be settled now. No new general design question is identified.

This review establishes consistency of the written functional design. It does not establish implementation correctness, institutional adequacy or readiness to operate.

## 2. Scope and evidence

Read the canonical OneDrive to-do list, updated 6 October, AOS-30 v0.2, AOS-01–05 v0.7, AOS-20 v0.2 and the current Kernel Exchange Register v0.7. The register's filename retains its original v0.1 suffix; its current content includes the AOS-30 approved-direction disposition. Earlier components retain the pre-AOS-30 decision baseline through DEC-086; AOS-30 and the register record DEC-087–089.

Review compared responsibilities, semantic exchanges, approval boundaries, ordinary/failure workflows, feedback and correction, privacy, protected reporting, independent review and external research. Detailed technical implementation and a fresh legal/standards assessment were outside scope. Common annexes were considered through the adoption declarations in these documents; this was not a new full review of those annexes or the source corpus.

Principal evidence: each component's §§3, 6, 7 and 9–14; AOS-30 §§4.3, 5, 15 and 17.1; AOS-20 §§4.3, 5 and 6.1; Exchange Register §§6, 14 and final approved-direction disposition. Requirement and planned-case references below identify supporting written provisions; cases were not executed.

## 3. Responsibility and behaviour comparison

| Relationship | Consistency finding | Main evidence |
| --- | --- | --- |
| AOS-01 authority / AOS-30 human workflow | AOS-30 records empowered human decisions and supports the approval sequence; AOS-01 determines instruments, powers and controlled activation. A recorded decision cannot manufacture authority. | 01 §§3/6.1/7/10.2; 30 §§3/7, REQ-008–012/017–020 |
| AOS-02 shared records / AOS-30 decision meaning | AOS-30 owns decision-account and accepted-duty semantics; AOS-02 owns shared structure, custody and governed lineage. Admission, truth, approval and actual effect remain distinct. | 02 §§3/5/6.1/10.4; 30 §§3/5/6.2/12 |
| AOS-03 identity and permitted use / AOS-30 participation | AOS-30 relies on verified capacity, purpose-bound input, approved disclosure and resident-agreed channels. Human approval does not remove processing restrictions. Descriptive feedback remains human supplied or confirmed. | 03 §§3/6.1/9/10.4; 30 §§7/9, REQ-014/015/017/031–035 |
| AOS-04 agent behaviour / AOS-30 instruction and feedback | Task assignment and human instruction confer no extra permission. Agents assist preparation and account structuring, but cannot perform Mode 2 adjudication or convert feedback into autonomous governing change. | 04 §§3/6/7; 30 §§4.2/7, REQ-002/006/007/015/028/037 |
| AOS-05 platform / AOS-30 continuing duty | The platform enforces controls and records actual effects; AOS-30 supports human acceptance, cover and outcome review. Outage, read receipt or restart cannot erase duty, establish service completion or restore withdrawn powers. | 05 §§3/6/10/11; 30 §§5/10.2/11, REQ-021–029/039/040/048 |
| GI preparation / human decision | GI owns substantive analysis, canonical meaning, validation and faithful presentation. AOS-30 coordinates the human workflow and records its disposition. Reviewed analysis remains distinct from a decision or action grant. | 20 §§3/6.1/10.1, REQ-021/022/024; 30 §§3/4.2/6.1/10.1, REQ-004/005 |
| GI corpus and oversight / human feedback | Decision storage is not automatic precedent admission. Interpretation approval and independent review remain separately empowered. Outcome feedback supports governed learning without reopening deferred self-calibration. | 20 REQ-010–012/034–036/045; 30 REQ-015/036–038, VER-022/023 |
| Protected findings and research | Both documents preserve permitted urgent reporting, accountable handoff, alternative recipients and distinct research remits. A finding or acceptance for further work cannot amend a specification or activate a change. | 20 REQ-029–033/037–046/053–057; 30 REQ-025/026/042–047; kernel research declarations |

The responsibilities of AOS-13 operational coordination, AOS-14 external exchange and AOS-11 resident relationships are preserved in AOS-30. Their detailed specifications were not reviewed here; their later drafting must adopt these boundaries.

## 4. Findings and proportionate recommendations

### CR30-01 — earlier adoption statements need updating

**Classification: documentary alignment; no behavioural contradiction.** AOS-20 §6.1 says detailed AOS-30 adoption remains pending its drafting, although AOS-30 now exists. Kernel/GI baseline declarations also precede the AOS-30 disposition. Conversely, AOS-30 §16 describes endpoints as mapped reciprocally, while Register §14 explicitly retains affected-consumer adoption work.

**Recommendation:** update present-tense status and dependency statements to identify AOS-30 v0.2 and DEC-087–089 as applicable to human-decision exchanges. Describe the register as mapping the intended logical producer/consumer relationships, with local adoption alignment still to be completed. Preserve historical baseline entries as history. This is a short document reconciliation, not a technical interoperability exercise.

### CR30-02 — make the board approval distinction explicit at the receiving boundary

**Classification: propagation clarification; settled design, no new decision.** AOS-30 §§5/6.2/10.3 and REQ-008–012 clearly distinguish minute-taker drafting, Company Secretary stewardship, optional Chair draft approval and board approval of the exact minutes and thereby the decision. The register's final disposition repeats this. Earlier AOS-01 CON-003 and AOS-20 CON-004 use generic empowered-approval language and do not themselves state the Chair/board distinction. They do not authorise a conflicting shortcut, but standalone reading leaves the later qualification implicit.

**Recommendation:** add a concise shared-reference clarification in AOS-01/AOS-02/AOS-20 decision-record participation, with applicable AOS-03/04/05 references: receiving a Chair-approved draft or certified extract is insufficient for authoritative reliance on a board decision; an extract refers to the exact board-approved source. Preserve different approval routes for non-board decisions. No duplicate schema or new approval mechanism is needed.

Existing AOS-30 VER-005–007 already describe the relevant planned checks. They can serve as functional walkthrough scenarios across the receiving components; no implementation test is required to close this documentary point.

### CR30-03 — explicitly include human decision preparation in correction notifications

**Classification: limited functional-link clarification.** AOS-02 CON-003 lists correction consumers 01/03/04/05/13/21–25 but omits AOS-30. General material-dependency behaviour and AOS-30 REQ-035/§11 already require reassessment, so this is not absence of a system-wide correction rule. However, a corrected source can affect an AOS-30 preparation pack or pending decision account as well as GI analysis and agent execution.

**Recommendation:** name AOS-30 as a conditional correction recipient where its pending preparation, account or outcome review materially depends on the corrected evidence. AOS-30 should flag that dependency and obtain appropriate human review; GI remains responsible for revising its canonical analysis. A source correction cannot silently rewrite approved minutes, make a new governing decision or reverse a completed effect. This follows existing DEC-069/089 and AOS-30 REQ-034–036; no new power or general design choice is proposed.

## 5. Functional walkthroughs

| Scenario considered against the written specifications | Coherent expected behaviour |
| --- | --- |
| Chair approves a draft; a component requests authority to act on it | AOS-30 preserves draft status; AOS-01 and receiving components require the applicable board approval evidence and current controls. CR30-02 makes that shared interpretation explicit. |
| Human rejects a GI recommendation | Record the empowered decision and rationale; retain analytical history; separately check permitted implementation; do not turn the override into precedent automatically. |
| A source changes after a board pack is prepared | GI reassesses affected analysis; AOS-30 flags affected preparation/account work and obtains human review; approved historical records remain governed by correction procedures. CR30-03 clarifies notification. |
| Protected finding implicates the normal recipient during a platform outage | Use only authorised alternative reporting/continuity, retain tracking ownership until accepted transfer, and preserve failed delivery and outstanding duties. |
| Resident disputes repair closure | Use agreed channels and accessible review, preserve original dispute/commitment, distinguish contractor status from verified outcome, and retain accountable follow-up. |
| Workflow research proposes an urgent amendment | Record evidence and permitted urgent operational response separately; human disposition and controlled change remain necessary. |

These are document walkthroughs, not executed tests or proof of effective human governance.

## 6. Completion and next step

Requested review and authorised functional alignment complete. No fundamental redesign or new general design question required. CR30-01–03 closed by amendments in §7. Next remaining GI specifications under item 7. Original review did not amend specifications; subsequent amendments were separately authorised by Mark.

Exact wire schemas, code lists, compatibility tests, organisation appointments, numerical settings and operational evidence remain later implementation/commissioning work. Their absence does not prevent completion of this functional consistency review or continued component drafting. Existing organisation-specific authority, privacy and independent-review prerequisites remain applicable before operation.

## 7. Authorised amendment disposition — 7 October 2026

Mark instructed three amendments and closure of AOS-30 work. AOS-00/Map v0.25, DEC-001–089; AOS-01–05 v0.8, AOS-14 v0.4, AOS-20 v0.3 and AOS-30 v0.3; Shared v0.9/Core v0.6/Exchange Register v0.8; source matrix v0.9 and template v0.4 unchanged; Control Coordination v0.2/Protected Reporting and Recovery v0.1 unchanged.

| Finding | Disposition / evidence |
| --- | --- |
| CR30-01 | Closed: current drafting/adoption/next-step references corrected in GI, kernel/Boundary, architecture/map and AOS-30; current adoption in Register §15. Dated history retained. |
| CR30-02 | Closed: kernel §§6.7, GI §6.5, Core REC-R09 and common contracts/register explicitly preserve separate roles and Chair draft versus board minutes/decision approval. Non-board routes and independent authority/use controls preserved. |
| CR30-03 | Closed: 02 CON-003/REQ-019/§10.2/VER-008 and 30 §6.2.1/REQ-035/VER-021 explicitly include correction receipt; GI §6.5 owns analysis revision and informs workflow. Existing KX-13 scope retained. |

AOS-30 functional specification work complete. Author validation checks changed references, unchanged register identities/counts and table structure. No operational case executed; independent review deferred. No new design question, schema or authority introduced.

