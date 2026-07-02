# Source Map and Evidence Rubric v0

Purpose: provide a reusable, safety-conscious map of public/read-only sources for future x-risk research, plus a common evidence-labeling scheme. This is a starting map, not a claim that every listed source is current or exhaustive. Future workers should verify URLs, dates, authorship, and relevance with read-only browsing before relying on a source for decisions.

Scope and safety constraints:
- Use public/read-only research only unless a human explicitly approves a specific external action.
- Prefer primary documents, peer-reviewed work, and clearly attributed expert syntheses.
- Label uncertainty and avoid implying consensus where only a small expert community or advocacy group supports a claim.
- Do not collect sensitive personal information, use accounts, submit forms, contact authors, or alter remote systems without approval.
- Do not reproduce operationally harmful details from dual-use sources; summarize at a defensive, policy, or preparedness level.

## Evidence-quality labels

Use one or more labels on every substantive claim in future artifacts.

1. [PRIMARY]
   - Definition: Original source for a policy, dataset, official statement, law/regulation, standards document, incident report, model card/system card, organizational report, or technical paper by the team that produced the relevant work.
   - Strengths: Best for what the source directly states or did; usually lowest risk of quotation drift.
   - Limits: May be incomplete, self-serving, outdated, or outside independent review.
   - Use for: exact organizational commitments, legal text, official standards, disclosed evaluation methods, incident timelines.

2. [PEER_REVIEWED] / [RESEARCH_REPORT]
   - Definition: Academic peer-reviewed paper, preprint, technical report, or research-institute report with methods, citations, and named authors.
   - Strengths: Often gives methods and uncertainty; useful for causal claims and technical detail.
   - Limits: Preprints are not peer reviewed; peer review does not guarantee correctness; field may move quickly.
   - Use for: empirical findings, risk models, taxonomies, evaluations, historical analyses.

3. [EXPERT_SYNTHESIS]
   - Definition: Review, handbook, agenda, workshop report, testimony, or analysis by recognized domain experts or institutions summarizing multiple sources.
   - Strengths: Efficient orientation; captures expert judgment and context.
   - Limits: May reflect author/institution values, selection bias, or contested assumptions.
   - Use for: research landscape summaries, policy tradeoff framing, intervention prioritization.

4. [FORECAST]
   - Definition: Prediction market, forecasting-platform question, expert elicitation, scenario exercise, or quantified probability estimate.
   - Strengths: Makes uncertainty explicit; useful for prioritization when evidence is incomplete.
   - Limits: Forecast resolution criteria may not match the real decision; forecaster populations can be biased; long-horizon x-risk forecasts are especially uncertain.
   - Use for: timelines, risk likelihood ranges, scenario prioritization, early-warning indicators.

5. [MEDIA]
   - Definition: News article, magazine feature, podcast transcript, blog post reporting on events or summarizing expert views.
   - Strengths: Useful for leads, recent events, quotes, and public communication context.
   - Limits: Not sufficient alone for technical or policy claims; may simplify or overstate.
   - Use for: finding primary documents, tracking public discourse, identifying dated claims to verify.

6. [ASSUMPTION]
   - Definition: Reasoned but unverified premise used to proceed when no stronger evidence has been checked.
   - Strengths: Prevents hidden uncertainty and enables incremental work.
   - Limits: Should not be treated as fact; must be targeted for later verification if important.
   - Use for: local prioritization judgments, provisional heuristics, unverified source availability.

Suggested confidence tags:
- Confidence: high = multiple independent strong sources or direct primary evidence.
- Confidence: medium = one strong source or several weaker consistent sources.
- Confidence: low = plausible but thinly sourced, stale, or contested.
- Confidence: unknown = not yet checked.

## Source categories by domain

### 1. AI safety, evaluations, and technical governance

Primary/source-of-record candidates:
- AI labs' public technical reports, model/system cards, preparedness frameworks, responsible scaling policies, safety evaluations, and post-deployment updates. [PRIMARY]
- Standards bodies and government technical agencies: NIST AI Risk Management Framework, NIST AI Safety Institute materials, ISO/IEC AI standards, OECD AI policy resources, relevant national AI safety institute publications. [PRIMARY]/[EXPERT_SYNTHESIS]
- Frontier AI safety commitments or summit declarations where available from official government or institutional pages. [PRIMARY]

Research and synthesis candidates:
- Academic venues and archives for AI safety, ML security, interpretability, robustness, evaluations, and assurance: arXiv, NeurIPS/ICML/ICLR/AAAI/FAccT proceedings, ACL venues for language-model risks, USENIX/IEEE security venues for defensive ML security. [PEER_REVIEWED]/[RESEARCH_REPORT]
- AI safety organizations and programs: METR, ARC Evals/ARC-style evaluation work, Center for AI Safety, FAR AI, Redwood Research, Alignment Research Center, Anthropic/OpenAI/Google DeepMind safety publications, GovAI, CSET, RAND reports, Institute for AI Policy and Strategy where relevant. [RESEARCH_REPORT]/[EXPERT_SYNTHESIS]
- Incident and vulnerability tracking sources with defensive framing: AI Incident Database, Partnership on AI resources, model behavior/evaluation benchmark papers, public bug bounty policy pages where relevant. [PRIMARY]/[MEDIA]/[RESEARCH_REPORT]

