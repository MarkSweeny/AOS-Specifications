# AOS — GIL v2 comparison and reconciliation

Document: aos-gil-v2-comparison-and-reconciliation-v0-1 · Source revision or record: v0.3

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

Version: 0.3  
Date: 7 October 2026  
Status: completed source comparison; Q01/Q02 approved by Mark on 7 October 2026 and recorded as DEC-090/091 in AOS-00/Map v0.26. AOS-20–25/30 functional drafting, 38-disposition allocation and author consistency closure are complete. Operational setup, exact compatibility and assurance remain separate later gates.

## 1. Conclusion and scope

GIL v2 contains a useful foundation for AOS-21 organisation knowledge and corpus stewardship and AOS-23 artefact assessment and monitoring. Its organisation context, sourced assessment criteria, document relationships, evidence-linked findings and explicit blind spots should be reused. It is not a complete specification for the present GI function: synthesis, presentation, oversight, human authority and common kernel controls now have distinct owners.

The material inconsistencies are resolvable using decisions already agreed. GI is the interpretive element of the 1+5 architecture, not a sixth peer sensing domain or an autonomous adjudicator. Its local database, agent and review assumptions must yield to common authority, evidence, data-use, execution, reporting and recovery mechanisms. Protected boardroom deliberation must remain excluded without excluding permitted preparation material and approved human post-meeting records. An assessment of documents must not be presented as proof that governance works in practice.

This is a functional architecture comparison. Database design, endpoints, vendor choices, deployment, numerical settings and executable schemas are later implementation work. The report identifies their disposition without developing replacements. The original GIL document is preserved as historical source material, rather than silently rewritten.

## 2. Sources and authority

| Source | Baseline used | Role in this comparison |
|---|---|---|
| GIL Technical Specification V2 | v2.0, May 2026; `V0.1/GIL_Technical_Specification_V2.docx` | Legacy material being reconciled; all nine sections reviewed |
| Foundational Principles | v4; controlled source documents | Foundational constraints |
| AOS Reasoning Principles | v6; controlled source documents | Current reasoning, Mode 1/Mode 2, delegation and sensing constraints; supersedes GIL's RP v4 checklist |
| Governance Intelligence Tests | controlled source document | Observable technical contribution versus human governance judgement; no self-certification |
| AOS-00 and Specification Map | v0.25; DEC-001–089 | Current architecture, allocations and agreed decisions |
| AOS-01–05 | v0.8 | Common authority, shared records, data use, agents and platform controls |
| AOS-14 / AOS-20 / AOS-30 | v0.4 / v0.3 / v0.3 | Boundary exchange, GI charter and accountable human workflows |
| Shared / Core / Exchange Register | v0.9 / v0.6 / v0.8 | Common semantic obligations and component exchanges |
| Control Coordination / Protected Reporting and Recovery | v0.2 / v0.1 | Material change, execution limits, protected findings and recovery |
| Component template | v0.4 | Functional specification structure, including own external-research remit |
| GI Material Review and Design Questions | content v0.2, 6 October | Seven approved directions, recorded as DEC-079–085 |

Current architecture and controlled principles govern the reconciliation. GIL's claim to be a self-contained coding brief does not override later decisions. Its references to legal or regulatory standards are source claims requiring currency, jurisdiction and applicability checks when admitted into the corpus; this comparison does not verify those standards or certify compliance.

## 3. Component allocation

| Destination | Material to develop |
|---|---|
| AOS-21 | Scoped organisation profiles; constitutional, operational and external corpus; artefact catalogue and relationships; source provenance, currency and supersession; human stewardship; approved precedent and its correction/withdrawal |
| AOS-23 | Ingestion and classification; applicability; document questions and assessment criteria; evidence-linked findings and uncertainty; review states; artefact/source change monitoring and reporting-cycle assessment |
| AOS-22 | Cross-domain synthesis, conflicting evidence, interpretations and options, including infeasible alternatives and their constraints |
| AOS-24 | Faithful presentation of canonical analysis, supporting evidence, limitations, disagreements and approved status |
| AOS-25 | Drift, overrides, blind spots, emergent effects and independent oversight; ordinary evaluation without reopening deferred self-calibration |
| AOS-30 | Human review, accepted duties, decisions, action/outcome feedback and post-meeting approval |
| AOS-01–05 / AOS-14 | Common governing controls, records and permitted external retrieval/exchange; components reference these rather than create competing mechanisms |

