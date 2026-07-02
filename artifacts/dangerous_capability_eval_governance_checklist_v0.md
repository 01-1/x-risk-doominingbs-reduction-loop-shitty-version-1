# Dangerous-Capability Evaluation Governance Checklist v0

Date/version: 2026-07-02 / v0
Status: draft local artifact; human review recommended before organizational use
Purpose: provide a non-operational governance checklist for deciding whether, how, and under what authority dangerous-capability evaluations of advanced AI systems should be approved, reviewed, gated, reported, and monitored.

Safety note: This artifact is about governance, authorization, evidence handling, and decision gates. It intentionally excludes evaluation prompts, test procedures, exploit methods, bio/chemical/weapon details, cyber-offensive steps, evasion tactics, or instructions for testing without permission.

Source status: derived from prior local artifacts, especially `ai_eval_safety_checklist_v0.md` and `ai_governance_framework_mini_brief_v0.md`. Current public sources were not browsed in this turn, so framework-specific claims remain source-needed.

## 1. Intended users and use cases

Intended users:
- Human AI safety leads deciding whether a proposed dangerous-capability evaluation is authorized and proportionate.
- Evaluation governance boards or review committees.
- Internal audit, legal, policy, or security reviewers.
- External auditors operating under explicit authorization and confidentiality.

Use cases:
- Pre-approval review before any dangerous-capability evaluation begins.
- Gate review before expanded access, stronger models, broader tool permissions, deployment, release, or publication.
- Post-evaluation review to ensure findings were handled safely and decisions are traceable.

Not a use case:
- Designing the technical tests themselves.
- Running unauthorized red-team activity.
- Publishing sensitive findings without review.

## 2. Governance principle summary

A dangerous-capability evaluation should proceed only when all of the following are true:

1. A named accountable authority has approved the exact scope.
2. The evaluation is necessary for a concrete safety, deployment, mitigation, or governance decision.
3. Evaluator independence and conflict controls are adequate for the stakes.
4. Methods are consent-based, non-operational in public artifacts, and bounded to avoid real-world harm.
5. Stop/escalation conditions are written before testing begins.
6. Evidence handling protects sensitive details while preserving auditability.
7. Results are linked to deployment/release gates, not merely recorded.
8. Disclosure is tiered to avoid enabling misuse while maintaining appropriate accountability.
9. Post-deployment monitoring and incident-response hooks exist for residual risk.

## 3. Pre-authorization checklist

Do not approve the evaluation unless each item is answered clearly.

### 3.1 Authority and consent

- [ ] A named evaluation owner is accountable for approval, pausing, escalation, and final signoff.
- [ ] The model/system owner or appropriate governing body has given written permission for the exact evaluation.
- [ ] In-scope systems, versions, tools, environments, accounts, datasets, time windows, and personnel are listed.
- [ ] Out-of-scope systems, third-party services, public targets, personal accounts, production resources, and private data are explicitly excluded unless separately authorized.
- [ ] Any use of external auditors, contractors, or partners has a confidentiality, data-handling, and authority basis.
- [ ] Legal, privacy, security, and ethics review requirements have been identified for the jurisdiction and organization. This checklist is not legal advice.

Red flag: If authorization is informal, ambiguous, retroactive, or dependent on “don’t ask/don’t tell,” stop and resolve governance before testing.

### 3.2 Decision relevance

- [ ] The evaluation informs a specific decision: mitigation priority, deployment gate, release gate, access tier, monitoring requirement, incident escalation, or research-governance decision.
- [ ] The evaluation question is written in terms of risk evidence needed, not curiosity or demonstration value.
- [ ] The team has documented why lower-risk evidence sources are insufficient.
- [ ] The expected output is a safe governance finding, not a public recipe, benchmark leakage, or capability showcase.

Red flag: If no decision would change after severe findings, the evaluation is not governance-relevant enough to justify dangerous-capability testing.

## 4. Evaluator independence and conflict controls

### 4.1 Independence model

Choose the strongest independence model proportionate to the risk tier:

- Internal team review: acceptable for low-risk, early screening when deployment consequences are limited.
- Independent internal safety/security review: separate reporting line from product/deployment team.
- External auditor or expert review: appropriate for higher-stakes systems, public-impact deployments, or unresolved internal disagreement.
- Regulator/AI safety institute review: only when legally required or explicitly authorized through proper channels.

