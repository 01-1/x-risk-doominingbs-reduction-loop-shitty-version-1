# X-Risk Reduction Loop State

Mission: Minimize existential risk using safe, lawful, cooperative means, maximizing positive impact.

Interpretation: reduce existential risk via safe, lawful, cooperative, truth-seeking, non-deceptive work. The loop may browse/read public information, write local files, send operational Discord status notifications when configured, and read Discord replies from the user. It must not take other external side effects without human approval; proposals for such actions go in proposals.md.

## Current strategy
1. Maintain a prioritized backlog of safe, high-leverage work with concrete acceptance checks.
2. Convert research into durable local artifacts others can inspect/use.
3. Regularly audit for safety drift, repetitiveness, unsupported claims, opportunity cost, and impact.
4. Prefer practical bottlenecks: AI safety evals, incident preparedness, governance research support, safety tooling, coordination materials, and local documentation/code that improves future safety work.
5. Keep claims calibrated: distinguish established facts, reasoned judgments, assumptions, and source-needed placeholders.
6. For the next worker turns, prioritize source verification and narrow evidence-log patching; if browsing is unavailable, avoid additional broad AI governance/evals artifacts.

## Run status
- Turn: 20, high-level monitor pass.
- User inbox: checked; no new steering beyond the run prompt.
- External side effects this run: none. Local files only.
- Monitor artifact created: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn20_monitor_reprioritization.md.
- Completed artifacts: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/intervention_map_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_eval_safety_checklist_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_incident_response_playbook_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/source_map_and_evidence_rubric_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/external_action_proposal_template.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/governance_brief_template_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_mini_brief_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/dangerous_capability_eval_governance_checklist_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/evidence_log_template_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn10_monitor_audit_and_backlog.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_evidence_log_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/artifact_index_and_usage_guide_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_eval_disclosure_rubric_v0.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn15_source_gap_triage_and_pause_recommendation.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn16_accidental_claim_audit.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn17_human_review_handoff.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn18_source_verification_packet.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn19_worker_pause_checkpoint.md; /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn20_monitor_reprioritization.md.
- Current priority theme until source verification is available: hard-pause broad new AI governance/evals templates, preserve source-needed warnings, use the evidence log plus turn18/turn20 packets as the canonical verification workflow, and avoid any new AI governance/evals artifact unless it performs real source verification or patches a specific verified gap.

## Turn 10 monitor audit summary
- Safety drift: none observed. The loop has stayed local, non-operational, and explicit about approval boundaries.
- Evidence drift: material. Several artifacts are useful scaffolds but contain source-needed/current-policy claims that should not be treated as established until public sources are verified.
- Repetition risk: moderate. The artifact set now has several templates/checklists; workers should avoid more generic templates unless they fill a distinct gap.
- Opportunity-cost note: AI governance/evals remains the best near-term focus because existing artifacts have clear source gaps and high leverage. Biosecurity/nuclear/resilience should be revisited later with source-map-only, non-operational tasks.
- External-action posture: no outreach, posting, submissions, purchases, account/API writes, or remote modifications are warranted at this stage.

## Turn 20 monitor audit summary
- Safety drift: none observed through turns 11-19. Work stayed local-only, governance-level, and explicit about approval boundaries.
- Evidence bottleneck: unresolved and now dominant. The artifact set should not produce new policy/current-framework claims until read-only public source verification is available.
- Repetition risk: high for additional AI governance/evals templates. Turns 15-19 already produced triage, audit, handoff, source-verification, and pause artifacts; more broad scaffolding would likely lower signal.
- Opportunity-cost correction: the next valuable AI governance/evals work is source verification and narrow claim patching, not further synthesis. If browsing is unavailable, workers should record the blocked status and avoid making another broad artifact.
- Worker-queue correction: P1 is decomposed into source-verification sprints: P1-S1 NIST/US AISI, P1-S2 public lab frameworks, P1-S3 evidence-log/minibrief patching.
- External-action posture: unchanged. No outreach, posting, submissions, purchases, account/API writes, public disclosure, or remote modifications are warranted.

## Prioritization rubric for worker turns
Score candidate tasks on:
- Impact relevance: direct connection to AI/bio/nuclear/other existential-risk reduction or resilience.
- Tractability in this loop: can be done safely with local writes and read-only public research.
- Evidence quality: can cite or clearly mark sources/assumptions.
- Leverage: reusable by future work or human reviewers.
- Safety/compliance: avoids operational harm, deception, unauthorized contact, or remote writes.

