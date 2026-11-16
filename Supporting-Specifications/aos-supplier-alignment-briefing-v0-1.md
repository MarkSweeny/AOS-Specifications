# Where does your product fit in AOS?

Document: aos-supplier-alignment-briefing-v0-1 · Source revision or record: Discussion draft, editorial revision 29 October 2026

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

**Editorial edition — 29 October 2026:** Mark authorised documentary corrections D-01–09. This edition reconciles navigation, count/revision pointers, conformance links and historical scope labels; existing technical meanings, requirement/IF/decision identities and proposed/planned status are retained. The internal version below identifies the retained functional baseline; this dated editorial edition identifies the corrected document. See the [current document inventory](aos-current-document-inventory-2026-10-29.md) and [correction record](aos-documentary-corrections-2026-10-29.md). Earlier dated adoption baselines are historical snapshots; exact logical family/view revisions are in Exchange Register §4.

## An invitation to system suppliers

**Draft for discussion · Editorial revision 29 October 2026**

Editorial change: corrected the AOS expansion; no supplier capability, conformance or publication approval is implied.

Good systems grow from the knowledge of the people who build and use them. If you supply software, sensors or technology services to housing organisations, you already bring part of that knowledge: an understanding of the work, the information it needs and the practical difficulties of making it all happen.

We would like to explore how that experience, and the capabilities of your products, can contribute to the Adaptive Operating System (AOS).

AOS is a reference architecture for bringing organisational information, software, AI and human judgement together. Its initial setting is social housing in England. It describes how different capabilities can work together to help an organisation understand what is happening, respond effectively and account for its decisions.

The starting question is simple: **where could your product fit into this mosaic, and what could we achieve together?**

We want to build on products that organisations already use and value. A product might contribute to several parts of AOS; several products and human teams might contribute to the same part. Each brings something useful. The shared task is to make those contributions work well together.

This briefing is an invitation to that conversation. Your experience can help us understand the possibilities, make the connections practical and improve the architecture itself.

## The picture we are building together

AOS brings together five areas of organisational understanding:

- **Assets:** understanding homes, buildings and equipment—their condition, what needs attention and whether work has achieved its purpose.
- **Residents:** understanding service needs, choices and participation, communicating in agreed ways and respecting the limits on private information.
- **People:** understanding workforce skills, capacity and employment information, and supporting people-management work while keeping employment judgement with humans.
- **Processes:** understanding how work should happen, how it actually happens, who has accepted responsibility and whether the intended outcome has been achieved.
- **External exchanges:** understanding information and activity across organisational boundaries, including relationships with suppliers, contractors and external services.

Governance Intelligence draws on appropriate evidence from these areas to help people interpret events, ask better questions, exercise oversight and prepare decisions. Accountable humans retain decisions that require judgement between competing values, along with the powers reserved to them.

Shared arrangements connect the parts: reliable records, clear meanings, identity and permissions, security, controlled actions and recovery when something goes wrong.

Your product might provide information, carry out a function, connect systems or support these shared arrangements. Together, we can identify where its contribution is most useful and what it needs around it.

## Where you might recognise your contribution

These examples offer starting points for discussion. We would welcome your help in refining them.

| Your product or service | A possible contribution to AOS | A useful conversation to have together |
| --- | --- | --- |
| Housing management or repairs software | Tenancy and service records, repair promises, appointments, contacts and work events | How we connect these records to a shared understanding of responsibility, progress and the outcome for the resident |
| Asset management or building-information software | Asset identities, inspections, condition evidence, maintenance history and information supporting safety responsibilities | How we preserve the source, age and limits of evidence, and share changes with those who rely on it |
| HR or workforce software | Employment records, skills and training evidence, and workforce-service processes | How we support useful work within agreed purposes, protect sensitive information and preserve human employment judgement |
| Sensors or IoT services | Observations about physical conditions, device health and gaps in coverage | How we combine readings with other evidence, understand their reliability and respond when readings are missing |
| Finance or treasury software | Financial records, commitments, expenditure, forecasts and payment evidence | How we connect financial information to authorised commitments and organisational outcomes while keeping their meanings clear |
| Workflow or case-management software | Work definitions, assignments, deadlines, exceptions, escalation and follow-up | How we connect work to people who have accepted responsibility, and keep unfinished or disputed matters visible |
| Governance or document software | Papers, evidence, analysis, decision records and explanations | How we help people understand the evidence, its limitations, what has been approved and what happened afterwards |
| Integration, identity, AI or platform services | Connections between systems, shared records, identity checks, controlled processing and dependable operation | How we preserve meaning and permissions across connections, and maintain a reliable account of actions and their effects |

A contribution may involve your product, an adapter, another supplier's service and the organisation's own people. Understanding that combination gives us a better basis for collaboration and helps everyone see where their expertise is needed.

## Four questions to explore together

### What can we learn from your product?

Your knowledge of the information your product holds or produces is central to understanding its place in AOS. We would like to explore where that information comes from, what it means and what it can reasonably tell us.

A sensor reading, an inspection finding, a contractor's report and a verified service outcome each add something different. Keeping those differences clear helps people make sound decisions. The same is true of information that is uncertain, disputed, missing or out of date.

Where systems hold overlapping information, we can agree which source to rely on for each purpose and how to share corrections.

### What can your product help people do?

We would like to understand the work your product supports and the actions it can take. Reading a record, sending a message, making a commitment and carrying out an action involve different responsibilities.

Together, we can clarify who authorises those activities, what information they use and how their limits are maintained. Existing permissions remain important when systems are connected; a connection does not itself create new decision rights or permission to reuse information.

