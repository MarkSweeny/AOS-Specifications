# DEC-099 — derived-information restrictions

Document: aos-dec-099-derived-information-restrictions-2026-10-29 · Source revision or record: DEC-99, 29 October 2026

AOS Specifications v1.0 · Edition dated 3 November 2026

Original architecture and specifications: Mark Sweeny, Governance Intelligence. © 2026 Mark Sweeny.

AOS-authored material is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). https://creativecommons.org/licenses/by/4.0/

Preserve third-party credits. Referenced external works remain subject to their own terms.

Canonical collection: https://www.governanceintelligence.co.uk/aos

Publication copy with editorial notices, public references and disclosure edits where applicable.

29 October 2026 · Approved architectural direction by Mark Sweeny in this chat, answering “yes” to substantive question 1. Author: Codex.

## Approved rule

Every transformation or combination must preserve the applicable restrictions of its contributing sources. The proposed use of the resulting information must satisfy those restrictions and account for any additional sensitive information the combination reveals. If the system cannot establish the lineage or permitted use sufficiently, it must withhold that use and refer the uncertainty for accountable review.

Applies to summaries, aggregates, embeddings/search indexes, joins, exports and restored derived copies within the declared governed scope. Transformation supplies no wider purpose or permission; conflicting restrictions can prevent the proposed combination. A different treatment requires an evidenced authorised determination under the governing rules, never mere notice or developer discretion. Completed disclosures and unreachable external copies remain explicit limitations with accountable handling; no recall or universal forgetting guarantee is made. AOS-03 REQ-011/012 and the existing necessity, explicit-consent, separate-governance and review-cycle conditions are retained; no new personal-inference exception is created.

## Controlled amendments and limits

AOS-00/Map v0.49; AOS-02/03 v0.9; Core v0.7; Shared v0.22; Exchange Register v0.21; Source Matrix v0.22. Existing requirement/case IDs and counts retained. AOS-02 REQ-021 and AOS-03 REQ-010 are amended proposed wording implementing the approved direction; ordinary separate review/readiness gates still apply. Existing planned cases 02-VER-009 and 03-VER-006/007 are expanded, not executed. No exact wire schema, profile value, exception, deployment permission or general compliance result is established.

The direction is approved; implementation sufficiency and experimental evidence remain open. Remaining substantive questions S-02–09 have not been decided.

## Verification/provenance

Before/after copies, exact diff, hash manifest and validation are retained locally in `AOS/deliverability-review-2026-10-29/decision-099`. Checks preserve all requirement/case identities, unrelated normative wording and AOS-03 REQ-011/012. Named case expectations are inspected for the approved normal, conflicting, missing-lineage, sensitive-combination, withdrawal/recovery and external-copy limits. This record supplies no independent assurance.

