# AI Governance Framework Mini-Brief v0

Working title: Using NIST AI RMF-style governance to structure dangerous-capability evaluation oversight
Date/version: 2026-07-02 / v0
Status: draft, local analysis only
Author/reviewer: Hermes x-risk loop worker / human review pending
External action status: no outreach, submissions, posting, account use, or remote writes authorized.

Important evidence note: This worker turn did not have a live web-browsing tool available. URLs below are public/source-of-record candidates to verify in a future read-only research pass. Claims about exact current versions, page contents, or legal obligations should be treated as source-needed until verified.

## 1. Decision question

How can teams use a NIST AI Risk Management Framework-style governance process to make dangerous-capability evaluations for frontier or high-impact AI systems more consistent, auditable, and safety-preserving without creating operational misuse guidance?

Target user: human reviewer, AI governance researcher, or organizational safety lead evaluating internal governance options.

Desired output: short governance analysis and next research agenda, not a recommendation to contact, submit, or implement anything externally.

## 2. Scope and exclusions

### In scope
- AI system area: frontier, general-purpose, or otherwise high-impact AI systems where severe misuse, loss-of-control, or systemic-safety concerns may be relevant.
- Governance levers: risk-management frameworks, evaluation gates, documentation, internal review boards, independent auditing, incident reporting, and publication controls.
- Geography/institution type: framework-level analysis relevant to labs, deployers, auditors, standards bodies, and public-sector AI safety institutes.
- Time horizon: near-term institutional practice and research agenda.

### Out of scope
- Operational instructions for cyber, biological, chemical, weapon, evasion, or other harmful capabilities.
- Designing red-team prompts, exploits, bypasses, or dangerous evaluation tasks.
- Testing any real system without permission.
- Legal advice or claims about binding obligations without current primary-source verification.
- Outreach, lobbying, public posting, submissions, or use of accounts without explicit human approval.

## 3. Executive summary

Bottom line: A NIST AI RMF-style process is useful as a neutral management scaffold for dangerous-capability evaluation governance because it emphasizes repeatable risk mapping, measurement, management, and governance rather than ad hoc testing. For x-risk-relevant work, the missing layer is usually not a generic risk-management vocabulary but concrete institutional commitments: who authorizes evaluations, what triggers deeper review, how results are handled, what deployment or release gates follow, and how independent scrutiny occurs.

Main uncertainty: This brief has not verified the latest public NIST, AI Safety Institute, EU, or lab framework documents during this turn. The analysis should therefore be treated as a structured hypothesis and agenda for a sourced follow-up, not as a current-policy summary.

Most decision-relevant evidence to verify next:
- NIST AI Risk Management Framework 1.0 and any current NIST Generative AI Profile / AI Safety Institute materials.
- Frontier AI lab preparedness or responsible-scaling frameworks.
- Official government or summit documents on advanced AI safety commitments and evaluation expectations.
- Independent research reports on dangerous-capability evaluations and audit governance.

Recommended next step: Perform a read-only verification pass that extracts the exact current NIST framework functions, compares them against 2-3 public lab preparedness frameworks, and fills a claim table with primary-source citations.

Confidence: medium for the framework-level reasoning; low for any current-document details until live source verification is completed.

## 4. Risk pathway and theory of change

### Risk pathway
- Trigger/capability class: AI systems may acquire or expose capabilities that increase severe misuse, systemic disruption, or loss-of-control risks. [ASSUMPTION]
- Governance gap: evaluations can be inconsistent, under-scoped, over-disclosed, or disconnected from deployment/release decisions. [ASSUMPTION]
- Harm pathway: weak evaluation governance may fail to detect high-risk behaviors before deployment, or may publicize methods/results in ways that enable misuse. [ASSUMPTION]
- Scale of possible harm: potentially severe for frontier systems; exact risk varies by capability, access model, deployment context, and safeguards. [ASSUMPTION]
- Current mitigations: public frameworks, lab policies, internal safety reviews, external audits, standards processes, and emerging AI safety institutes appear relevant but need current-source verification. [SOURCE_NEEDED]
- Residual concern: governance artifacts may be voluntary, unevenly enforced, poorly audited, or too slow for rapid model-development cycles. [ASSUMPTION]