Checklist:
- [ ] Evaluators have enough access to assess risk, but not unnecessary access that increases harm.
- [ ] Evaluators can report unfavorable findings without retaliation or product-pressure override.
- [ ] Conflicts of interest are documented: launch incentives, commercial pressure, funding, authorship credit, policy agenda, or audit-client dependence.
- [ ] A protected dissent path exists when evaluators and decision owners disagree.
- [ ] Final go/no-go authority is distinct from the team most incentivized to deploy, or the conflict is explicitly mitigated.

## 5. Risk-tier triggers

Use a risk-tier trigger table before evaluation. Thresholds below are governance placeholders, not technical test procedures.

| Tier | Trigger examples | Required governance response |
|---|---|---|
| Tier 0 — routine safety check | Low-impact model or narrow system; no plausible severe dual-use or autonomous-action pathway identified | Standard authorization, basic logging, normal reporting |
| Tier 1 — elevated evaluation sensitivity | General-purpose model, tool access, sensitive user context, or plausible dual-use categories at abstract level | Written scope, owner approval, data plan, stop conditions, safe reporting review |
| Tier 2 — dangerous-capability concern | Preliminary evidence or credible expert concern that the system may materially increase severe misuse, autonomous harm, or systemic safety risk | Independent safety review, stricter sandboxing, restricted evidence access, deployment gate, disclosure plan |
| Tier 3 — severe unresolved concern | Findings suggest risk could be severe if mishandled or deployed without mitigation | Pause expansion/deployment by default, escalate to senior governance and legal/security review, preserve evidence securely, consider incident process |
| Tier 4 — active or imminent harm indicator | Evidence of real-world impact, unapproved external action, exposure of sensitive details, or safety-control failure affecting third parties | Stop evaluation, initiate incident response, contain at high level, preserve evidence, notify authorized stakeholders per policy |

Checklist:
- [ ] A risk tier has been assigned before the evaluation.
- [ ] Tier escalation criteria are written before testing.
- [ ] The team has documented who may move a finding from one tier to another.
- [ ] The response to each tier is tied to deployment, release, access, or mitigation decisions.

## 6. Stop and escalation conditions

Stop the evaluation and escalate if any condition occurs:

- [ ] Scope or authorization becomes unclear.
- [ ] The evaluation appears to require harmful operational detail to proceed.
- [ ] The system attempts, enables, or requests an unapproved external side effect.
- [ ] The evaluation touches third-party systems, public targets, private data, credentials, secrets, or regulated data outside scope.
- [ ] A severe dangerous-capability finding emerges that could cause harm if further probed or disclosed.
- [ ] A safety, legal, privacy, or ethics reviewer raises a good-faith objection.
- [ ] Evidence-handling protections fail or sensitive details are exposed to unauthorized people.
- [ ] Evaluator independence is compromised by pressure to continue, suppress, or reframe findings.

Escalation record should include:
- Date/time, owner, system/version, risk tier, safe summary of trigger, immediate action taken, evidence location/access controls, next decision owner, and whether incident response was activated.

## 7. Deployment and release gates

Dangerous-capability evaluation governance should be coupled to gates. A finding without a gate is often just documentation.

### 7.1 Gate types

- Development gate: whether to continue scaling, tool integration, or capability expansion.
- Access gate: whether to restrict internal users, external testers, API users, or product surfaces.
- Deployment gate: whether the system may be launched, expanded, or connected to real-world tools.
- Publication gate: whether evaluation results, benchmarks, examples, or model details can be shared and at what level.
- Monitoring gate: what post-deployment telemetry, abuse monitoring, incident triggers, and review cadence are required.

### 7.2 Gate checklist

- [ ] Each risk tier maps to a default gate decision or required review.
- [ ] Gate criteria are defined before results are known.
- [ ] Exceptions require named approval, rationale, expiration date, and compensating controls.
- [ ] Severe unresolved findings block deployment/release expansion unless a senior, documented, safety-reviewed exception is approved.
- [ ] Mitigations are verified before a blocked gate is reopened.
- [ ] Gate decisions include residual risk, uncertainty, dissenting views, and follow-up schedule.

## 8. Evidence logging and auditability

The evidence log should be detailed enough for authorized review but not broadly expose harmful content.

Minimum fields:
- Evaluation ID and title.
- Owner, approving authority, evaluators, reviewers.
- Date range and system/model/version/configuration.
- Authorization basis and scope summary.
- Risk tier at start and after findings.
- Decision question and gate affected.
- Method summary at a safe level of abstraction.
- Findings summary, severity, confidence, and uncertainty.
- Sensitive evidence pointer: restricted location/access list, not copied into broad reports.
- Stop/escalation events and decisions.
- Mitigations required and verification status.
- Deployment/release/publication decision.
- Data retention, deletion, and redaction plan.

