# Turn 17 Human-Review Handoff: What Is Safe to Use Now vs. What Must Wait

Date/version: 2026-07-02 / turn 17
Status: local handoff artifact; no public-source verification performed
Scope: clarify how a human reviewer or future worker should use the current local x-risk reduction artifact set while source verification remains blocked/unperformed.

## Bottom line

The current artifact set is useful as internal scaffolding for AI governance, evaluation safety, disclosure control, and incident preparedness. It is not yet suitable as an externally cited policy brief, compliance guide, public recommendation, or evidence-backed comparison of current AI governance frameworks.

Until read-only public source verification is completed, use the artifacts for internal planning, review structure, and claim triage only. Treat all statements about current NIST materials, AI safety institutes, public lab preparedness/responsible-scaling/frontier-safety frameworks, law, regulation, compliance, and framework efficacy as source-needed unless a future verification artifact upgrades them with exact citations, dates, and access dates.

## Safe to use now, with caveats

1. Internal artifact navigation
   - Use `artifact_index_and_usage_guide_v0.md` to find the right local artifact and understand source/safety caveats.
   - Caveat: the index does not verify external facts.

2. Claim triage and verification planning
   - Use `ai_governance_framework_evidence_log_v0.md` as the canonical source-verification queue.
   - Use `evidence_log_template_v0.md` for any new claim tracking.
   - Caveat: evidence-log entries are not evidence; they are questions to verify.

3. Internal governance scaffolding
   - Use `ai_eval_safety_checklist_v0.md`, `dangerous_capability_eval_governance_checklist_v0.md`, and `ai_eval_disclosure_rubric_v0.md` to structure human review conversations around authorization, scope, evidence handling, stop conditions, disclosure control, and post-deployment monitoring.
   - Caveat: keep use high-level and governance-focused; do not treat placeholder tiers or process suggestions as standards.

4. Defensive incident-preparedness thinking
   - Use `ai_incident_response_playbook_v0.md` as a local defensive workflow scaffold for detection, triage, escalation, communications, recovery, and lessons learned.
   - Caveat: it still needs source-upgrading before real-world adoption.

5. External-action gating
   - Use `external_action_proposal_template.md` before any outreach, posting, submission, account/API-write action, purchase, or remote-system modification.
   - Caveat: filling out a proposal is not approval; exact human approval is still required before action.

## Must wait for source verification and human review

Do not use the current artifacts for any of the following until source verification and human review are complete:

1. Public-facing claims about NIST AI RMF, NIST/US AISI materials, UK or other AI safety/security institute mandates, or lab frontier-safety/preparedness frameworks.
2. Claims that a voluntary lab framework is legally binding or represents industry consensus.
3. Claims that a local checklist or risk-tier table is a standard, regulation, compliance requirement, or validated best practice.
4. Claims that a governance process demonstrably reduces catastrophic or existential risk, unless supported by strong sources and labeled with appropriate uncertainty.
5. Legal, compliance, jurisdiction-specific, or professional advice.
6. Any publication of dangerous-capability evaluation details, raw results, benchmark-sensitive material, exploit paths, evasion methods, private information, secrets, or weapon/bio/chemical/cyber operational detail.
7. Outreach, posting, submissions, account/API-write actions, purchases, remote writes, or public disclosure without exact human approval.

## Recommended next review sequence

1. Read `artifact_index_and_usage_guide_v0.md` for map and caveats.
2. Read `turn15_source_gap_triage_and_pause_recommendation.md` and `turn16_accidental_claim_audit.md` to understand the current pause rationale.
3. Use `ai_governance_framework_evidence_log_v0.md` to verify GOV-E-001 through GOV-E-004 first:
   - NIST AI RMF title/version/date/functions and related current NIST/US AISI materials.
   - At least two public lab preparedness/responsible-scaling/frontier-safety frameworks, limited to governance dimensions.
4. Only after that, patch or annotate `ai_governance_framework_mini_brief_v0.md` and `dangerous_capability_eval_governance_checklist_v0.md` with verified source labels.
5. Then consider P2 comparison work; do not compare frameworks from memory or unverified candidate URLs.

## Minimal source-verification acceptance checklist

A future browsing-enabled worker or human reviewer should not mark a claim verified unless the verification note includes:

- Exact source title.
- Source publisher/authoring organization.
- URL or stable citation.
- Publication date, version date, or explicit "undated" label.
- Access date.
- Short non-operational paraphrase or exact brief quotation supporting the claim.
- Scope limit: whether the source supports the exact claim, only a weaker claim, or only a related claim.
- Safety note for any dual-use or disclosure-sensitive material.

## Safety posture

This handoff recommends no external action. It reinforces the current local-only posture: read-only public research is acceptable when available; all other external side effects require exact human approval. The artifact intentionally avoids operational harmful detail and does not upgrade any source-needed claim.

## Acceptance check

- Produced a one-page-style human-review handoff rather than another broad governance/evals template.
- Clearly separated safe internal uses from uses that must wait for source verification and human review.
- Identified the next source-verification sequence and minimum acceptance checklist.
- Included no harmful operational detail and no external-action recommendation.