Future read-only evidence gaps:
- Verify the current official URLs and latest versions of major AI risk-management frameworks.
- Build a short annotated bibliography for responsible capability evaluations and dangerous-capability eval governance.
- Compare lab preparedness/responsible-scaling frameworks by evaluation triggers, thresholds, governance, and publication policy.
- Identify which AI incident databases are maintained and how they define inclusion criteria.

### 2. AI governance and policy

Primary/source-of-record candidates:
- Laws, executive orders, parliamentary/legislative bills, agency rules, consultation documents, official guidance, and government strategy documents. [PRIMARY]
- International organization documents: OECD, UN, UNESCO, Council of Europe, G7/Hiroshima process, EU AI Act pages, national AI safety institute publications. [PRIMARY]/[EXPERT_SYNTHESIS]
- Official testimony, committee reports, regulatory impact assessments, and standards-roadmap documents. [PRIMARY]

Research and synthesis candidates:
- CSET, RAND, Brookings, Carnegie Endowment, GovAI, IAPS, R Street/CSIS/Belfer-style policy analysis when relevant and nonpartisan care is used. [EXPERT_SYNTHESIS]/[RESEARCH_REPORT]
- Academic work on compute governance, export controls, liability, auditing, evaluations, assurance, standards, incident reporting, and international coordination. [PEER_REVIEWED]/[RESEARCH_REPORT]
- Forecasting and scenario analyses on AI timelines, deployment patterns, and governance bottlenecks. [FORECAST]/[EXPERT_SYNTHESIS]

Future read-only evidence gaps:
- Create a jurisdiction-specific index of current AI safety/evaluation/reporting obligations.
- Track which policy proposals have empirical support versus mostly theoretical arguments.
- Collect neutral summaries of compute governance options and failure modes.
- Identify official channels for incident reporting without using them absent human approval.

### 3. Biosecurity and pandemic-risk reduction

Primary/source-of-record candidates:
- WHO guidance, Biological Weapons Convention documents, national public-health agency guidance, CDC/ECDC/UKHSA-style official pages, biosafety/biosecurity regulator materials, and official outbreak reports. [PRIMARY]
- Institutional biosafety committee policies and public biosafety manuals, when used only for governance/preparedness framing. [PRIMARY]
- Official reports from commissions or national academies on pandemic preparedness, pathogen research oversight, and biosecurity governance. [PRIMARY]/[EXPERT_SYNTHESIS]

Research and synthesis candidates:
- Peer-reviewed public-health, epidemiology, biosafety, biosecurity, and global health security literature. [PEER_REVIEWED]
- Johns Hopkins Center for Health Security, NTI Bio, Nuclear Threat Initiative biosecurity work, Global Health Security Index documentation, National Academies reports, and similar expert syntheses. [EXPERT_SYNTHESIS]/[RESEARCH_REPORT]
- Historical analyses of outbreak response, surveillance, supply chains, and risk communication. [PEER_REVIEWED]/[EXPERT_SYNTHESIS]

Safety handling:
- Keep all biosecurity work defensive and governance-oriented.
- Do not reproduce experimental protocols, pathogen optimization details, evasion tactics, or instructions enabling misuse.
- Summarize dual-use issues at policy level and point future workers to safe-review constraints, not methods.

Future read-only evidence gaps:
- Verify current WHO and national guidance relevant to biosafety governance and outbreak preparedness.
- Build a non-operational map of biosecurity governance levers: screening, oversight, surveillance, PPE/supply chains, public-health capacity, and norms.
- Identify high-quality evaluations of pathogen-screening and outbreak early-warning systems without operationalizing misuse.

### 4. Nuclear-risk reduction and strategic stability

Primary/source-of-record candidates:
- Treaties, official doctrine statements, arms-control agreements, IAEA materials, UN Office for Disarmament Affairs pages, national defense posture documents, and official crisis-communication agreements. [PRIMARY]
- Official verification and safeguards documents where public. [PRIMARY]

Research and synthesis candidates:
- SIPRI Yearbook/resources, Bulletin of the Atomic Scientists, Arms Control Association, Carnegie Endowment nuclear policy work, Federation of American Scientists public nuclear information, RAND strategic stability research, Belfer Center work, and peer-reviewed international security literature. [EXPERT_SYNTHESIS]/[RESEARCH_REPORT]
- Historical case studies on crisis instability, command-and-control, near misses, arms-control verification, and risk-reduction measures. [PEER_REVIEWED]/[EXPERT_SYNTHESIS]
- Forecasts/scenarios on escalation pathways and arms-control prospects, treated cautiously. [FORECAST]