The allocation is a drafting map, not a claim that the remaining components are already specified.

## 4. Traceable disposition of GIL material

Retain means preserve the business concept in the allocated specification. Revise means preserve its purpose while changing the governing assumption. Retire means remove the stated rule from the current functional baseline. Defer means preserve an implementation candidate without making it a functional requirement. GIL has no comprehensive numbered requirement register; section and table/concept references below provide the source trace.

| ID | GIL source and concept | Disposition and current direction | Destination / governing reference |
|---|---|---|---|
| GIL-C01 | §1, internal organisation-owned GI | Retain organisational ownership and accountability. Do not restore commercial customer/subscription assumptions. Ownership alone does not resolve supplier or corpus licensing. | 20/21; FP v4 |
| GIL-C02 | §1, sixth domain and conscience that adjudicates | Revise to 1+5: GI prepares and interprets; empowered humans adjudicate. GI does not own kernel authority or govern every other component by itself. | 20/22/30; DEC-005 |
| GIL-C03 | §1.1, four operational layers | Retain as useful decomposition of organisation knowledge, assessment and monitoring; extend with current corpus/precedent, synthesis, presentation and oversight responsibilities. | 21–25; Map |
| GIL-C04 | §§1.1/2.2/8, 121 artefact types | Retain an extensible sourced catalogue. The specification does not supply the full 121-item inventory or its knowledge content; do not claim that seed content has been reviewed or that this number defines complete coverage. | 21/23/25 |
| GIL-C05 | §1.2, not a board portal or compliance certificate | Retain. Analysis may ingest permitted documents and deliver through approved channels; it need not replace the portal. Findings are evidence-qualified analytical conclusions, not automatic legal or governance certification. | 23/24/30; GT |
| GIL-C06 | §§1.2/2.6/6.2/7.2, boardroom exclusion | Revise blanket exclusion of agendas, minutes and action logs. Exclude protected live/deliberative capture; admit purpose-permitted preparation artefacts and human post-meeting accounts with their actual approval state. A false default flag is not evidence of permitted content. | 03/23/30; DEC-008/087–089 |
| GIL-C07 | §§1.2/3.3, no external contact or API calls; external monitoring elsewhere | Resolve the internal conflict: authorised source retrieval uses Boundary exchange. Outward representations or commitments require applicable human authority. No local agent bypass or blanket API prohibition. | 01/03/04/14; DEC-086 |
| GIL-C08 | §§1.3/6.2/6.3, UDL events and review before recording | Retain canonical recording; revise blanket human review before any UDL write. Provisional material is recorded/accessed with status and restrictions; formal validated reliance requires review. Urgent protected escalation need not wait for ordinary validation. | 02/20/30; DEC-084 |
| GIL-C09 | §1.3, every Mode 1 process traced to an assessed artefact | Revise: valid governing instruments, powers and applied controls establish authority. Artefact assessment supplies evidence and can expose gaps; it neither creates authority nor replaces current-checkpoint control. | 01/04/20/23 |
| GIL-C10 | §§1.4/6.3, continuing monitoring and periodic review/reporting | Retain both ongoing awareness and human review cycles. Monitoring does not eliminate contextual human reassessment. Cadence and reporting scope belong to governed profiles, not universal quarterly defaults. | 21/23/25/30 |
| GIL-C11 | §§1.5/2/5, technology, UUID tables, REST endpoints, named model and hosting | Defer physical design, vendor/model and integration choices. Preserve privacy, residency and security needs as governed requirements/profiles; do not adopt legacy technical settings automatically. | 03/05; implementation |
| GIL-C12 | §2.1, singleton organisation and annual-report-derived profile | Retain contextual profiles; revise to sourced, versioned and scoped knowledge with human confirmation. Annual reports are one source, not sole truth until next year. Subsidiary scope is approved under Q01/DEC-090 below. | 21; evidence contract |
| GIL-C13 | §2.1, false/empty defaults for contextual attributes | Retire assumptions that unknown means false or absent. Distinguish unknown, unverified, disputed, restricted and refuted; retain source, assurance and applicability. | 02/21/23; DEC-045–048/062–066 |
| GIL-C14 | §2.2, frameworks, questions, quality criteria and relationships | Retain sourced, effective-dated, jurisdiction/applicability-aware knowledge. Separate legal references, analytical standards and governing powers; a liability flag cannot establish a legal conclusion. | 21/23; 01/02 |
| GIL-C15 | §§2.2/5/6.5, administrator/Company Secretary writes and ARC/board amendment rules | Revise access versus authority. Human Knowledge Steward may perform delegated routine admission/versioning and faithful capture of approved meaning. Disputed authority, new interpretation and normative adoption use empowered review/change routes; no universal admin-write or ARC-minor/board-material shortcut. | 01/20/21/30; DEC-025/079–081 |
| GIL-C16 | §§2.3/6.2, evidenced/asserted/absent/not provided/not applicable | Retain useful descriptive assessment states with explicit uncertainty and evidence. A claim supported in a document differs from a verified fact; silence in a document does not prove absence in practice. Corroboration scope is approved under Q02/DEC-091. | 02/23; assurance contract |
| GIL-C17 | §§1.1/2.3/6.2/7.4, mandatory confidence scores and weak-match thresholds | Revise to calibrated, explained uncertainty and limitations; scores only where an approved method supports them. Retire universal confidence defaults and numerical caution triggers as functional rules. Confidence cannot substitute for source/fact assurance or human approval. | 20/23; DEC-084; profiles later |
| GIL-C18 | §2.3, findings, actions, interview packs, overrides | Retain citations, rationale, review and history. Recommendations require accepted accountable ownership before becoming duties; role labels alone are insufficient. Interviews/surveys require permitted purpose and review. | 22/23/24/30; Q02 |
| GIL-C19 | §§2.3/7.4, blind spots including non-applicable/unseeded artefacts | Retain explicit coverage limits and human ownership. Distinguish justified non-applicability, missing evidence, unseeded analysis, unassessed scope and intentional exclusion; they are not interchangeable risks. Committee acknowledgement is not proof that a blind spot is safe. | 21/23/25/30 |
| GIL-C20 | §§2.5/3, one agent per type and fixed schedules/deadlines | Retire mandatory deployment count and inherited numerical defaults. Use bounded common profiles, permissions, capacity, cover and escalation. An artefact type need not be a separately deployed agent. | 04/05/23; DEC-054–057/086 |
| GIL-C21 | §3, external changes and internal document currency | Retain change detection, source versions, effective dates and currency indicators. Record coverage and failure; distinguish no material change from incomplete, failed or unperformed checking. | 21/23; 02/04/14 |
| GIL-C22 | §§3/7.5, agents detect but never assess or judge | Revise: bounded agents may research, analyse, compare and propose; humans retain Mode 2 judgement and adoption. Separate corpus/artefact monitoring, research into component adequacy, and runtime/system oversight. | 20–25; DEC-082/086 |
| GIL-C23 | §§2.5/3.3/7.5, parameter register and hardcoded guarantees | Retain explicit permitted/prohibited actions and independent enforcement. Replace local control duplication with common authority/data-use/execution. An ethics statement, approval flag or permitted-action list alone does not demonstrate safety or impossibility of unauthorised action. | 01/03/04/05; common contracts |
| GIL-C24 | §§3/4, run logs, source checks, document versions and hashes | Retain provenance, exact revisions and auditable activity as common record views. Do not create a competing evidence silo or require unlimited raw content retention. Hashes identify bytes; they do not establish truth or permitted use. | 02/03/21/23 |
| GIL-C25 | §4, permanent/seven-year/two-year retention and soft-delete-only | Retire blanket retention/no-hard-delete rules. Apply record-class policy, purpose, legal holds and authorised deletion with suitable audit evidence; actual deletion cannot leave the same content indefinitely recoverable by default. | 02/03/05; DEC-045–048 |
| GIL-C26 | §5, functional API operations | Retain ingestion, retrieval, review, amendment proposal and reporting capabilities at semantic level. Defer endpoint/wire design. All operations use common governing controls; authenticated administrator access is not normative approval. | 01–05/21/23/30 |
| GIL-C27 | §6.1, annual-report calibration and profile review | Retain proposed profile/criteria application and human confirmation; distinguish routine faithful application from amendment of governing meaning. Retire autonomous normative calibration and annual-only freshness. Recording calibration completion does not establish outcome feedback. | 21/23/25/30; DEC-018/080/081 |
| GIL-C28 | §6.2, assessment sequence | Retain classification, applicable criteria, evidence analysis, findings/actions/questions and reviewed output. Add permitted-use checks, actual review states, uncertainty, source corrections and affected-consumer notification. | 23; 02/03/20/30 |
| GIL-C29 | §6.3, narrative reporting and approval | Split canonical assessment/synthesis, faithful presentation and human approval. An ARC Chair's report approval is not board minutes/decision approval. Publication, delivery, acceptance of duty and case completion remain distinct. | 22/23/24/30; DEC-087 |
| GIL-C30 | §6.4, safety/welfare handoff and executive review before routing | Revise executive gating of protected findings. Apply mandatory protected internal routes, accepted ownership, cover and implicated-recipient alternatives; no discretionary executive delay. Receipt is not resolution. Retire hardcoded deadlines; use applicable urgency profiles. | 05/20/30; DEC-073–078/083 |
| GIL-C31 | §6.5, amendments wait for next meeting or annual recalibration | Retire universal waiting rules. Material findings and changes require timely governed review, impact identification, notifications and owned reassessment. Preserve exact applied state; no silent bulk recalibration or automatic historical reversal. | 01/02/20/21/23/30; DEC-067–072/089 |
| GIL-C32 | §7, RP v4 compliance checklist | Retire as a current compliance claim. Re-map to all RP v6 domains, FP v4 and relevant GI Tests, stating contributions, limits and planned evidence. Selected schema fields and explanatory assertions do not prove a test passed. | 20–25/30; template |
| GIL-C33 | §7.1, absence questions instead of infeasible alternatives | Retain absence questions but reject their equivalence to surfacing infeasible options. Both missing evidence and useful options constrained by authority/resources require explicit treatment. | 22/23; RP v6 |
| GIL-C34 | §7, UDL events/ethics fields claimed to close feedback or demonstrate telos | Revise to evidence of actual consequences, human challenge and review. Capture outcomes, unintended effects and constraints. Only the empowered board changes telos; database statements do not enact or validate it. | 22/25/30; DEC-024; FP/GT |
| GIL-C35 | §§7.5/7.6, transparency and cross-domain access defaults | Retain reviewable explanations and purpose limits. Use independent permission/data-use controls, not audience-role defaults alone. No inferred individual emotional/preference profiles or secondary use merely because records are accessible. | 03/20/30; DEC-049–053/088 |
| GIL-C36 | §8, phased build and one risk-management fixture | Defer build sequencing. A fixture may illustrate assessment but cannot prove full GI/AOS coverage. Preserve the already agreed overdue-repair first demonstration; no build activation is authorised by this comparison. | 40; existing project direction |
| GIL-C37 | §9, portal, survey, UDL API and seed population questions | Defer channel/form/API choices. Seed completeness is an explicit coverage/content dependency, not a requirement to populate 121 documents before functional drafting. Current shared records settle the semantic UDL direction. | 21/23/24/30; implementation |
| GIL-C38 | §9, subsidiary scope and annual-report frequency | Apply approved subsidiary scope under Q01/DEC-090. Resolve frequency through governed monitoring and multiple current sources rather than reopening a sole-annual-report assumption. | 21/23; DEC-086 |

