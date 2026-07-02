# AI Incident Preparedness and Response Playbook v0

Purpose: Provide a concise, defensive, non-operational playbook for teams preparing for AI-related safety incidents. This is a planning artifact, not legal advice, security instructions, or a substitute for organization-specific incident response procedures.

Scope: Applies to incidents involving AI systems, model deployments, AI-enabled workflows, evaluation environments, and downstream uses where safety, security, legal, reputational, or public-interest harms may arise.

Safety boundary: Keep response actions authorized, lawful, proportionate, and defensive. Do not perform unauthorized access, deception, exploit development, credential collection, evasion, public disclosure of dangerous details, or uncontrolled reproduction of harmful capabilities.

## 1. Preparedness before an incident

### Ownership and roles
- Incident lead: accountable for triage, coordination, decision log, and closure.
- Technical lead: understands the affected AI system, evaluation setup, data, and deployment controls.
- Safety/risk lead: evaluates misuse, loss-of-control, systemic, and affected-stakeholder risks.
- Legal/ethics/privacy reviewer: advises on legal duties, data handling, disclosure, and affected-party obligations.
- Communications lead: prepares accurate internal/external updates approved by responsible humans.
- Executive sponsor: makes high-impact tradeoff decisions and authorizes major containment or disclosure steps.

### Minimum preparation artifacts
- System inventory: model/system name, owner, deployment location, access paths, data classes, dependencies, and rollback owners.
- Contact tree: names or roles for escalation, including after-hours path.
- Severity rubric: pre-agreed levels and response targets.
- Evidence protocol: where logs, prompts, outputs, screenshots, approvals, and timelines are preserved.
- Communications protocol: who can speak internally/externally, review steps, and sensitive-detail redaction rules.
- Stop/rollback authority: who may pause a model, feature, eval, data pipeline, integration, or release.

## 2. Detection and intake

Possible detection channels:
- Monitoring alerts: unusual output rates, policy violations, anomalous user reports, safety filter triggers, data leakage signals, or suspicious integration behavior.
- Human reports: employees, evaluators, customers, researchers, or affected stakeholders.
- Evaluation findings: unexpected capabilities, unreliable safeguards, dangerous generalization, or severe failure modes.
- External signals: credible public reports, regulator notices, partner notifications, or vulnerability disclosures.

Intake record should capture:
- Who reported it and when.
- A short factual description of observed behavior.
- Affected system, version, environment, and access mode.
- Known impact or potential impact.
- Evidence location, without copying sensitive data unnecessarily.
- Immediate safety concerns and whether active harm appears ongoing.

## 3. Triage and severity levels

Use the lowest sufficient level, but escalate quickly when uncertainty is high and possible harm is severe.

### S0 — False alarm / informational
Criteria:
- No plausible safety, security, privacy, legal, or stakeholder harm after initial review.
Response:
- Record rationale, close or monitor, and update detection rules if useful.

### S1 — Minor localized issue
Criteria:
- Low-risk failure with limited scope; no sensitive data exposure, no dangerous capability disclosure, no ongoing misuse, and no vulnerable population impact.
Response target:
- Assign owner, fix through normal process, document lessons.

### S2 — Material but contained incident
Criteria:
- Affected users, repeated unsafe behavior, moderate policy failure, limited confidential data exposure, or evaluation finding requiring mitigation before broader release.
Response target:
- Same-day incident lead assignment, containment plan, legal/privacy review if relevant, stakeholder update as appropriate.

### S3 — Severe safety/security incident
Criteria:
- Active or likely significant harm; substantial data exposure; model behavior enabling serious misuse at a high level; failure of critical safeguards; uncontrolled propagation through integrations; or public-interest implications.
Response target:
- Immediate escalation to executive sponsor, safety/risk lead, legal/privacy, and communications; pause/limit affected capabilities where authorized; preserve evidence; prepare coordinated communications.

### S4 — Critical / potentially catastrophic or systemic incident
Criteria:
- Plausible large-scale physical, societal, national-security, biosecurity, cyber, or infrastructure risk; severe loss of control; or credible evidence that continued operation could materially increase catastrophic risk.
Response target:
- Immediate all-hands incident command for responsible roles; safest available containment or shutdown actions under authority; urgent legal/ethical review; coordinate with appropriate trusted partners or authorities only through approved human decision-makers.

## 4. High-level response workflow

1. Stabilize intake
- Confirm report is logged.
- Assign temporary incident lead if none exists.
- Avoid public speculation and avoid sharing sensitive technical details in broad channels.

2. Triage severity
- Apply severity rubric.
- State known facts, unknowns, and assumptions.
- Choose initial response tempo and escalation path.

3. Contain at a high level
- Consider pausing, rate-limiting, rolling back, disabling a feature, restricting access, isolating an evaluation environment, or reverting to a safer configuration.
- Ensure actions are authorized and proportionate.
- Do not attempt unauthorized probing, exploit reproduction, or external testing.

