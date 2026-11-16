# AOS Change Constitution

Document: aos-change-constitution-v0-1 · Source revision or record: v0.1, 9 October 2026, draft for review

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

## How we improve the architecture together

**Version 0.1 · 9 October 2026 · Draft for review**

AOS should be capable of learning from experience without losing the principles that give it purpose. People who use, build, supply or are affected by it should be able to question it and help improve it. Changes should be understandable, supported by evidence and decided by people with a clear responsibility for the whole.

This Constitution proposes how that happens. It governs changes to the shared AOS foundations, architecture, specifications, contracts and assessment arrangements. It also describes how stewardship can pass from the founder to others.

It does not govern an individual organisation's decisions, change its purpose or grant powers to its staff, suppliers or AI. Each organisation retains its own authority and approval arrangements. A new AOS release is not permission to change a live system.

**This document is a proposal.** Mark Sweeny remains the current project custodian and human decision authority. Drafting this Constitution does not adopt its proposed rules, appoint future reviewers or approve publication. Existing architecture decisions and specification-quality gates continue to govern the working suite until an explicit adoption decision is recorded.

## 1. The commitments behind change

We propose six commitments:

- **Welcome contribution.** Useful insight can come from residents, employees, boards, researchers, suppliers, implementers and other interested people. The right to raise a concern should not depend on purchasing a product or holding an official position.
- **Keep human responsibility clear.** AI can observe, research, analyse, challenge and draft. People decide whether the shared specification changes and take responsibility for that decision.
- **Make reasons visible.** Show the problem, evidence, alternatives, uncertainty and reasons for the outcome. Explain necessary limits on disclosure.
- **Consider the whole.** A local improvement can create difficulties elsewhere. Examine affected components, users, information exchanges and existing implementations together.
- **Preserve meaningful disagreement.** A decision need not be unanimous, but an unresolved objection must remain visible and receive a reasoned response.
- **Make stewardship transferable.** Authority belongs to an identified role with recorded duties and limits. It should be possible to hand over that role and its records without depending on the founder's memory or continuing availability.

## 2. Who can contribute

Anyone may propose a correction, improvement or new capability, or challenge an existing assumption. People may submit a concern without drafting replacement specification text. Assistance should be available to help turn that concern into a reviewable proposal.

Suppliers may contribute implementation experience and suggest practical alternatives. Residents and employees may describe effects that technical reviewers have missed. Researchers may offer evidence that challenges an established position. None of these contributions carries an automatic entitlement to approval.

An AI research agent may submit a finding or proposed change within its approved remit. The record must identify the agent, its sources and limitations. An agent cannot approve its own proposal, amend the authoritative specification directly or expand its permissions through the change process.

Contributors should declare relevant interests, including commercial interests. Participation does not confer exclusive ownership of an AOS function, preference in procurement or a conformity endorsement. Licensing and reuse terms will be settled through the separate publication arrangements.

## 3. The responsibilities we need

These are proposed responsibilities, not an announcement that all the roles are already filled.

| Responsibility | What it involves |
| --- | --- |
| Project custodian | Maintains the process, identifies who has authority, arranges consultation and keeps unresolved matters visible |
| Proposer | Describes the concern or opportunity and helps clarify the proposed response |
| Evidence steward | Checks sources, dates, provenance, uncertainty and whether the evidence supports the claims being made |
| Component and shared-contract stewards | Examine effects on their areas and on the meanings and responsibilities shared with other components |
| Reviewers | Challenge assumptions, consider affected people and implementations, and record agreement and disagreement |
| Decision authority | Makes and explains the authorised human decision, including conditions and unresolved objections |
| Release custodian | Ensures the approved wording, document versions, decision record and release notes agree |
| Implementation and assessment owners | Decide what an approved specification change means for particular implementations and existing evidence |

One person may initially carry several responsibilities, but the record must show that overlap. A second AI analysis is useful challenge; it is not independent human review.

During the present sole-human stage, Mark holds the project-custodian and decision-authority responsibilities. Drafting and author checks can continue with AI assistance. Independent project review remains deferred and must be described as such. No fictitious committee, independent reviewer or second approval is to be recorded.

As participation grows, appointments should record the person's remit, acceptance, relevant interests, authority, duration and cover. A proposed future review group should include architectural knowledge and perspectives from implementation and affected users. A supplier's commercial interest must be visible and managed; supplying technology alone does not give the supplier authority over the shared architecture.

## 4. Different changes need different attention

| Type of change | Proposed approach |
| --- | --- |
| Editorial correction | A spelling, layout or broken-link correction that leaves meaning unchanged may use a short record and custodian check |
| Clarification | Wording intended to preserve meaning needs confirmation from affected stewards; if reasonable readers could act differently, treat it as substantive |
| Substantive change | A change to responsibilities, required behaviour, information meaning, controls or assessment needs evidence, cross-component review, impact assessment and an explicit decision |
| Foundational change | A change to the principles, human decision rights, core constraints, source hierarchy or this Constitution needs a separate, prominently identified proposal and strengthened scrutiny |
| Emergency response | A serious newly identified concern may need immediate protective action and an accelerated review, followed by a full recorded decision |