Default ranking: verified-source work + safe + concrete artifact beats speculative synthesis or additional templates. For AI governance/evals, source verification and narrow evidence-log patching outrank all new local-only templates. If browsing is unavailable, prefer a truthful blocked-status update over inventing more source-needed content.

## Prioritized backlog for upcoming normal turns

### P0 — Worker intake and no-browser gate
- Objective: At the start of each normal worker turn, check user_inbox.md and determine whether read-only public browsing/source inspection is available in that environment.
- Expected artifact: none unless the wrapper requires a local note; if required, create only a concise blocked-status note pointing to turn18_source_verification_packet.md, turn19_worker_pause_checkpoint.md, and turn20_monitor_reprioritization.md.
- Minimum acceptance check:
  - If browsing is available, proceed to P1-S1/P1-S2.
  - If browsing is unavailable and no new user steering exists, do not create another broad AI governance/evals artifact.
  - Do not upgrade candidate URLs, framework names, or current-policy claims without inspecting public sources.

### P1-S1 — Verify NIST / US AISI sources with read-only public research
- Objective: Verify official NIST AI RMF-related materials and directly relevant NIST/US AISI generative/frontier AI governance materials.
- Expected artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_source_verification_v0.md.
- Minimum acceptance check:
  - Records exact source title, publisher/organization, URL/citation, publication/version date if available, and access date.
  - Verifies high-level NIST AI RMF functions/categories at governance-process level only.
  - Records whether each source presents itself as voluntary guidance, profile, standard, official institute material, or another category; does not infer binding legal force.
  - Maps justified support to evidence-log IDs GOV-E-001, GOV-E-002, GOV-E-003, and/or GOV-E-009.
  - Leaves unsupported claims as source-needed, not supported, or not checked in this sprint.
  - No outreach, posting, account use, form submission, external submissions, remote writes, or operational harmful detail.

### P1-S2 — Verify public lab preparedness/responsible-scaling/frontier-safety frameworks
- Objective: Verify at least two official public frontier-lab frameworks at governance-structure level.
- Expected artifact: append to /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_source_verification_v0.md or create a clearly linked source-verification subsection/file if needed.
- Minimum acceptance check:
  - Checks official organization pages or PDFs first.
  - Records exact document/page titles, organizations, URLs/citations, dates/versions if available, and access date.
  - Extracts governance dimensions only: high-level trigger categories, decision authority, review cadence, deployment/release gates, disclosure controls, audit/oversight, incident/post-deployment monitoring, and update process.
  - States whether each framework appears to be a voluntary organizational policy, external commitment, legal obligation, or another category, without overclaiming.
  - Maps justified support to GOV-E-004, GOV-E-010, and GOV-E-011.
  - Avoids dangerous eval procedures, prompts, thresholds in operational detail, exploit details, bio/weapon instructions, or evasion content.

### P1-S3 — Patch evidence log and local AI governance/evals artifacts only after source verification
- Objective: Convert verified source findings into calibrated claim statuses and narrow local artifact patches.
- Expected artifacts: patched /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_evidence_log_v0.md; narrowly patched /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_mini_brief_v0.md and/or /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/dangerous_capability_eval_governance_checklist_v0.md; updated /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/artifact_index_and_usage_guide_v0.md readiness notes.
- Minimum acceptance check:
  - Every upgraded claim has a source ID, title, URL/citation, date/version or not-found note, access date, support scope, and confidence label.
  - Legal/current-policy claims remain dated and calibrated.
  - Unsupported or partially supported claims remain visibly marked.
  - No harmful operational details are introduced.

### P2 — Create a governance-framework comparison matrix after P1-S1 and P1-S2
- Objective: Compare the governance structure of NIST-style process language with verified public lab preparedness/responsible-scaling/frontier-safety frameworks.
- Expected artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/lab_preparedness_framework_comparison_v0.md.
- Minimum acceptance check:
  - Uses source labels, dates, and access dates from P1-S1/P1-S2.
  - Compares governance dimensions only: high-level trigger categories, decision authority, review cadence, deployment/release gates, disclosure controls, audit/oversight, incident/post-deployment monitoring, and update process.
  - Flags uncertainty and non-comparability instead of forcing false alignment.
  - Avoids dangerous eval procedures, prompts, exploit details, bio/weapon instructions, or evasion content.