Checklist:
- [ ] Raw sensitive transcripts or artifacts are not placed in broadly shared documents.
- [ ] Public or wide internal summaries redact operationally harmful details.
- [ ] Evidence labels distinguish observation, assumption, expert judgment, and primary-source claim.
- [ ] The log records what was not tested and why.
- [ ] A reviewer can reconstruct the decision without needing dangerous procedural details.

## 9. Disclosure tiers

Use the narrowest disclosure tier that satisfies safety, accountability, and governance needs.

| Tier | Audience | Appropriate content | Avoid |
|---|---|---|---|
| D0 — restricted raw evidence | Named evaluators and safety/security reviewers | Raw or near-raw evidence when needed for mitigation | Sharing beyond need-to-know |
| D1 — internal governance summary | Decision owners, legal/ethics/security, leadership | Safe summary of scope, severity, decisions, mitigations | Reproducible harmful details |
| D2 — authorized external review | Auditors, regulators, AI safety institutes, partners under approval | Necessary evidence and safe details under agreement/authority | Unapproved submissions or account use |
| D3 — public transparency summary | Public or broad community | High-level risk class, governance action, mitigations, uncertainty | Prompts, methods, exploit paths, bio/weapon/cyber procedures, secrets |
| D4 — do not publish | No broad distribution | Used when even summary risks enabling misuse or violating privacy/security | Any uncontrolled release |

Checklist:
- [ ] Disclosure tier is chosen before report drafting.
- [ ] The public version, if any, is separately reviewed for misuse, privacy, legal, and security risk.
- [ ] The team documents accountability tradeoffs if information is withheld for safety.
- [ ] No external disclosure, submission, contact, or posting occurs without explicit human/organizational approval.

## 10. Post-deployment monitoring and feedback

If a system proceeds after dangerous-capability evaluation, residual risk must be monitored.

Checklist:
- [ ] Monitoring signals are linked to the evaluated risk class at a safe abstraction level.
- [ ] Abuse, anomaly, incident, and near-miss reporting channels are defined.
- [ ] A threshold exists for rolling back access, disabling tools, tightening rate limits, or re-entering incident response.
- [ ] The evaluation owner or successor has a review cadence.
- [ ] New incidents, model updates, tool integrations, user populations, or deployment contexts trigger re-evaluation.
- [ ] Lessons learned feed back into risk-tier triggers, stop conditions, and future authorization templates.

## 11. Relationship to the general AI-safety evaluation checklist

This artifact complements `ai_eval_safety_checklist_v0.md`:

- The general checklist focuses on safe evaluation planning and execution boundaries.
- This governance checklist focuses on authority, independence, risk tiers, gates, evidence handling, disclosure, and monitoring.
- Both require explicit authorization, safe data handling, no harmful operational detail, and no unapproved external actions.

If the two artifacts conflict, use the stricter safety control and escalate for human review.

## 12. One-page pre-approval form

Copy this section for each proposed evaluation.

- Evaluation title:
- Owner / approving authority:
- Evaluators / reviewers:
- System/model/version/configuration:
- Decision the evaluation informs:
- In-scope systems/data/tools/dates:
- Out-of-scope boundaries:
- Authorization basis:
- Initial risk tier:
- Independence model:
- Conflicts and mitigations:
- Stop/escalation conditions:
- Deployment/release gates affected:
- Evidence storage/access plan:
- Disclosure tier plan:
- Post-deployment monitoring hooks:
- Legal/privacy/security/ethics reviews needed:
- Human approval status: not approved / approved with conditions / approved
- Date and signature/record link:

## 13. Review checklist for this artifact

- [x] Covers authorization and scope.
- [x] Covers evaluator independence and conflict controls.
- [x] Covers risk-tier triggers.
- [x] Covers stop and escalation conditions.
- [x] Covers deployment and release gates.
- [x] Covers evidence logging and auditability.
- [x] Covers disclosure tiers.
- [x] Covers post-deployment monitoring.
- [x] Complements rather than duplicates the general AI evaluation checklist.
- [x] Excludes harmful operational evaluation content and unauthorized testing.
- [x] Recommends no outreach, posting, submissions, account use, purchases, or remote writes.

## 14. Future improvements

- Verify current public primary sources for NIST AI RMF, NIST AI Safety Institute materials, and lab preparedness/responsible-scaling frameworks.
- Add a sourced comparison matrix of public framework governance levers.
- Add organization-specific role templates for review boards, evaluators, model owners, legal/privacy, and incident response.
- Add a lightweight evidence-log template file if future turns prioritize implementation support.
