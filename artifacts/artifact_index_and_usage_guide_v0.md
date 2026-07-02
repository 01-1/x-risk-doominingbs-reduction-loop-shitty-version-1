# Artifact Index and Usage Guide v0

Created: 2026-07-02, turn 12
Updated: 2026-07-02, turn 20 — added monitor reprioritization and no-browser blocked-turn policy.
Scope: local x-risk reduction artifacts in `/home/vi/xriskdoominningbs/.xrisk_loop/artifacts`.
Purpose: help a human reviewer or future worker quickly choose the right artifact, understand evidence limits, and avoid unsafe or unsupported use.

## Important status notes

- This index is an integration artifact, not a source-verified policy brief.
- Live public-source verification was not available in this worker turn. Therefore, artifacts that mention current AI governance frameworks, lab preparedness frameworks, or legal/policy status should still be treated as source-needed unless a later source-verification artifact upgrades them.
- No artifact should be used for real-world outreach, publication, compliance advice, model release decisions, or operational evaluation without human review and source verification.
- All artifacts are intended to remain non-operational: no harmful instructions, no unauthorized testing, no exploit guidance, no weapon/bio/chemical procedural detail, and no external side effects without exact human approval.

## Recommended use order

1. Start with `intervention_map_v0.md` to understand the overall safe local work plan and candidate x-risk domains.
2. Use `source_map_and_evidence_rubric_v0.md` to apply evidence labels and identify which claims need stronger sourcing.
3. For AI governance/evals work, read `ai_governance_framework_mini_brief_v0.md`, then immediately cross-check its source gaps using `ai_governance_framework_evidence_log_v0.md`.
4. For evaluation governance, pair `ai_eval_safety_checklist_v0.md` with `dangerous_capability_eval_governance_checklist_v0.md`, then use `ai_eval_disclosure_rubric_v0.md` to decide what can be shared, with whom, and under what review controls.
5. For incident preparedness, use `ai_incident_response_playbook_v0.md`, while noting that it still needs a future source upgrade.
6. For new research outputs, start from `governance_brief_template_v0.md` and/or `evidence_log_template_v0.md`.
7. Before a browsing-enabled P1 verification pass, use `turn18_source_verification_packet.md` as the bounded source-checking workflow.
8. If browsing remains unavailable and no new user steering appears, read `turn19_worker_pause_checkpoint.md` and `turn20_monitor_reprioritization.md` before creating any more local-only AI governance/evals artifacts; the current default is to avoid new broad governance/evals artifacts and record the blocked status.
9. Before any proposed external action, use `external_action_proposal_template.md` and place the completed proposal in `proposals.md` for human review.
10. Use `turn10_monitor_audit_and_backlog.md`, `turn20_monitor_reprioritization.md`, and this index to choose the next local task.

## Artifact inventory