Splitting a proposal into small edits must not hide its combined effect. Where classification is disputed, use the more thorough route until the dispute is resolved.

## 5. From a concern to a decision

### Make the proposal understandable

Give the proposal a stable identifier and record who raised it, when, which version it concerns and what problem it seeks to address. Explain the intended outcome in ordinary language before presenting detailed wording.

The proposal should identify affected documents and requirements where known. It should distinguish a correction to the architecture from a new use case, implementation choice or organisation-specific policy. Later applications belong in their own scope rather than quietly enlarging the core architecture.

### Assemble the evidence

Keep links or retained references to the sources, with their dates, versions and relevant limitations. Separate observed facts, interpretations and assumptions. Explain why the evidence is relevant to AOS and what it cannot establish.

Evidence may include incidents, research, user experience, supplier experience, test results and contradictions within the suite. The strength of evidence needed should reflect the consequences of the change. A plausible suggestion is enough to begin discussion; it is not automatically enough to justify adoption.

### Invite challenge

Identify the people and component stewards affected. Provide the proposal, relevant evidence and questions in an accessible form, with a response period appropriate to its consequences and urgency. Record the period, who was invited and any participation limitations.

Seek perspectives beyond the proposer, particularly where residents, employees or smaller suppliers could experience unequal effects. Consultation is an opportunity to influence the outcome. Silence is not agreement.

Record objections, alternative interpretations and suggested alternatives. Assess whether the proposal moves a responsibility into a part of the system that cannot properly fulfil it.

### Assess the consequences

Before deciding, consider:

- The foundations and existing architectural decisions.
- Affected responsibilities, requirements, contracts, terminology and planned tests.
- Privacy, permissions, human judgement, access and inclusion.
- Financial exposure and resource impacts separately, including staff workload and displaced duties.
- Compatibility with existing implementations and the meaning of existing conformity claims.
- Migration, recovery, reversal and risks of leaving the architecture unchanged.

An impact assessment should name remaining uncertainties and who will resolve them. It must not invent missing operational thresholds, authority or evidence.

### Make and explain the decision

The authorised human decision may be to accept, accept with conditions, request further work, defer or reject. Record the exact scope, reasons, evidence considered, dissent, conditions, responsible owners and intended effective date.

A conditional decision must say which conditions prevent release or reliance, and how fulfilment will be checked. It must not be presented as unconditional approval. Disagreement does not automatically prevent a decision, but the decision must address material objections rather than merely note that they exist.

### Release, then learn

Update the affected documents together, check their consistency and issue a clear account of the change. Preserve the previous version and link it to the proposal and decision.

After implementation, review whether the expected benefits and safeguards have been achieved. New evidence may justify reopening the decision. Closing a proposal does not close the right to challenge it.

## 6. Protecting the foundations

A foundational amendment must state clearly which principle or protected arrangement it would change and why. It must explain alternatives, consequences for affected people and existing systems, and how the amendment remains coherent with the rest of AOS.

The proposed adoption rule is an explicit human decision supported by cross-component review and independent human scrutiny appropriate to the subject. A concern raised about a protected principle cannot be settled by silently rewriting its wording in a component document.

Independent scrutiny has not yet been arranged. Foundational proposals can be researched and drafted now, but adoption under this proposed route remains pending that scrutiny and a recorded decision. This does not retrospectively invalidate existing approved directions or block ordinary drafting under the present project arrangements.

An amendment that removes a defining commitment must be identified openly as a change of foundation. Publication must explain the resulting scope and identity, rather than claiming effortless continuity with earlier releases.

## 7. Interests, dissent and requests for reconsideration

Relevant personal, professional and commercial interests should be declared when a proposal is submitted and reviewed. The custodian should record how each material conflict is handled.

In a future arrangement with several authorised people, a conflicted decision-maker should step aside and an appointed alternate should decide. During the sole-human stage, where Mark cannot reasonably make an impartial decision, the proposed disposition is to seek an appropriate external reviewer or leave the substantive decision pending. An AI does not become the replacement decision authority.

A contributor may request reconsideration by identifying new evidence, an overlooked effect, a material process failure or an unanswered objection. A new reviewer should be used where one is available and authorised. If none is available, record the limitation and arrange review; do not label repeated consideration by the same person as an independent appeal.

Records should represent dissent fairly, including the reason the decision authority did not follow it. Personal or protected information may need restricted handling, but a public summary should explain the substance where it can safely do so.

## 8. Emergency action and reversal

Urgency may justify a faster process. It does not create new authority, suspend human judgement or permit an AI to approve a normative change.