4. Preserve evidence
- Preserve relevant logs, prompts, outputs, model/config versions, deployment timestamps, alerts, access records, and decisions.
- Maintain chain-of-custody notes for sensitive evidence.
- Minimize copying of personal, confidential, or hazardous information.

5. Analyze causes and impact
- Identify affected systems and users/stakeholders.
- Determine whether the issue is ongoing, reproducible in an authorized safe environment, or already contained.
- Separate factual findings from hypotheses.
- Use domain experts for specialized safety, legal, privacy, or security questions.

6. Communicate responsibly
- Internal updates should be factual, brief, and role-appropriate.
- External communications should be reviewed by accountable humans and avoid harmful operational details.
- If disclosure to affected parties, partners, regulators, or authorities may be needed, prepare a human-review proposal and follow legal/ethical obligations.

7. Recover safely
- Apply mitigations, tests, approvals, and rollback plans before restoring capability.
- Verify that monitoring covers recurrence.
- Avoid declaring closure until responsible owners agree severity-specific exit criteria are met.

8. Learn and improve
- Conduct a blameless postmortem proportionate to severity.
- Track corrective actions with owners and due dates.
- Update evals, guardrails, monitoring, data handling, and governance processes.

## 5. Escalation triggers

Escalate immediately if any of the following are plausible:
- Active real-world harm or credible imminent harm.
- Sensitive data exposure, especially personal, confidential, or regulated data.
- Behavior that could substantially aid serious misuse if details spread.
- Evidence of unauthorized access or compromise.
- Affected critical infrastructure, healthcare, public safety, national security, or vulnerable populations.
- Incident crossing organizational boundaries: partners, customers, vendors, open-source releases, or public deployments.
- Strong uncertainty combined with high downside risk.

## 6. Communications principles

- Be truthful, concise, and uncertainty-aware.
- Avoid blame and premature root-cause claims.
- Share only what recipients need for safety and response.
- Avoid operational details that could enable harm.
- Document who approved each major communication.
- If external contact is contemplated, create a proposal for human approval before action unless already covered by the organization's established incident policy and authorized humans.

## 7. Evidence preservation checklist

Preserve when relevant and authorized:
- Incident report and timeline.
- Affected system/model/version/configuration.
- Prompts, outputs, tool calls, policy decisions, and safety-filter events.
- Deployment and change history.
- Access logs and relevant user/session identifiers, handled under privacy rules.
- Screenshots or transcripts, redacted where appropriate.
- Decisions, approvals, and communications.
- Mitigation steps and verification results.

Avoid:
- Unnecessary copying of personal data.
- Sharing hazardous details in broad channels.
- Reproducing potentially dangerous behavior outside approved safe environments.

## 8. Recovery and closure criteria

For closure, document:
- Severity level and final incident summary.
- Actual and potential impact.
- Root cause or best current explanation, with uncertainty.
- Containment and remediation completed.
- Verification performed.
- Stakeholders notified or rationale for not notifying.
- Residual risks accepted by accountable humans.
- Follow-up actions with owners and dates.

## 9. Blameless postmortem template

- Incident title and date.
- Severity and affected systems.
- Executive summary.
- Timeline of detection, triage, escalation, containment, recovery, and closure.
- What went well.
- What went poorly.
- Root causes and contributing factors.
- Missed detection or prevention opportunities.
- Policy, eval, monitoring, staffing, or governance gaps.
- Corrective actions, owners, and deadlines.
- Evidence/source quality notes: primary logs, human reports, assumptions, unresolved questions.

## 10. One-page quick-start checklist

When an AI incident is reported:

1. Log the report
- Record time, reporter, affected system, observed behavior, and evidence location.

2. Assign an incident lead
- Name one accountable coordinator and backup.

3. Triage severity
- S0 informational, S1 minor, S2 material contained, S3 severe, S4 critical/systemic.
- If uncertain and downside is high, escalate.

4. Protect people and systems
- Consider authorized pause, rollback, access restriction, or feature disablement.
- Do not take unauthorized external action or probe systems without permission.

5. Escalate to required roles
- Technical owner, safety/risk owner, legal/privacy/ethics, communications, executive sponsor as severity requires.

6. Preserve evidence
- Save relevant logs, versions, prompts/outputs, alerts, decisions, and timeline.
- Minimize sensitive data copying and restrict access.

7. Communicate carefully
- Share factual updates with need-to-know recipients.
- Avoid harmful operational details and premature conclusions.

8. Analyze and remediate
- Identify scope, impact, cause, mitigations, and verification plan.

9. Recover only after checks
- Confirm mitigation, monitoring, approvals, and rollback plan.

10. Close with lessons learned
- Write a short postmortem and track corrective actions.

## Source/evidence status

This v0 playbook is a reasoned synthesis based on common incident management patterns and AI safety governance needs, without live web research in this turn. Future versions should cite public incident response standards, AI risk management frameworks, and domain-specific disclosure guidance.