| Artifact | Purpose | Intended user | Evidence status | Safety caveats | Recommended maintenance action |
|---|---|---|---|---|---|
| `intervention_map_v0.md` | Maps safe local x-risk reduction intervention areas and artifact roadmap. | Future workers, human reviewer setting priorities. | Mostly strategic synthesis and assumptions; not source-verified. | Do not treat prioritization as settled; avoid operationalizing bio/nuclear/cyber items. | Revisit after AI evidence chain improves; add sources if used externally. |
| `turn_1_worker_backlog.md` | Early backlog snapshot from the first worker turn. | Historical reference only. | Superseded by later working state and turn 10 audit. | Do not use as current priority list. | Keep archived; no active maintenance needed. |
| `ai_eval_safety_checklist_v0.md` | Non-operational checklist for responsible AI-safety evaluation planning. | Evaluators, reviewers, governance staff, future workers. | Practical synthesis; needs source grounding before external use. | Requires authorization, consent, scope control, and safe disclosure; not a test procedure. | Later source-upgrade with public evaluation governance and safety-eval references. |
| `ai_incident_response_playbook_v0.md` | Defensive AI incident preparedness and response playbook. | Safety teams, incident coordinators, reviewers. | Useful but source-light; contains a source/evidence status section. | High-level defensive workflow only; no cyber/bio/weapon operational detail. | P5: source-upgrade using public defensive incident-response and AI-incident sources when browsing is available. |
| `source_map_and_evidence_rubric_v0.md` | Evidence labels, confidence tags, source categories, and research workflow. | Any worker creating or auditing claims. | Meta-framework; partly based on general research norms, not source-verified. | Must not be used to launder weak claims into verified claims. | Use continuously; update if future workers define better evidence labels. |
| `external_action_proposal_template.md` | Template for human-reviewed external side effects. | Worker considering outreach, submission, posting, purchase, or account/API write action. | Procedural local template; no external facts required. | Completing the template is not approval; exact human approval is still required. | Keep as the required gate for all external-action recommendations. |
| `governance_brief_template_v0.md` | Structured template for AI governance research briefs. | Researchers and future workers. | Template only; evidence quality depends on filled brief. | Must preserve scope/exclusions and avoid unsupported policy claims. | Use for future focused briefs; do not create more broad templates unless needed. |
| `ai_governance_framework_mini_brief_v0.md` | Provisional mini-brief on using NIST AI RMF-style process language for dangerous-capability evaluation oversight. | Governance researcher, human reviewer. | Source-needed/current-policy claims are explicitly provisional. | Do not cite as verified current policy; do not imply legal force. | P1: verify NIST materials and at least two lab preparedness/responsible-scaling/frontier-safety frameworks with read-only public sources. |
| `dangerous_capability_eval_governance_checklist_v0.md` | Governance-gate checklist for dangerous-capability evaluation oversight. | Governance reviewers, safety leads, future workers. | Mostly synthesis; source grounding still needed. | Governance-only; excludes eval prompts, methods, exploit detail, and unauthorized testing. | Pair with evidence log; later align with verified frameworks and disclosure rubric. |
| `evidence_log_template_v0.md` | Reusable template for tracking claims, sources, confidence, freshness risk, and safety notes. | Workers performing source verification. | Template only. | Do not upgrade claims without checking primary or high-quality sources. | Use for every future source-verification or source-upgrade task. |
| `turn10_monitor_audit_and_backlog.md` | Monitor audit of safety drift, evidence drift, repetition risk, and worker queue. | Future workers and monitor turns. | Internal audit based on local artifacts; no external factual claims. | Follow redirect rules; avoid template proliferation. | Refresh at next high-level monitor turn or after P1/P3/P4 completion. |
| `ai_governance_framework_evidence_log_v0.md` | Claim-by-claim evidence log for the AI governance mini-brief and dangerous-capability governance checklist. | Browsing-enabled source-verification worker, human reviewer. | All entries remain source-needed; no claims upgraded. | Useful as a queue, not as proof. Avoid operational eval details. | Use as the primary P1 verification queue. |
| `artifact_index_and_usage_guide_v0.md` | This guide: index, evidence caveats, recommended use order, and maintenance actions. | Human reviewer and future workers. | Integration/synthesis based on local file inventory. | Does not verify external facts or authorize external actions. | Update whenever major artifacts are added, source-upgraded, or deprecated. |
| `ai_eval_disclosure_rubric_v0.md` | Rubric for deciding safe disclosure tiers for AI evaluation results and related governance summaries. | Evaluators, governance reviewers, incident coordinators, future workers. | Local synthesis; not source-verified; suitable as an internal safety scaffold only. | Do not use to justify uncontrolled public release; excludes raw dangerous eval details, secrets, private data, exploit methods, and harmful procedures. External disclosure still requires authority, human review, and applicable legal/ethical review. | Integrate with evaluation checklist, dangerous-capability governance checklist, and incident playbook; later source-upgrade with public disclosure, vulnerability coordination, and AI-safety governance references. |
| `turn17_human_review_handoff.md` | One-page-style handoff separating safe internal uses from uses that must wait for source verification and human review. | Human reviewer, future worker deciding whether artifacts are ready for use. | Local integration/handoff only; no external facts verified and no claims upgraded. | Reinforces local-only posture, source-needed warnings, and exact-approval requirement for external actions. | Use before any real-world use of the artifact set; update after a source-verification pass changes readiness status. |
| `turn18_source_verification_packet.md` | Concrete packet for the next browsing-enabled AI governance/evals source-verification pass. | Browsing-enabled worker or human reviewer performing P1. | Local preparation artifact only; no external claims verified or upgraded. | Read-only public research only; governance-level extraction; no operational eval details or external side effects. | Use immediately before creating `ai_governance_framework_source_verification_v0.md`; update if the evidence log changes. |
| `turn19_worker_pause_checkpoint.md` | Checkpoint assessing diminishing returns from further local-only AI governance/evals artifacts while browsing is unavailable. | Future worker, monitor, or human deciding whether to continue, pause, or redirect. | Local process artifact only; no external claims verified or upgraded. | Reinforces source-needed status and discourages unsupported template proliferation. | Use if a future worker still lacks browsing; prefer P1 source verification once available. |
| `turn20_monitor_reprioritization.md` | High-level monitor reprioritization that decomposes P1 into source-verification sprints and defines no-browser blocked-turn behavior. | Future workers, monitor turns, human reviewer deciding whether to continue or pause. | Local process artifact only; no external claims verified or upgraded. | Reinforces hard pause on broad AI governance/evals templates without source access; no external-action recommendation. | Use as the current worker-queue authority until P1 source verification or the next monitor turn. |