The authorised project custodian may, within existing project rights, mark an affected draft or release as under review, withdraw a recommendation or pause project publication pending assessment. Record the concern, affected versions, protective action, authority, owner and review date.

A change to normative wording still requires an explicit human decision. An emergency record must state its limited scope, expiry or review point, notifications and follow-up scrutiny. Temporary measures must not become permanent by being forgotten; continued measures require a recorded decision.

An operational organisation may need to suspend activity under its own authorised procedures. This Constitution does not issue that instruction or grant the project custodian power over a live installation.

Reversal follows a recorded decision and impact assessment. Restoring older wording may help, but cannot undo disclosures, payments or other effects that have already occurred. Preserve the history, identify outstanding consequences and assign responsibility for addressing them. Reversal must not restore permissions or reinstate withdrawn authority automatically.

## 9. Versions, publication and implementation

Each released document should show its identifier, version, date, status and relationship to the approved release collection. Keep requirement identifiers stable where their meaning continues; explicitly retire or supersede them when necessary. Never reuse an identifier to conceal a different obligation.

Release notes should explain material changes, affected interfaces and assessment cases, compatibility limits and actions expected of implementers. Identify the exact versions that belong together. Drafts, approved architectural directions, released specifications and demonstrated implementation behaviour must remain distinguishable.

A proposed change remains outside the authoritative baseline until the required decision and release checks are complete. Earlier decision records and source histories are retained; approval dates must not be backdated.

Each implementing organisation decides whether and how to adopt a release under its own arrangements. Implementation owners assess migration and verify the affected behaviour. Existing conformity claims must be reviewed for their actual scope and version; a new release does not automatically invalidate every earlier claim or validate an upgraded implementation.

Public records should include proposals, dispositions, release notes and meaningful reasons. Where information must be restricted, record why, who can review it and what can be disclosed. Publication arrangements must provide an accessible contribution route and explain how feedback is handled.

## 10. Passing stewardship to others

The founder's present role should be capable of transfer. A handover should include:

- The appointed successor's remit, acceptance and decision limits.
- The current baseline, source hierarchy and outstanding proposals and objections.
- Decisions, review records, release history and unresolved assurance limitations.
- Access and custody arrangements, with credentials transferred securely.
- Funding, relevant interests, supplier relationships and publication commitments.
- Effective date, cover and the authority retained or relinquished by the outgoing custodian.

Holding an account password or hosting the files does not itself confer constitutional authority. Technical custody and decision authority should be recorded separately.

Mark should appoint a successor or interim custodian through a recorded handover while he is able to do so. A later multi-person stewardship arrangement should have its own approved membership, appointment, voting, quorum, conflict and continuity rules before it exercises authority. Those rules are not invented by this draft.

If the decision authority becomes unavailable without an authorised successor, preserve the records and use existing permissions for protective maintenance. Substantive approvals remain pending until legitimate authority is established. An agent must not fill the vacancy by inference.

## 11. A practical change record

| Field | What to record |
| --- | --- |
| Proposal | Identifier, proposer, date, affected baseline and declared interests |
| Purpose | The problem, intended outcome and suggested wording or response |
| Evidence | Sources, provenance, dates, uncertainty and limits |
| Review | Classification, affected stewards, consultation, challenges, alternatives and dissent |
| Impact | Principles, components, exchanges, users, financial and resource effects, compatibility and migration |
| Decision | Authorised person, disposition, reasons, conditions, owners and date |
| Release | Approved text, document versions, effective date, release checks and public summary |
| Follow-up | Implementation and verification responsibilities, review point, outcomes and reversal arrangements |

For an editorial correction, this can be brief. For a foundational amendment, it should provide a full account that another person can inspect and understand.

## 12. Status and next decisions

This draft completes the author drafting portion of to-do item 13a. Its proposed arrangements require Mark's review and an explicit adoption decision before they become project rules. The main choices for review are the change categories; current and future decision roles; independent scrutiny of foundational amendments; conflict and reconsideration arrangements; and emergency action and succession.

The Living Specification (RI-001) is deferred to Phase 2 (deferred under DEC-098) on Mark's instruction of 9 October 2026. Its design, implementation and testing are outside the current documentation and publication work. This Constitution can be used through ordinary documents and records; it does not depend on building RI-001. CAP-01 and CAP-02 also remain deferred. The overdue-repair example remains the selected first demonstration.

This draft builds on the earlier Change Constitution outline, the recorded FAR-001 reconciliation, the [system architecture](../Foundation/aos-00.md), and the specification-quality and change gates referenced by that architecture. It preserves the distinction between governing the shared specification and governing an organisation using it.

**Project custodian:** Mark Sweeny. **Draft prepared by:** Codex at Mark's request. No independent review, constitutional adoption, implementation or publication is claimed by this draft.