## 5. Coverage beyond GIL's checklist

| RP v6 domain | Required treatment in remaining GI specifications |
|---|---|
| 1 — Architecture and completeness | Account for evidence gaps and useful infeasible alternatives; no single-document fixture completeness claim |
| 2 — Mode 1/Mode 2 | Governed operational boundaries; human deliberation and approved post-meeting accounts; no automated normative judgement |
| 3 — 1+5 | Cross-domain evidence and synthesis; no sixth peer/adjudication framing |
| 4 — Options and Decisions | Ground options in actual organisational evidence; preserve reasons, rejected options, caveats and human-confirmed context; trace actual decision consequences |
| 5 — Blind spots and honesty | Scoped coverage, uncertainty, disputed evidence and missing/failed monitoring |
| 6 — Ethics and Telos | Preserve board-owned telos, affected residents' circumstances, equity and meaningful challenge/access, including those unable to exit; examine system-wide emergent effects; documentary completeness alone cannot establish ethical governance |
| 7 — Radical Transparency | Explain evidence, uncertainty, constraints and human responsibility in intelligible terms; enable scrutiny without exposing protected personal or deliberative material |
| 8 — Agentic delegation | Bounded permissions, shared cumulative limits, independent controls, meaningful explanations and accepted human handoff |
| 9 — Data and sensing | Declared purpose, independent data-use permission, protected deliberation and human-confirmed contextual descriptors |