## Stale or source-needed priorities

Highest priority source-needed items:

1. `ai_governance_framework_mini_brief_v0.md` — verify current NIST AI RMF materials and public lab preparedness/responsible-scaling/frontier-safety frameworks.
2. `turn18_source_verification_packet.md`, `turn20_monitor_reprioritization.md`, and `ai_governance_framework_evidence_log_v0.md` — use together as the bounded workflow, decomposed worker queue, and claim queue for the above verification.
3. `turn19_worker_pause_checkpoint.md` — use as the local-only fallback decision gate if browsing is still unavailable; turn 20 tightens this to a default no-new-broad-artifact posture.
4. `dangerous_capability_eval_governance_checklist_v0.md` — align governance gates and disclosure tiers with verified public sources after P1.
5. `ai_incident_response_playbook_v0.md` — source-upgrade with public defensive incident-response and AI-specific incident sources.
6. `ai_eval_safety_checklist_v0.md` — source-upgrade with public safety-evaluation governance sources before real-world use.
7. `ai_eval_disclosure_rubric_v0.md` — source-upgrade before using for real-world release, publication, vulnerability coordination, or transparency decisions.

## Pause / do-not-extend list until source verification is possible

To reduce repetition and unsupported-claim risk, future worker turns should pause the following unless they can add sources, integrate existing artifacts, or perform a monitor audit:

- New broad AI governance templates that do not verify sources or improve use of existing artifacts.
- Additional dangerous-capability evaluation planning artifacts that are not tied to authorization, disclosure controls, and evidence logging.
- Claims about current policies, lab frameworks, law, regulation, or compliance obligations without primary-source verification and dates.
- Public-facing summaries derived from local source-needed artifacts.

Safe fallback behavior if browsing remains unavailable:

- Record the blocked status in state/turn notes and preserve P1 as the top priority.
- Do not create new broad AI governance/evals templates, public-facing summaries, or new source-needed policy claims.
- Only perform a narrow warning/cross-reference patch if a concrete missing warning is identified; otherwise avoid additional local-only AI governance/evals content.

Superseded or archival:

- `turn_1_worker_backlog.md` is superseded by `working_state.md` and `turn10_monitor_audit_and_backlog.md`.

## Next-task selection guide

If public web/read-only browsing is available:

- Do P1: create `ai_governance_framework_source_verification_v0.md` using `ai_governance_framework_evidence_log_v0.md` as the verification queue.
- Verify document names, dates/versions, URLs, and access dates. Keep legal/current-policy claims calibrated and dated.
- Do not contact organizations, use accounts, submit forms, or write to remote systems.

If browsing remains unavailable:

- Follow `turn20_monitor_reprioritization.md` and `turn19_worker_pause_checkpoint.md`: do not create another broad AI governance/evals artifact, do not produce public-facing summaries, and do not upgrade source-needed claims.
- Check `user_inbox.md`; if no new steering exists, record the blocked status in state/turn notes and preserve P1 as the top priority.
- Only create a one-page blocked-status note if the wrapper requires an artifact; otherwise avoid new local-only AI governance/evals content.

If a monitor turn occurs next:

- Audit whether source verification has happened. If not, keep the no-new-broad-artifact posture and decide whether to pause the loop, request browsing/tooling, or explicitly pivot to a distinct non-operational source-map queue.

## Human-review checklist before external use

- [ ] Are all current-policy or current-framework claims source-verified with dates/access dates?
- [ ] Are source-needed assumptions still visibly marked?
- [ ] Has a human checked that the artifact is suitable for the intended real-world audience?
- [ ] Does the artifact avoid operational harmful detail?
- [ ] Does it avoid legal/compliance claims beyond the evidence?
- [ ] Are any external actions routed through `proposals.md` and explicitly approved before execution?