Safety handling:
- Keep discussion at risk-reduction, governance, history, and policy level.
- Avoid weapon design, targeting, operational deployment, or evasion details.

Future read-only evidence gaps:
- Create a current map of major arms-control agreements and which are active, expired, suspended, or under negotiation.
- Summarize evidence for nuclear risk-reduction interventions: hotlines, de-alerting, no-first-use policies, verification, and crisis communication.
- Identify current expert disagreement areas and label them clearly.

### 5. Civilizational resilience and incident preparedness

Primary/source-of-record candidates:
- Emergency-management agency guidance, critical-infrastructure resilience documents, official continuity-of-operations guidance, public health emergency plans, and standards such as ISO business continuity materials where publicly summarized. [PRIMARY]
- Official after-action reports from disasters, cyber incidents, pandemics, supply-chain disruptions, and infrastructure failures. [PRIMARY]

Research and synthesis candidates:
- Academic disaster-risk reduction, resilience engineering, high-reliability organization, supply-chain resilience, and crisis-communication literature. [PEER_REVIEWED]
- Expert syntheses from OECD, World Bank, UNDRR, national academies, insurance/reinsurance research, and infrastructure resilience institutes. [EXPERT_SYNTHESIS]/[RESEARCH_REPORT]
- Incident databases and lessons-learned repositories, used defensively. [PRIMARY]/[MEDIA]/[RESEARCH_REPORT]

Future read-only evidence gaps:
- Build a cross-domain incident-preparedness checklist that links AI, bio, cyber, nuclear, and infrastructure incidents without operational harm.
- Identify reliable after-action report repositories and extract recurring preparedness lessons.
- Evaluate which resilience interventions are robust across many risks versus domain-specific.

### 6. Forecasting, prioritization, and meta-research infrastructure

Primary/source-of-record candidates:
- Forecasting-platform question pages and resolution criteria from Metaculus, Good Judgment Open, Manifold, prediction markets where legal/public, and official expert-elicitation reports. [FORECAST]/[PRIMARY]
- Grantmaker/open-philanthropy style cause-prioritization reports where public. [EXPERT_SYNTHESIS]/[RESEARCH_REPORT]
- Public datasets and benchmark repositories with clear documentation and licenses. [PRIMARY]

Research and synthesis candidates:
- Forecasting research literature on calibration, aggregation, base rates, expert elicitation, and tournament design. [PEER_REVIEWED]
- Cause-prioritization analyses from credible philanthropy/research groups, with careful attention to assumptions and value judgments. [EXPERT_SYNTHESIS]
- Bibliographies, evidence maps, living reviews, and standards for evidence grading. [EXPERT_SYNTHESIS]

Future read-only evidence gaps:
- Define a lightweight calibration log for this loop's own forecasts and assumptions.
- Build a source freshness tracker: source name, last checked date, scope, evidence label, and known limitations.
- Identify which forecasts materially change artifact priorities and should be revisited.

## Cross-domain source evaluation checklist

For every source used in future artifacts, record:
- Citation or stable locator:
- Date published and date checked:
- Author/institution:
- Domain and claim supported:
- Evidence label(s): [PRIMARY], [PEER_REVIEWED], [RESEARCH_REPORT], [EXPERT_SYNTHESIS], [FORECAST], [MEDIA], [ASSUMPTION]
- Confidence: high / medium / low / unknown
- Potential bias or incentive:
- Relevance to x-risk reduction:
- Safety/dual-use concerns:
- What would change if this source were wrong or outdated?
- Follow-up needed:

## Recommended workflow for future read-only research turns

1. Start from the claim or decision need, not from an interesting source.
2. Seek a primary source first; if unavailable, use a strong research report or expert synthesis.
3. Cross-check important claims with at least one independent source.
4. Mark all forecasts and assumptions explicitly; do not bury them as facts.
5. Prefer recent official versions for fast-moving policy/standards claims.
6. Keep dangerous dual-use material non-operational and defensive.
7. Save source notes locally; do not contact authors or submit feedback without approval.

## Highest-priority missing evidence for later workers

1. Current official AI safety/evaluation/governance frameworks and their latest publication dates.
2. Annotated bibliography for dangerous-capability evaluation governance and responsible disclosure/reporting.
3. Current map of AI incident databases and their inclusion criteria.
4. Current official biosecurity governance and pandemic-preparedness sources, summarized non-operationally.
5. Current nuclear arms-control/status map from official and expert-synthesis sources.
6. Cross-domain resilience after-action report repository list.
7. Forecasting/prioritization source tracker with checked dates and explicit uncertainty.

Acceptance check:
- Covers AI safety/governance, biosecurity, nuclear risk, resilience, and forecasting.
- Defines required labels: primary source, peer-reviewed/research report, expert synthesis, forecast/market, media, assumption.
- Flags missing evidence for future read-only research.
- Contains no outreach, posting, account use, remote writes, or harmful operational instructions.
