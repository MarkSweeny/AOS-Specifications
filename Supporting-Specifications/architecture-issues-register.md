# Architecture issues register — FAR-001 intake

Document: architecture-issues-register · Source revision or record: 29 September intake with 9 October 2026 disposition

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**Current OQ-009/010/014 disposition — 9 October 2026:** Mark directed RI-001 Living Specification into Phase 2 under AOS-00-DEC-098. Its design, scope, implementation and acceptance work are deferred and are not prerequisites for current documentation or publication. The parked concept (deferred under DEC-098) retains the original proposal. The [Change Constitution v0.1](aos-change-constitution-v0-1.md) now offers proposed answers for evidence, challenge, decision rights, protected amendments, emergencies, reversal and succession; OQ-009/010 remain open for Mark's review/adoption and appropriate independent scrutiny. Drafting is not constitutional approval. Original issue rows and earlier dispositions below remain history; no unrelated question or source status is closed by this update.

**Status:** open questions, 29 September 2026. These are not new approvals. Owners are functional placeholders until allocated through AOS-00/AOS-QS. Source FAR-001 §19 unless otherwise noted.

| ID | Question or required reconciliation | Affected specifications | Next evidence or decision |
| --- | --- | --- | --- |
| OQ-001 | Represent ethics for artificial reasoning without reducing it to a simplistic rule list? | 00/01/04/20 | Map RP v6 and test novel cases. |
| OQ-002 | Distinguish constitutional hard boundaries from overridable operational ones? | 01/03/05/30 | Classify examples, authority and failure states. |
| OQ-003 | What independence between actor and constraint is sufficient? | 01/04/05/40 | Threat model D08 and attempted-bypass test. |
| OQ-004 | How are telos/ethics and competing ethical principles escalated and resolved? | 01/20/30 | Human authority and dissent process. |
| OQ-005 | Which decisions always require human authority? | 01/04/30 | Reconcile Mode 1/2 with DEC-024/025 and organisation schedule. |
| OQ-006 | What is a material action for Radical Transparency? | 02/04/30/40 | Threshold, access and proportionality cases. |
| OQ-007 | How are cumulative, population-level and emergent behaviours sensed? | 02/04/05/14/25/40 | Scenarios and false-positive limits. |
| OQ-008 | How are cross-component dependencies discovered and kept current? | 00/02/40 | Contract registry and change-impact cases. |
| OQ-009 | What evidence triggers reconsideration, and how much challenge before approval? | Change Constitution | Trial a proposal with divergent evidence. |
| OQ-010 | Which constitutional elements are exceptionally difficult to amend? | Change Constitution/00 | Separate AOS constitution from organisation telos authority. |
| OQ-011 | What is conformance, who may assert it, and how is partial conformance disclosed? | 02/40 | Scope/profile and evidence model. |
| OQ-012 | What may be federated across organisations, including incident duties? | 14/01/02/03 | Materiality, legal duties and external authority. |
| OQ-013 | Resolve Boundary Intelligence naming: external exchange versus shared authority enforcement. | 00/01/03/04/05/14 | Preserve DEC-005 allocation; choose unambiguous vocabulary. |
| OQ-014 | How does the proposed RI-001 fit after the selected overdue-repair first example? | 04/40/publication plan | Define sequence and bounded scope; do not reopen DEC-021. |

Each question should acquire an owner, source links, current evidence, confidence, decision gate, disposition and affected requirement IDs when triaged. Custodian research may monitor these questions as well as existing requirements; monitoring itself confers no change authority.

## Research agent pilot and intake

`AOS-14-Boundary-Research-Agent.md` defines the first component custodian. It watches OQ-002/003/006–014 where relevant, but its owned component is AOS-14 external exchange. Route systemwide authority findings to AOS-01/03/05 and AOS-04, with OQ-013 tracking terminology. A new material research update should state the baseline version and sources, classify facts versus inference, identify the affected element, use **No change / Monitor / Clarify / Change candidate / Urgent review**, and link any proposed change candidate to the later governed decision. No candidate is an adopted requirement simply by appearing here.

## Reconciliation dispositions — 3 October 2026

See `../90 Architecture Records/FAR-001-Reconciliation-v0.1.md` for all 14 issue dispositions and source/requirement links. Original intake rows above remain for provenance.

- **OQ-013:** resolved for working naming/allocation. AOS-14 is Boundary Intelligence and external exchange; systemwide enforcement is “shared authority and data-use enforcement” in AOS-01/03/05 with AOS-04. DEC-005 remains controlling. D08 mechanisms and threat-model sufficiency remain open.
- **OQ-014:** first-example sequencing resolved: overdue repair remains first. Later RI-001 scope and acceptance remain deferred.
- **OQ-012:** any federated model is deferred; existing external-exchange controls and verified duties remain in scope.
- **FAR-R-002:** Mark confirmed constraint explanations as a required default, with reviewed, recorded security/privacy/feasibility exceptions. Schema, permitted disclosure and exception authority remain component drafting obligations in AOS-01/03/04/05, applied in AOS-14; new REQ/VER records are not yet approved.
- Other issues remain open or partly constrained as classified in reconciliation §5. Mechanism gaps must not acquire default answers. Material decisions return to Mark.

Project-owner/custodian for this drafting stage: Mark Sweeny. Independent project review deferred; author/project review does not replace required independent organisational oversight or G3 evidence.

## Research intake — 4 October 2026

**External-agent trust evidence: provisional Clarify; author/project review only.** Mark supplied a substantive research update. Reviewed against the live AOS-14 charter of 29 September and this register's 3 October dispositions. Allocation is consistent with DEC-005: AOS-14 governs exchange obligations; AOS-01/03/05 and AOS-04 determine/enforce authority, data-use, delegation and revocation; AOS-02 retains provenance and exchange evidence. No normative change, new REQ/VER or federated identity architecture is approved by this intake.

**Primary sources verified, retrieved 4 October:** [NIST consultation summary](https://pages.nist.gov/nccoe-ai-identity/summary-of-comments.html), announced 29 September, and [OpenA2A AAP draft-02](https://www.ietf.org/ietf-ftp/internet-drafts/draft-fane-opena2a-aap-02.html), dated 30 September. NIST reports over 600 responses, rather than necessarily distinct respondents; the DevSecOps demonstration is planned, not completed. OpenA2A is an individual Internet-Draft/work in progress, not an adopted standard or implementation assurance. The separate 27 September per-action draft was not identified with a title/link and remains unverified.

**OQ-012 / item 6 input:** test exchange contracts for principal binding, mandate, provenance, delegation lineage, policy context, current revocation evidence and common claim semantics. Define responses to missing, stale, unverifiable or misunderstood claims; consider proportional disclosure/privacy. These are drafting questions, not approved defaults. The federated-model deferral stands. Precise requirement-level gap analysis remains provisional pending full clause mapping.

**Item 5b limitations:** a material output reached Mark, but its exact run and delivery reliability remain unverified. The scheduled agent reported a sign-in barrier to the live charter, although this project review could access it. Resolve scheduled baseline access; require source links, review period and retrieval records; calibrate duplicates/false positives; establish urgent escalation and accepted-finding intake. Mark remains project owner/custodian; the operational escalation route is not yet verified. No urgent escalation occurred. Independent review remains deferred.


