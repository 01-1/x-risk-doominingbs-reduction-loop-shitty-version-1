# Responsible AI-Safety Evaluation Checklist v0

Purpose: a reusable, non-operational checklist for planning, approving, running, and reviewing AI safety evaluations or red-team exercises. It is designed for consent-based, defensive evaluation under explicit governance. It does not provide exploit, evasion, malware, weapon, bio, credential theft, or harmful operational instructions.

Status: draft local artifact. Source status: based on general safety/evaluation practice and the loop's standing safety constraints; future work should add citations from public AI risk management and eval guidance.

## 1. Core principles

- Authorization first: every evaluation must have an accountable owner, written approval, and a defined scope before testing begins.
- Minimize harm: prefer synthetic, sandboxed, least-capability, least-access methods that answer the safety question without increasing risk.
- Need-to-know handling: sensitive prompts, model outputs, logs, vulnerabilities, and incident details should be accessed only by authorized people.
- No uncontrolled release: do not publish dangerous capabilities, recipes, exploit chains, sensitive data, or unmitigated vulnerabilities.
- Stop when unsafe: predefine stop conditions and empower evaluators to pause without penalty.
- Measure decision-relevant questions: evaluations should inform a concrete release, mitigation, governance, or monitoring decision.
- Preserve auditability: maintain enough documentation for review, while protecting sensitive details.

## 2. Authorization and scope

Before work begins, document:

- Evaluation owner: accountable person/team for approval, safety decisions, and final signoff.
- Authorization basis: contract, internal mandate, model owner permission, platform permission, or other explicit consent.
- Systems in scope: exact models, tools, integrations, datasets, environments, dates, and accounts approved for testing.
- Systems out of scope: anything not named, third-party services without permission, production systems unless explicitly authorized, personal accounts, private data, and public targets.
- Allowed methods: high-level categories of tests, data sources, logging, and review methods.
- Disallowed methods: any harmful, intrusive, deceptive, or non-consensual methods; see forbidden zones below.
- Review gates: who can approve escalation to more sensitive tests, broader access, or changed scope.

Acceptance check: a reviewer who was not in the planning meeting can tell exactly what is authorized and what is not.

## 3. Model and system access boundaries

- Use dedicated test environments where possible.
- Use test accounts and synthetic data unless real data is explicitly necessary and approved.
- Disable or sandbox tools that can create external side effects unless the evaluation specifically requires them and has explicit approval.
- Bound rate limits, spend limits, network access, file access, and tool permissions.
- Keep credentials, API keys, and secrets out of prompts, logs, notebooks, and shared documents.
- Do not attempt to bypass access controls, monitoring, platform policies, or safety systems outside the approved evaluation design.
- If evaluating agentic systems, ensure all write actions, messages, purchases, submissions, code deployments, and account operations are blocked, mocked, or human-approved.

## 4. Risk taxonomy to define before testing

Choose the risk categories relevant to the system. For each, define severity, likelihood, evidence needed, and safe test boundaries.

- Autonomy and agency: undesired pursuit of objectives, inappropriate tool use, unsafe delegation, or failure to defer.
- Cyber misuse: assistance that could enable unauthorized access, malware, credential theft, evasion, or exploitation. Keep testing non-operational and permissioned.
- Bio/chemical misuse: assistance that could materially enable harmful biological or chemical activity. Use abstract or policy-level probes; do not elicit procedures.
- Weapons or physical harm: assistance that could enable violence or construction/use of weapons. Avoid operational detail.
- Persuasion/manipulation: deceptive, coercive, targeted manipulation, fraud, scams, or harassment.
- Privacy/data leakage: memorized or retrieved personal, confidential, proprietary, or regulated information.
- Disallowed external actions: emails, posts, purchases, account changes, submissions, or remote writes without approval.
- Robustness and reliability: hallucination, overclaiming, tool misuse, brittle refusal behavior, or unsafe uncertainty handling.
- Governance compliance: violations of policy, law, contractual limits, or organizational release criteria.

## 5. Measurement design

- State the decision the evaluation will inform, e.g. release readiness, mitigation priority, monitoring requirements, or incident response preparation.
- Define success/failure criteria before seeing results.
- Separate capability, propensity, and control effectiveness where possible.
- Use benign or synthetic prompts and scenarios when they answer the question adequately.
- Avoid benchmarks that require generating harmful procedural content; use rubrics, refusals, summaries, or expert review instead.
- Include negative controls, ordinary-use baselines, and regression checks where feasible.
- Track uncertainty: sample size limits, evaluator judgment calls, model/version changes, and prompt sensitivity.
- Prevent score gaming: do not tune against a narrow hidden checklist and then overclaim broad safety.
- Document known blind spots and tests intentionally not run for safety reasons.

## 6. Mitigations and safeguards during evaluation

- Run in sandboxed or isolated environments for tool-using systems.
- Use allowlists for tools, domains, files, and APIs.
- Use mock services for email, messaging, purchases, code deployment, and external submissions.
- Put a human approval gate in front of any external side effect.
- Apply content filters, logging, and monitoring appropriate to the test.
- Limit access to sensitive outputs and redact where possible.
- Maintain an escalation contact for unexpected severe findings.
- Prefer pair review for tests near safety boundaries.

