# Evidence Log Template for AI Governance / Dangerous-Capability Evaluation Work v0

Purpose: provide a lightweight, auditable way to track claims, sources, confidence, missing evidence, and safety constraints for future x-risk reduction artifacts. This is a local documentation template only; it does not authorize outreach, testing, account use, submissions, or other external side effects.

## When to use
Use this log when creating or updating:
- AI governance mini-briefs.
- Dangerous-capability evaluation governance checklists.
- Incident preparedness guidance.
- Source verification notes from public/read-only research.
- Any artifact containing factual or policy-relevant claims that may become stale.

## Evidence labels
Use the labels from `source_map_and_evidence_rubric_v0.md`:
- Primary source: official document, law/regulation text, standards document, organization policy/framework, or direct dataset.
- Peer-reviewed / research report: academic paper, technical report, or institutional research report.
- Expert synthesis: reputable expert summary, review, or consensus-style analysis.
- Forecast / market: prediction platform, scenario analysis, or structured forecast.
- Media: journalism, press release, or public commentary.
- Assumption / source-needed: plausible but unverified claim that must not be treated as established.

Confidence tags:
- High: directly supported by reliable current source and low ambiguity.
- Medium: supported but interpretation, scope, or freshness has uncertainty.
- Low: weak, indirect, stale, or contested evidence.
- Source-needed: not yet verified.

## Master evidence log table

| ID | Claim or decision-relevant statement | Artifact/section affected | Evidence label | Source name | URL/path | Publication or access date | Quoted/paraphrased support | Confidence | Freshness risk | Safety/compliance notes | Needed follow-up |
|---|---|---|---|---|---|---|---|---|---|---|---|
| E-001 | [Short claim] | [File + section] | [Primary / Research / Expert synthesis / Forecast / Media / Assumption] | [Source] | [URL or local path] | [YYYY-MM-DD] | [Short non-operational quote or paraphrase] | [High/Medium/Low/Source-needed] | [Low/Medium/High] | [No harmful operational detail; no external action] | [Verify/update/replace/remove] |

## Source verification checklist
For each important claim, record:
1. Source identity: Who published it? Is it the source of record or a secondary description?
2. Version/date: What version, publication date, effective date, or access date applies?
3. Scope: What exactly does the source cover and not cover?
4. Claim support: Which sentence, section, table, or page supports the claim?
5. Interpretation: Is the artifact making a direct factual claim or an analytical judgment?
6. Freshness: How likely is the claim to go stale in 3, 6, or 12 months?
7. Conflict check: Do other credible sources disagree or frame it differently?
8. Safety check: Does citing or summarizing the source risk spreading harmful operational details?
9. Approval check: Would any proposed next step require human approval because it creates external effects?

## Claim status workflow

### Status: source-needed
Use when a claim is plausible but not verified. Required handling:
- Mark clearly as `source-needed` or `assumption`.
- Avoid using it as the sole basis for recommendations.
- Add a follow-up item naming likely public sources to verify.

### Status: verified-current
Use when a claim is supported by a primary or strong research source checked this run. Required handling:
- Include publication/access date.
- Include source name and exact section/title if available.
- Keep paraphrase non-operational and proportionate.

### Status: verified-but-stale-risk
Use when a claim is supported but may change quickly, e.g. law, standards, frontier-lab frameworks, model capability thresholds, or incident reporting mechanisms. Required handling:
- Include explicit review-by date or freshness warning.
- Avoid categorical claims like “currently requires” unless dated.

### Status: deprecated/replaced
Use when a source or claim has been superseded. Required handling:
- Do not delete silently; note replacement source if known.
- Update affected artifact sections.

## Review cadence suggestion
- High-stakes governance/current-policy claims: review every 1-3 months or before external use.
- Standards/framework descriptions: review every 3-6 months.
- General conceptual claims: review every 6-12 months.
- Any claim marked source-needed: prioritize in next browsing-enabled worker turn.

## Safety guardrails for evidence logging
- Do not include procedural details that enable cyber offense, weapons development, biological/chemical harm, evasion of safeguards, or unauthorized testing.
- Do not log private, personal, confidential, or credential-like information.
- Do not contact source authors, submit forms, open issues, post, or use accounts unless the user explicitly approved that exact action.
- If a useful source contains harmful operational detail, cite only the non-sensitive governance or safety-relevant high-level point.
- If an artifact recommends outreach, publication, submission, account use, or other external effects, move it to `proposals.md` for human review instead of executing.

## Example entries

| ID | Claim or decision-relevant statement | Artifact/section affected | Evidence label | Source name | URL/path | Publication or access date | Quoted/paraphrased support | Confidence | Freshness risk | Safety/compliance notes | Needed follow-up |
|---|---|---|---|---|---|---|---|---|---|---|---|
| E-EX1 | NIST AI RMF-style processes can structure risk identification, measurement, management, and governance for AI systems. | ai_governance_framework_mini_brief_v0.md / governance landscape | Source-needed until verified | NIST AI RMF candidate source | https://www.nist.gov/itl/ai-risk-management-framework | Access date needed | Verify exact RMF functions and wording from primary source. | Source-needed | Medium | Non-operational governance summary only. | Browsing-enabled worker should verify current version/date. |
| E-EX2 | Frontier-lab preparedness or responsible-scaling frameworks may provide examples of capability-triggered governance gates. | dangerous_capability_eval_governance_checklist_v0.md / deployment gates | Source-needed until verified | Candidate lab frameworks | [URLs needed] | Access date needed | Verify at least two public lab frameworks before treating as evidence. | Source-needed | High | Avoid reproducing dangerous eval methods; summarize only governance gates. | Browsing-enabled worker should collect primary-source citations. |

## Acceptance checks for a completed evidence log
- Every major factual claim has a row or an explicit reason it is low-stakes/background.
- No source-needed claim is presented as established fact.
- Current-policy and current-framework claims include date/version/access date.
- High-impact recommendations cite at least one primary or strong research source, or are clearly marked provisional.
- Safety/compliance column confirms that no harmful operational detail or unauthorized external action is included.