### Completed — Build and update an artifact index and usage guide
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/artifact_index_and_usage_guide_v0.md.
- Result: indexed all local artifacts, recommended use order, evidence status, safety caveats, stale/source-needed items, and next maintenance actions; turn 14 updated it to include the AI evaluation disclosure rubric and a pause/do-not-extend list for unsupported or repetitive work; included no external-action recommendations.

### Completed — Turn 15 source-gap triage and pause recommendation
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn15_source_gap_triage_and_pause_recommendation.md.
- Result: reaffirmed that source verification is the bottleneck, recommended pausing new broad AI governance/evals artifacts until a verification pass is completed, and listed narrow local-only fallback tasks if browsing remains unavailable.

### Completed — Turn 16 accidental-claim audit
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn16_accidental_claim_audit.md.
- Result: reviewed the AI governance mini-brief and dangerous-capability evaluation governance checklist for accidental overclaims, missing source warnings, unsafe operational detail, and external-action recommendations; found no urgent patch needed, preserved source-needed warnings, and reaffirmed read-only source verification as the next best step.

### Completed — Turn 17 human-review handoff
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn17_human_review_handoff.md.
- Result: created a concise handoff that separates safe internal uses of the local artifact set from uses that must wait for source verification and human review; restated the minimum source-verification acceptance checklist and made no external-action recommendation.

### Completed — Turn 18 source-verification packet
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn18_source_verification_packet.md.
- Result: converted the existing AI governance/evals evidence log into a concrete, bounded workflow for a future browsing-enabled P1 verification pass, including source-target tiers, extraction fields, claim-upgrade rules, red flags, patch targets, and safety constraints; did not verify or upgrade any external claim.

### Completed — Turn 19 worker pause checkpoint
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn19_worker_pause_checkpoint.md.
- Result: assessed diminishing returns for further local-only AI governance/evals work while browsing remains unavailable; recommended pausing broad artifact creation and prioritizing P1 source verification when browsing is available, or human/monitor redirect if it remains unavailable.

### Completed — Turn 20 monitor reprioritization and backlog tightening
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn20_monitor_reprioritization.md.
- Result: audited turns 11-19 for safety drift, evidence bottlenecks, repetition risk, and opportunity cost; decomposed P1 into NIST/US AISI verification, lab-framework verification, and evidence-log patch sprints; added a no-browser blocked-turn policy to prevent more low-value AI governance/evals templates.

### Completed — Draft a safe disclosure rubric for AI evaluation results
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_eval_disclosure_rubric_v0.md.
- Result: consolidated disclosure tiers and decision criteria for AI evaluation results, including restricted raw evidence, internal governance summaries, authorized independent review, aggregated public transparency summaries, and do-not-disclose-without-review cases; emphasized misuse risk, accountability, authority/consent, legal/ethical review, privacy/security, uncertainty, and redaction; avoided procedural harmful details and did not recommend uncontrolled public release.

### P5 — Source-upgrade the AI incident response playbook
- Objective: Improve evidence grounding for ai_incident_response_playbook_v0.md using public/read-only incident-response and AI-incident sources when browsing is available.
- Expected artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_incident_response_source_upgrade_v0.md.
- Minimum acceptance check:
  - Cites current public defensive sources for incident response concepts and AI-specific incident reporting/monitoring where available.
  - Labels claims and dates sources.
  - Keeps cyber/bio/weapon content defensive and non-operational.

### P6 later — Non-operational biosecurity or nuclear source map after AI evidence chain improves
- Objective: Diversify risk-domain coverage without operational harm.
- Expected artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/biosecurity_governance_source_map_v0.md or /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/nuclear_risk_public_source_map_v0.md.
- Minimum acceptance check:
  - Source map only; no protocols, tactical advice, targeting, acquisition, optimization, or evasion details.
  - Uses authoritative public sources and uncertainty labels.
  - No outreach, posting, account use, external submissions, remote writes, or operational harmful detail.

## Completed backlog items

### Completed — Build an intervention map and local artifact roadmap
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/intervention_map_v0.md
- Result: covered AI safety/evals, AI governance, biosecurity, nuclear-risk reduction, civilizational resilience/incident preparedness, and meta/research infrastructure, with local artifact options and safety constraints.

### Completed — Draft responsible AI-safety evaluation checklist
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_eval_safety_checklist_v0.md
- Result: non-operational checklist covering authorization/scope, access boundaries, risk taxonomy, measurement design, mitigations, stop conditions, data handling, reporting, and postmortem.