### Theory of change
- Intervention: adapt a NIST AI RMF-style process to dangerous-capability evaluation governance.
- Mechanism of impact: clarify roles, require documented risk mapping and evaluation plans, link evaluation results to deployment gates, preserve evidence for review, and reduce unsafe disclosure.
- Required adoption/enforcement: organizational policy, leadership accountability, evaluator independence, review-board authority, and documentation practices.
- Key assumptions: better process quality changes real deployment decisions; evaluators can measure relevant risks without increasing misuse; organizations face incentives to comply.
- Indicators of success: clear evaluation authorization records, documented scope and stop conditions, traceable decisions, safer disclosure practices, post-deployment monitoring, and lessons-learned updates.
- Possible negative side effects: checkbox compliance, false confidence from weak metrics, regulatory capture, slowed beneficial safety research, or over-sharing dangerous evaluation detail.

## 5. Stakeholder map

| Stakeholder | Role / authority | Incentives | Constraints | Concerns / objections | Engagement status |
|---|---|---|---|---|---|
| AI developers/labs | Build systems; set internal gates; control access and deployment | Reduce catastrophic and reputational risk; ship useful products | Commercial pressure; secrecy; fast iteration | Burdensome process, disclosure risk, ambiguous thresholds | No contact unless approved |
| AI deployers/product teams | Integrate models into real workflows | Reliability, safety, compliance, user trust | Limited visibility into upstream model internals | Need usable go/no-go criteria | No contact unless approved |
| Evaluators/auditors | Design and review tests under authorization | Accurate measurement; independence; safety | Access limits; dual-use methods; liability | Need standards and protected reporting channels | No contact unless approved |
| Standards bodies/NIST-like institutions | Define risk-management language and profiles | Broad adoption; interoperability; neutrality | Consensus processes; rapid technology change | Avoiding vague or obsolete standards | No contact unless approved |
| Regulators/policymakers | Create incentives, duties, or reporting requirements | Public safety; accountability | Legal authority limits; international competition | Over/under-regulation and enforceability | No contact unless approved |
| Civil society/affected communities | Represent public-interest concerns | Transparency, rights, risk reduction | Limited access to technical evidence | Capture, secrecy, inadequate redress | No contact unless approved |
| Security/incident response teams | Handle discovered vulnerabilities/incidents | Containment and evidence preservation | Need-to-know restrictions; speed | Dangerous disclosure and unclear escalation | No contact unless approved |
| Researchers/forecasters | Analyze risk, evaluate evidence, track trends | Truth-seeking and prioritization | Uncertainty, sparse data, publication risks | Overclaiming, stale evidence, misuse | No contact unless approved |

## 6. Claims and evidence table

| Claim | Evidence label | Source / citation candidate | Confidence | Decision relevance | Notes / caveats |
|---|---|---|---|---|---|
| NIST AI RMF is a public risk-management framework relevant to AI governance. | PRIMARY candidate | NIST AI Risk Management Framework page: https://www.nist.gov/itl/ai-risk-management-framework | Medium | High | Verify latest version and exact function names in follow-up. |
| A generic risk-management framework can structure dangerous-capability evaluation governance but does not by itself define sufficient frontier-model thresholds. | ASSUMPTION / expert-judgment | Needs comparison with lab preparedness frameworks and eval research. | Medium | High | Central crux: process scaffolds need concrete trigger/threshold design. |
| Dangerous-capability evaluations require authorization, scope control, data-handling rules, and careful disclosure to avoid increasing misuse risk. | ASSUMPTION supported by prior local checklist | Local artifact: ai_eval_safety_checklist_v0.md; external sources needed. | Medium | High | Follow-up should cite public eval governance reports. |
| Public lab preparedness/responsible-scaling frameworks are useful comparison points for eval triggers and deployment gates. | PRIMARY candidate / SOURCE_NEEDED | Candidate sources: Anthropic Responsible Scaling Policy, OpenAI Preparedness Framework, Google DeepMind safety framework pages. | Low | High | Must verify current versions and avoid treating voluntary policies as binding law. |
| Government AI safety institutes and standards bodies may improve evaluation norms by convening, testing, and publishing guidance. | PRIMARY / EXPERT_SYNTHESIS candidate | Candidate sources: NIST AI Safety Institute materials; UK/US AI safety institute publications; official summit documents. | Low | Medium | Current mandates and outputs need verification. |
| Poorly designed evaluation publication can increase harmful capability diffusion. | ASSUMPTION / SOURCE_NEEDED | Need cited research or policy guidance on responsible disclosure for AI evals. | Medium | High | Keep examples non-operational. |

## 7. Current governance landscape: provisional map

This section is intentionally provisional because current public sources were not browsed this turn.

