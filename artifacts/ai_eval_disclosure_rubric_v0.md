# AI Evaluation Disclosure Rubric v0

Created: 2026-07-02, turn 13
Status: draft local artifact; human review and source verification required before real-world use
Scope: non-operational rubric for deciding how to disclose AI-safety evaluation results, especially dangerous-capability or misuse-relevant findings.

Purpose: help authorized reviewers choose a disclosure tier that preserves accountability and decision usefulness while reducing misuse, privacy, legal, and security risk. This rubric consolidates disclosure themes from `ai_eval_safety_checklist_v0.md` and `dangerous_capability_eval_governance_checklist_v0.md`.

Safety note: This artifact does not authorize outreach, publication, submission, public posting, regulator contact, account/API writes, or any other external side effect. It also does not include evaluation prompts, exploit paths, bio/chemical/weapon procedures, evasion methods, private data, secrets, or reproducible harmful detail.

Source status: local synthesis only. No public-source verification was available in this worker turn. Treat all recommendations as draft governance guidance pending human/source review.

## 1. Core disclosure principles

1. Need-to-know by default: share sensitive evaluation details only with people or bodies that need them for mitigation, governance, legal/ethical review, or authorized oversight.
2. Accountability still matters: withholding operational details should not become a reason to hide the existence, severity, uncertainty, or governance implications of important findings from appropriate decision makers.
3. Separate raw evidence from safe summaries: raw or near-raw evidence may be necessary for mitigation, but broad reports should use redacted, high-level summaries.
4. Authority and consent first: external disclosure requires appropriate authorization, legal/ethical review, and any required confidentiality or reporting pathway.
5. Minimize enablement: do not disclose information that materially helps non-authorized actors reproduce harmful capabilities, bypass safeguards, identify vulnerable systems, or misuse private data.
6. Preserve auditability: keep enough restricted documentation for authorized review, postmortem, and accountability.
7. Date and scope claims: state what system/version/configuration was evaluated and avoid overgeneralizing beyond the evidence.

## 2. Disclosure tiers

Use the narrowest tier that satisfies safety, accountability, and governance needs.

| Tier | Audience | Appropriate content | Required controls | Do not include |
|---|---|---|---|---|
| T0 — Restricted raw evidence | Named evaluators, safety/security leads, mitigation engineers, legal/ethics reviewers with need-to-know | Raw logs, transcripts, artifacts, or detailed evidence needed to verify/mitigate a finding | Access list, secure storage, retention/deletion plan, no forwarding, audit trail | Broad circulation, public links, unrelated examples, unnecessary personal/secret data |
| T1 — Internal governance summary | Decision owners, release/deployment gatekeepers, senior safety leadership, incident commanders | Safe summary of scope, severity, confidence, affected decision, mitigations, residual risk, uncertainty, dissent | Redaction review; pointer to restricted evidence rather than embedding sensitive detail | Reproducible procedures, prompts, exploit chains, sensitive model/system details beyond need |
| T2 — Authorized independent review | External auditor, regulator, AI safety institute, partner, or expert reviewer operating under proper authority/approval | Evidence and context necessary for independent assessment, tailored to the reviewer’s mandate | Explicit authorization, confidentiality/data-handling terms where applicable, legal/ethics review, disclosure log | Unapproved submissions, informal sharing, details outside the reviewer’s mandate |
| T3 — Aggregated public transparency summary | Public, research community, customers/users, or broad stakeholders when approved | High-level risk class, governance action taken, mitigation status, limits, uncertainty, and safe lessons learned | Separate publication review for misuse/privacy/security/legal risk; approved communications owner | Sensitive methods, detailed prompts, exploit paths, bio/weapon/cyber procedures, secrets, private data, benchmark leakage |
| T4 — Do not disclose beyond restricted review without further approval | No broad audience; possibly only T0/T1 holders until reviewed | A placeholder that a sensitive issue exists may be recorded internally; broader content waits for review | Senior safety/legal/security review; explicit re-review date and accountable owner | Any uncontrolled external or broad internal release |

## 3. Decision criteria

Before choosing a tier, answer each question and record the rationale.

### 3.1 Misuse and harm-enablement risk

- Could the information help a non-authorized actor cause harm, evade safeguards, exploit systems, or reproduce a dangerous capability?
- Does it contain procedural detail, prompts, code, configurations, vulnerabilities, or examples that materially lower barriers to misuse?
- Would aggregation or redaction preserve decision usefulness while reducing enablement?

Default: if enablement risk is high or uncertain, keep raw details in T0 and use T1/T3 summaries only after review.

### 3.2 Accountability and governance need

- Who must know to make or audit a release, mitigation, incident, policy, or monitoring decision?
- Would withholding even a high-level summary prevent appropriate oversight or allow unsafe deployment?
- Is an independent reviewer needed because of severity, conflict of interest, public impact, or unresolved disagreement?

Default: high accountability need can justify T1 or T2 disclosure, but not uncontrolled public release of sensitive methods.

### 3.3 Authority, consent, and legal/ethical review

- Who owns or controls the evaluated system, data, and results?
- Is the proposed recipient authorized to receive this information?
- Are confidentiality, privacy, contractual, regulatory, or jurisdiction-specific constraints identified?
- Has a qualified human reviewed the disclosure plan where stakes are non-trivial?