### Completed — Draft AI incident preparedness / response playbook
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_incident_response_playbook_v0.md
- Result: defensive playbook covering detection, triage, severity levels, escalation, high-level containment, communications, legal/ethical review, evidence preservation, recovery, and lessons learned.

### Completed — Create source and evidence map for future research
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/source_map_and_evidence_rubric_v0.md
- Result: source categories, evidence labels, confidence tags, and missing-evidence list.

### Completed — Build a proposals template for human-reviewed external actions
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/external_action_proposal_template.md
- Result: standardized review template for outreach/submissions/account-use or other external side effects; no action authorized without exact human approval.

### Completed — Draft governance research brief skeleton
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/governance_brief_template_v0.md
- Result: template sections for question, stakeholders, claims/evidence, uncertainty, governance options, failure modes, and next research steps.

### Completed — Fill one high-priority evidence gap with structured source-needed mini-brief
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_mini_brief_v0.md
- Result: NIST AI RMF-style governance mini-brief; current/source-specific claims are marked assumption/source-needed pending verification.

### Completed — Draft a dangerous-capability evaluation governance checklist
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/dangerous_capability_eval_governance_checklist_v0.md
- Result: governance-gate checklist covering authorization, evaluator independence, risk-tier triggers, stop/escalation, deployment gates, evidence logging, disclosure tiers, and monitoring.

### Completed — Create an evidence-log template for governance/evals artifacts
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/evidence_log_template_v0.md
- Result: reusable evidence table and workflow for tracking source status, confidence, freshness risk, and safety notes.

### Completed — Turn 10 monitor audit and backlog refresh
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn10_monitor_audit_and_backlog.md
- Result: audited recent work, identified evidence quality and repetition risks, and reprioritized the next worker queue.

### Completed — Instantiate an evidence log for the AI governance/evals chain because browsing was unavailable
- Artifact: /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_evidence_log_v0.md.
- Result: extracted 12 major claims from the AI governance mini-brief and dangerous-capability evaluation governance checklist; recorded source status, likely source-of-record candidates, freshness risk, safety notes, and exact follow-up questions; did not upgrade any claim to verified.

## Current best next step
If the next turn is a normal worker turn and browsing/source inspection is available, execute P1-S1 first: create or begin /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_source_verification_v0.md by verifying official NIST AI RMF / NIST or US AISI source records using /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn18_source_verification_packet.md, /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/turn20_monitor_reprioritization.md, and /home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_evidence_log_v0.md. If time/tooling allows in the same or next browsing-enabled turn, execute P1-S2 for at least two public lab frameworks. If browsing is still unavailable and no new user steering appears, follow P0/W-no-browser: do not create another broad AI governance/evals artifact; record the blocked status in state/turn notes, preserve source-needed warnings, and ask for human/tooling redirect rather than inventing new unverified governance content.

## Open questions / assumptions to track
- Whether public web/source inspection is available in worker turns; if not, broad AI governance/evals artifact creation should pause rather than producing more source-needed content.
- Which risk domains should dominate after the AI governance/evals source chain is improved; AI remains the near-term focus, but biosecurity/nuclear/resilience source maps should be reconsidered later.
- Whether the user wants any external outreach, publishing, or submissions later; absent explicit approval, do not do it.
- Whether any produced artifact is intended for real-world use; before external use, source verification and human review are required.

## Stop / redirect conditions
Redirect or pause a task if it:
- Requires real-world contact, posting, submission, purchase, account/API write, or remote-system modification without explicit human approval.
- Starts giving operational instructions for harm, evasion, intrusion, weapons, unsafe biological/chemical activity, or unauthorized testing.
- Produces unsupported factual claims without labels or sources.
- Repeats existing artifacts without improving quality, evidence, or usability.
- Attempts another broad AI governance/evals template while browsing/source inspection remains unavailable.
- Uses candidate source names, candidate URLs, or prior local notes as evidence without inspecting the public source.
- Produces a public-ready narrative from source-needed artifacts.
- Treats voluntary frameworks, local risk tiers, candidate URLs, or source-needed notes as verified current policy, standards, consensus, or law.
- Claims x-risk reduction effectiveness from a process artifact without evidence.
- Becomes speculative advocacy instead of producing concrete local artifacts.

## Safety invariants
- No unauthorized external actions.
- No harmful operational detail.
- No deception, coercion, harassment, or manipulation.
- No credential/account use except read-only public research unless explicitly approved.
- Human approval required for real-world outreach, posting, purchases, remote writes, submissions, or use of accounts/API-write actions.
- Prefer defensive, non-operational, consent-based guidance.