Relevant framework families to verify:
1. NIST AI Risk Management Framework and related generative-AI profile/safety institute outputs. [PRIMARY candidate]
2. Voluntary or institutional frontier-model safety commitments, preparedness frameworks, and responsible-scaling policies. [PRIMARY candidate]
3. Standards and assurance processes for AI risk management, auditability, documentation, and conformity assessment. [PRIMARY/SOURCE_NEEDED]
4. Government or international policy documents on advanced AI evaluations, incident reporting, and safety institutes. [PRIMARY/SOURCE_NEEDED]
5. Independent research reports on dangerous-capability evaluations, external auditing, and disclosure governance. [RESEARCH_REPORT/SOURCE_NEEDED]

Likely gap: many frameworks discuss risk management at a high level, while practical dangerous-capability evaluation governance requires detailed but safely handled operational decisions: authorization, evaluator independence, thresholds, escalation, deployment gating, data retention, and controlled reporting. [ASSUMPTION]

## 8. Governance levers and options

| Option | Mechanism | Benefits | Risks / failure modes | Evidence need | Local next step |
|---|---|---|---|---|---|
| Evaluation authorization charter | Defines who may run dangerous-capability evals and under what scope | Reduces unauthorized or unsafe testing | Can become bureaucratic or vague | Examples from lab/audit practice | Draft a local charter template |
| Risk-tier trigger table | Links model/capability/deployment signals to review depth | Makes gates explicit | Threshold gaming, false precision | Compare lab frameworks | Build non-operational comparison table |
| Evaluation disclosure policy | Separates internal details, regulator/auditor reports, and public summaries | Reduces misuse from over-disclosure | Excess secrecy can reduce accountability | Responsible disclosure sources | Draft safe reporting rubric |
| Independent review or audit | Adds external scrutiny and conflict checks | Improves credibility | Capture, access limits, confidentiality barriers | Audit governance literature | Map audit design questions |
| Incident and post-deployment monitoring | Catches risks missed pre-deployment | Feedback loop for governance | Underreporting, unclear responsibility | Incident database and reporting sources | Link to incident playbook artifact |
| Versioned evidence log | Preserves claims, sources, dates, and decisions | Auditable learning | Maintenance burden | Documentation standards | Create a simple evidence-log template |

## 9. Failure modes and safeguards

1. Checkbox compliance: teams complete forms without changing deployment decisions.
   - Safeguard: require named decision owners, documented go/no-go criteria, and post-decision review.

2. False confidence from weak evaluations: measured tasks fail to cover relevant risk pathways.
   - Safeguard: include uncertainty statements, adversarial review, and periodic test revision.

3. Unsafe disclosure: reports reveal methods or details that help misuse.
   - Safeguard: tiered reporting, need-to-know access, and public summaries that focus on governance implications rather than procedural detail.

4. Incentive conflict: internal evaluators face pressure to approve launches.
   - Safeguard: independent review authority, escalation paths, and protected dissent channels.

5. Fragmentation: each lab or jurisdiction uses incompatible categories.
   - Safeguard: align terminology with public standards where appropriate while preserving stricter internal gates.

6. Regulatory capture or performative governance: standards lag behind frontier capabilities.
   - Safeguard: sunset/review dates, incident-triggered updates, and external expert input when approved.

## 10. Recommendations for local research only

1. Verify primary sources: read the current NIST AI RMF and related NIST AI safety/generative-AI materials; extract exact terms, dates, and functions.
2. Create a comparison matrix of 2-3 public lab preparedness/responsible-scaling frameworks, focusing on triggers, thresholds, governance authority, publication rules, and auditability.
3. Draft a non-operational dangerous-capability evaluation governance checklist that complements the existing AI eval safety checklist.
4. Build a safe disclosure rubric for evaluation results: internal-only, shared-with-auditor/regulator, public summary, or do-not-publish.
5. Mark every claim with evidence labels and avoid making legal/current-policy claims until primary sources are verified.

## 11. Next research steps

- Read-only browsing task: verify URLs, dates, current versions, and exact language for NIST AI RMF and related AI Safety Institute materials.
- Evidence extraction task: fill a source table with quotations/paraphrases from primary documents and stable URLs.
- Comparison task: compare NIST-style process categories with public lab preparedness frameworks.
- Artifact task: produce `dangerous_capability_eval_governance_checklist_v0.md` as a local, non-operational checklist.
- Review task: have a high-level monitor check for overclaims, stale sources, operational detail, and opportunity cost.

## 12. Review checklist

- [x] Decision question is narrow and governance-focused.
- [x] No outreach, posting, submissions, purchases, account/API writes, or remote modifications were performed.
- [x] No operational harmful instructions, exploit steps, evasion, weapon, or bio/chemical procedural detail included.
- [x] Unsupported/current claims are marked as assumptions, source-needed, or candidates for verification.
- [x] Stakeholders and failure modes are included.
- [x] Next steps are local/read-only unless separately approved by a human.