For example, measuring a property's condition does not automatically authorise conclusions about a resident's behaviour. Access to employment records does not automatically permit workforce profiling. Clear boundaries help suppliers and organisations develop useful capabilities with confidence.

### What does it need from others?

Every product has a scope. Understanding what sits around it helps us design a workable whole.

Your product may rely on another service to check permissions, a person to assess physical evidence, a manager to approve expenditure or a team to resolve a disputed fact. Those are opportunities to make the connections and responsibilities clear.

Where a person needs to accept a duty, we should establish together that they have accepted its scope and have the authority, capacity and cover to carry it out. A name in a field is only part of that arrangement.

### How can we keep the arrangement dependable?

Suppliers bring valuable experience of real operating conditions. We want to draw on that experience when considering missing information, interrupted work, changed permissions, conflicting records and failed connections.

What can continue safely? What needs to pause? Who should be informed? How can unfinished work be handed over? How would an organisation retain its information and outstanding responsibilities if it changed supplier?

Sometimes a lost response leaves us unsure whether an action happened. Checking before retrying can prevent a repeated payment or instruction. Agreeing how to resolve that uncertainty is part of building a dependable connection together.

## Bringing it to life: a repair reported as complete

Imagine a repairs platform that records a promised completion date and receives a contractor's message saying the repair is complete.

The supplier already brings useful capabilities: records of the promise, the job and property, the contractor's report, changes over time and communications sent or received. The housing organisation brings knowledge of its service responsibilities and the arrangements for assessing the work. Other products or services may contribute further evidence.

The collaboration is about bringing those contributions together. A contractor's completion message is evidence, but does not by itself establish that the work was completed satisfactorily. Payment of an invoice does not establish that either.

AOS connects the report, assessment of the work, accepted human responsibility and service outcome, keeping their meanings distinct. If completion remains uncertain, everyone who needs to act should be able to see that. A revised internal target does not erase the original promise to the resident.

If follow-up is needed, an authorised person accepts responsibility. Communication uses the channel currently agreed with the resident and provides the appropriate case-owner and repairs-team contact details. Silence from the resident does not establish that the problem is resolved.

A shared account of the product's contribution might then read:

> Our platform provides the repair records, work events and history, and supports these parts of the workflow. Together with the organisation and its other providers, we can connect those capabilities to assessment of completion, permission checks and accepted human responsibility. These are the connections already available, and these are the areas we could develop together.

That gives us a practical basis for deciding what to do next.

## A starting point for our conversation

You do not need a lengthy submission to begin. A short account under these headings would help us prepare a useful discussion. We can develop it together as our understanding grows.

| Topic | What would help us start |
| --- | --- |
| Your product | Its name, version or service configuration, users and operating context |
| Its contribution | The capabilities you see contributing to AOS and the value they offer |
| Information and actions | What it provides or needs, where information comes from and any limits on its meaning |
| Responsibilities | How information, decisions, permissions and human approval are handled |
| Working with others | Existing integrations and the other products, adapters or human procedures involved |
| Dependable operation | How corrections, outages, changed permissions, uncertain results, recovery and supplier exit are handled |
| What we can build on | Capabilities available now, supporting evidence, possible adaptations and questions still to resolve |
| Your perspective | What we have missed, what may be impractical and how you think the architecture could improve |

Being clear about what is available today and what would need development helps us choose a realistic next step. An honest account of a limitation gives us something useful to work on. We welcome challenge as well as enthusiasm.

## Building confidence as we progress

We can develop our understanding in three stages:

- **Understanding the fit:** agreeing how the product contributes, what it is responsible for and what it needs from others.
- **Agreeing the connections:** establishing how information exchanges preserve meaning, permissions and the handling of change or failure.
- **Demonstrating the behaviour:** testing a particular configuration and recording what it has shown under specified conditions.

Different capabilities may be at different stages. We can explore a useful contribution before every connection exists, then gather evidence as the work develops.

Keeping conclusions specific helps everyone understand what has been established and what remains to be done. Evidence for one connection or function supports a claim about that scope; it does not establish conformity across the whole architecture. Software assessment also cannot establish that an organisation is well governed.

## Developing the technical connections

APIs will be part of some implementations. Our first conversation gives them a purpose: which capabilities should work together, what information they should exchange and what responsibilities they need to preserve.

From there, a particular implementation can define its interfaces, supported versions, identity and security arrangements, and tests. AOS currently offers a reference architecture and proposed assessment approach; there is no live AOS API or certification service.

The immediate opportunity is to arrive together at a strong answer to **“Where does our product fit, and what would be a worthwhile next step?”**

## Let's start with one useful contribution

Choose a capability that you think could make a useful contribution. We can explore its place in the architecture, the connections it needs and the practical value of developing them.

That discussion should work in both directions. Your experience may reveal an unclear assumption, a missing capability or a better way to achieve an intended outcome. We want that feedback to inform the architecture, with proposed changes recorded and considered through the project's change process.

The ambition is a system whose parts work well together because the people building and using them have developed a shared understanding of the whole.

## Further reading and status

The [extension and scoped conformance specification](../Foundation/aos-extension-and-conformance-specification-v0-1.md) sets out the underlying proposed requirements and assessment method. The [specification map](../Foundation/specification-map.md) and [system architecture](../Foundation/aos-00.md) provide more detail about the components and governing decisions.

This is a discussion draft describing intended arrangements. Product-specific assessments, technical connections and operational approvals will need an agreed scope and supporting evidence. The briefing does not endorse a named supplier or certify conformity.

**Project custodian:** Mark Sweeny. **Draft prepared by:** Codex at Mark's request. Item 12a author drafting is complete; substantive review and publication remain separate. CAP-01 and CAP-02 remain deferred to Phase 2.