The Governance Intelligence Tests require observable technical evidence and human assessment of governance in practice. The comparison identifies contribution and limits; it does not award passes or substitute AI evaluation for human Mode 2 review.

## 6. Scope choices approved by Mark

### Q01 — Group and subsidiary scope

Should AOS-21 support relevant subsidiaries/group entities as distinct scoped profiles linked to the parent?

**Recommendation: yes, within the approved organisational remit.** Preserve each entity's powers, governing corpus, applicability and evidence, and identify excluded entities with a responsible human owner. This establishes semantic scope without requiring separate deployments or cross-organisation federation. GIL §9 explicitly leaves this unresolved; the current architecture does not select the organisational perimeter.

Status: approved 7 October 2026; Mark: “Yes, both agreed”. Recorded as DEC-090. AOS-21 drafting must preserve the approved scoped-entity distinction.

### Q02 — Documentary claims and corroborating evidence

Should AOS-23 be allowed to corroborate documentary claims using separately permitted records, outcomes and human-supplied interview or survey evidence?

**Recommendation: yes, while reporting document quality, support for a claim and evidence of actual practice separately.** Each use must be purposeful, sourced and permitted. No live boardroom observation, inferred personal profiling or automatic certification follows. Broader judgement of governance effectiveness remains with human review and the oversight/workflow/test responsibilities of AOS-25/30/40.