Default: absent clear authority for external disclosure, do not contact, submit, post, or share externally; write a proposal for human review instead.

### 3.4 Privacy, security, and confidential information

- Does the material include personal data, credentials, secrets, proprietary information, user content, private vulnerabilities, or regulated data?
- Can it be redacted, aggregated, anonymized, or replaced with a pointer to restricted evidence?
- Are storage, retention, deletion, and access controls documented?

Default: sensitive personal/security/confidential information stays T0 unless a reviewed basis exists for broader sharing.

### 3.5 Evidence quality and uncertainty

- Are findings observations, assumptions, evaluator judgments, or source-verified claims?
- What system/version/configuration/date does the evidence cover?
- Could the result be an artifact of prompt sensitivity, small sample size, evaluator judgment, or changed model behavior?
- Does the report clearly state what was not tested?

Default: uncertainty should be disclosed to authorized decision makers, but public summaries should avoid overstated or sensational claims.

## 4. Quick tier-selection workflow

1. Classify the raw material: raw evidence, restricted evidence pointer, internal summary, independent-review packet, or public summary.
2. Identify the decision the disclosure supports: mitigation, release gate, incident response, oversight, public transparency, or archival audit.
3. Score misuse risk: low, medium, high, or unknown.
4. Score accountability need: low, medium, high, or legally/ethically mandatory.
5. Check authority: internal authorized, external authorized, public approved, or unclear.
6. Choose the narrowest tier that satisfies the decision need.
7. Redact or aggregate before any broader tier.
8. Record the chosen tier, rationale, approver, date, recipients, evidence pointer, and re-review date.

## 5. Default decision table

| Condition | Default tier | Escalation / review action |
|---|---|---|
| Raw logs or transcripts contain sensitive harmful procedural content | T0 | Restrict access; summarize safely for T1 if needed for governance |
| Finding affects deployment/release gate but raw details are risky | T1 plus T0 pointer | Decision owner and safety/legal/security review |
| Severe finding with conflict of interest or public-impact implications | T1 initially; consider T2 | Independent review proposal under proper authority |
| Need for public accountability after mitigation without enabling misuse | T3 after approval | Publish only aggregated safe summary; exclude methods and sensitive examples |
| Personal data, secrets, credentials, or proprietary data appear in evidence | T0 | Privacy/security review and redaction before any broader tier |
| Unclear authorization, unclear law/policy, or uncertain misuse risk | T4/T0 | Pause broad disclosure; obtain human review |
| Third-party systems/users may be affected | T1/T2 only if authorized | Incident/legal/security process; no informal sharing |

## 6. Minimum disclosure record

For every non-trivial evaluation finding, record:

- Evaluation ID/title.
- System/model/version/configuration and date range.
- Finding summary at a safe level of abstraction.
- Severity, confidence, and uncertainty.
- Chosen disclosure tier and rationale.
- Audience/recipients or access group.
- Approver and review date.
- Restricted evidence pointer and access controls.
- Redactions or aggregation performed.
- External-action status: none, proposed for human review, or explicitly approved outside this rubric.
- Re-review date or closure condition.

## 7. Redaction checklist for broader summaries

Before moving from T0/T1 to T2/T3, confirm:

- [ ] No procedural harmful instructions, prompts, exploit chains, malware details, weapon/bio/chemical procedures, or evasion steps.
- [ ] No credentials, secrets, private user data, regulated data, or unnecessary proprietary details.
- [ ] No third-party identifiers unless legally/ethically approved and necessary.
- [ ] No benchmark leakage or test details that would undermine future safety evaluations.
- [ ] Claims are scoped to evaluated versions/configurations and dates.
- [ ] Severity and uncertainty are stated without sensationalism.
- [ ] Mitigation status and residual risk are included where appropriate.
- [ ] A qualified human has reviewed external or broad disclosure.

## 8. Stop conditions

Stop drafting or distributing a disclosure and escalate for human review if:

- The report begins to include operational harmful detail.
- Authorization, audience, or legal/ethical basis is unclear.
- The finding suggests active or imminent harm.
- The disclosure could compromise third-party systems, privacy, confidential information, or safety mitigations.
- Reviewers disagree materially about misuse risk or accountability need.
- Anyone proposes posting, outreach, submission, or account/API write action without exact approval.

## 9. Relationship to other artifacts

- Use with `ai_eval_safety_checklist_v0.md` for safe evaluation planning and reporting constraints.
- Use with `dangerous_capability_eval_governance_checklist_v0.md` for risk tiers, deployment/release gates, and evidence logging.
- Use with `external_action_proposal_template.md` if any external disclosure, outreach, posting, or submission is proposed. The proposal is not approval.
- Use with `evidence_log_template_v0.md` to separate verified claims from assumptions and record source status.

## 10. Known gaps for future versions

- Add source citations from public AI evaluation, risk management, coordinated vulnerability disclosure, incident response, and responsible publication guidance when browsing is available.
- Add organization-specific legal/privacy/security review hooks.
- Align terminology with any verified public AI safety institute, NIST-style, or lab framework sources after source verification.
- Create a compact one-page disclosure decision form if a human reviewer requests operational usability improvements.