## 7. Stop conditions

Pause the evaluation and escalate if any of these occur:

- The test begins to produce or require operational instructions for cyber offense, malware, weapons, bio/chemical harm, credential theft, or evasion.
- The system attempts or appears able to take an unapproved external action.
- The evaluation encounters real private data, credentials, secrets, or regulated information outside scope.
- The evaluator discovers a vulnerability or capability that could cause real-world harm if mishandled.
- Test activity affects or may affect third-party systems, users, data, or services without permission.
- Scope, authorization, or reviewer availability becomes unclear.
- A team member raises a good-faith safety objection.

Stop response: preserve relevant logs safely, do not further probe the risky behavior, notify the evaluation owner, and decide whether a formal incident process is needed.

## 8. Data handling

- Classify evaluation data before collection: public, internal, confidential, sensitive safety finding, personal data, regulated data, or secret.
- Collect the minimum data needed for the evaluation decision.
- Use synthetic or anonymized data where possible.
- Define retention period, storage location, access list, and deletion procedure.
- Redact secrets, personal data, and dangerous procedural details from broad reports.
- Keep raw high-risk transcripts in restricted storage; publish only safe summaries where appropriate.
- Record model versions, system prompts/configuration identifiers, tool permissions, date/time, and evaluator notes.

## 9. Reporting

A responsible evaluation report should include:

- Scope and authorization summary.
- System/version evaluated and material configuration details.
- Risk categories tested and not tested.
- Method summary at a safe level of detail.
- Findings by severity and confidence.
- Evidence snippets redacted to avoid harmful detail.
- Recommended mitigations or release conditions.
- Residual risk and uncertainty.
- Data handling and access notes.
- Reviewer names/roles or approval record.
- Clear distinction between established observations, judgments, assumptions, and open questions.

Do not include operational instructions, exploit chains, malware details, weapon/bio procedures, secrets, or private data in broadly distributed reports.

## 10. Postmortem and continuous improvement

After the evaluation:

- Compare results against pre-registered expectations and decision criteria.
- Identify which safeguards worked, failed, or were missing.
- Record near misses and ambiguous cases.
- Update test harnesses, rubrics, mitigations, and stop conditions.
- Decide whether follow-up evaluation is needed before release or deployment changes.
- Feed safe, generalized lessons into organizational policy and training.
- Archive or delete data according to the data plan.

## 11. Explicit forbidden zones

The evaluation must not include or facilitate:

- Testing without explicit permission from the system/model/platform owner.
- Unauthorized access, intrusion, exploitation, account takeover, credential theft, phishing, or social engineering.
- Malware, persistence, evasion, stealth, botnets, or command-and-control instructions.
- Bypassing access controls, monitoring, rate limits, safety systems, or platform terms outside approved defensive testing.
- Uncontrolled release of dangerous capabilities, vulnerability details, or procedural harmful instructions.
- Real-world weapon, bio, chemical, or physical-harm procedures.
- Deceptive or coercive interaction with people.
- Doxxing, harassment, extortion, blackmail, fraud, spam, or market manipulation.
- External side effects such as messages, posts, purchases, submissions, code deployments, or account changes without exact human approval.

## 12. Short human pre-flight checklist

Use this immediately before starting an evaluation.

- [ ] Written authorization exists for this exact system, date range, team, and test scope.
- [ ] In-scope and out-of-scope systems are listed clearly.
- [ ] A named owner can pause, escalate, or terminate the evaluation.
- [ ] Test methods avoid forbidden zones and harmful operational detail.
- [ ] Tool access, network access, spend, and external side effects are sandboxed, mocked, or blocked.
- [ ] Real user data, credentials, and secrets are not used unless explicitly approved and protected.
- [ ] Risk taxonomy, severity levels, and decision criteria are defined.
- [ ] Stop conditions and emergency contacts are known to all evaluators.
- [ ] Logging, storage, access control, retention, and redaction plan are in place.
- [ ] Reporting plan avoids publishing sensitive details while preserving decision-useful evidence.
- [ ] The team has confirmed that the evaluation is necessary, proportionate, lawful, and consent-based.

## 13. Reviewer quick scoring rubric

Rate each area before approving the evaluation: Green = adequate, Yellow = needs mitigation, Red = do not proceed.

| Area | Green | Yellow | Red |
|---|---|---|---|
| Authorization | Written, specific, accountable | Informal or partly unclear | Absent or disputed |
| Scope | Precise in/out boundaries | Some ambiguity | Open-ended or includes non-consenting systems |
| Safety methods | Non-operational, sandboxed, least access | Some sensitive tests with mitigations | Harmful or uncontrolled methods |
| Data handling | Minimal, classified, access-controlled | Plan incomplete | Sensitive data unmanaged |
| Stop/escalation | Clear triggers and contacts | Triggers vague | No pause path |
| Reporting | Safe summaries and restricted details | Redaction plan unclear | Broad release of dangerous/private details |

Proceed only when all red items are resolved and yellow items have documented mitigations accepted by the owner.

## 14. Known gaps for future versions

- Add citations to public AI risk management and evaluation guidance.
- Add example severity matrix that remains non-operational.
- Add a lightweight template for evaluation approval records.
- Add organization-specific legal/privacy review hooks.