Status: approved 7 October 2026; Mark: “Yes, both agreed”. Recorded as DEC-091. AOS-23 drafting must preserve the three distinct assessment dimensions and permitted-use boundaries.

The seven GI choices already approved as DEC-079–085 settle charter/profile separation, stewardship, precedent, proactive review/research, protected routing, graduated review and independent preparation. They need applying, not asking again.

## 7. Follow-through and completion

The source comparison is complete. Item 7 remains open because the component specifications and their requirement/case allocation are not yet drafted. Q01/Q02 are approved; next draft AOS-21 and AOS-23 using this disposition register. Develop AOS-22/24/25 around their allocated responsibilities. Each new specification must include its own external-research remit/profile and common AOS-04/AOS-02/AOS-01 references under DEC-086/template v0.4, without inventing a separate deployment or cadence.

Draft acceptance should confirm that each applicable GIL-C disposition is carried into a component requirement, constraint, source note or explicit retirement/deferment; that human review/monitoring transitions and affected-consumer correction paths agree with current contracts; and that no legacy confidence, timing, retention or approval default has slipped back in. Planned cases should include disputed/absent evidence, protected deliberation versus permitted records, provisional versus validated outputs, failed source coverage, implicated reviewers and correction of dependent analysis.

Checks performed: ordered GIL text and tables reviewed; dispositions mapped across all nine source sections; current decisions, component allocations and principle domains compared; open choices separated from settled directions. This is an author document comparison, with no executed implementation cases, independent assurance, new DEC, component amendment or build/readiness approval. AOS-30 remains complete at functional specification level. Research pilot item 5b remains open and unchanged.


**Approval update, v0.2 — 7 October 2026:** Mark approved both recommendations. AOS-00/Map updated to v0.26 with DEC-090/091. The §2 source manifest records the comparison baseline; this approval supplement records the later decision baseline. All 38 disposition IDs preserved. No additional comparison design question remains; AOS-21/23 drafting is next.

## Current drafting and consistency closure — 7 October 2026

Mark authorised GI-CR-01–04 corrections and closure. The GI consistency review v0.2 records the applied amendments and all 38 GIL disposition allocations. AOS-00/Map v0.32, DEC-001–091; AOS-20 v0.5/21 v0.6/22 v0.4/23 v0.5/24 v0.3/25 v0.2/30 v0.5; AOS-01–05 v0.8, AOS-14 v0.4; Shared v0.15/Core v0.6/Exchange Register v0.14/source matrix v0.15; template v0.4; Control Coordination v0.2/Protected Reporting and Recovery v0.1. Earlier consultation/drafting-next statements are historical; retained, revised, retired and deferred source dispositions remain unchanged. No legacy vendor/schema/default is reinstated; no operational acceptance claim is made. Next AOS-40.

