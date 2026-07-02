# Turn 18 Source-Verification Packet for AI Governance/Evals

Date: 2026-07-02
Status: local preparation artifact only; no claims verified this turn
Purpose: make the next browsing-enabled P1 pass faster and safer by converting the existing evidence log into a concrete, bounded verification packet.

## Scope and safety posture

This packet supports read-only public verification of source-needed claims in:

- `ai_governance_framework_mini_brief_v0.md`
- `dangerous_capability_eval_governance_checklist_v0.md`
- `ai_governance_framework_evidence_log_v0.md`

No outreach, posting, form submission, account/API write, purchase, remote modification, or contact with source authors is authorized. Use only public/read-only sources. Do not collect sensitive information. Do not reproduce dangerous evaluation prompts, exploit methods, cyber-offensive procedures, bio/chemical/weapon details, or evasion content.

## Deliverable for the next browsing-enabled worker

Create or update:

- `/home/vi/xriskdoominningbs/.xrisk_loop/artifacts/ai_governance_framework_source_verification_v0.md`

Minimum output fields for each verified source:

| Field | Required content |
|---|---|
| Source ID | Stable local ID, e.g. `SRC-NIST-AIRMF-001` |
| Organization | Source publisher or authoring organization |
| Exact title | Exact public document/page title as shown by the source |
| URL/citation | Canonical URL or citation inspected |
| Publication/version date | Date/version on the source, or `not found on page` if absent |
| Access date | Date the worker inspected it |
| Source type | Primary official page, primary policy document, technical standard/guidance, research report, or other |
| Relevant support | Short non-operational paraphrase of what the source supports |
| Claims supported | Evidence-log IDs, e.g. GOV-E-001, GOV-E-004 |
| Claims not supported | Any local claim the source does not actually support |
| Confidence | Verified-current, partially supported, stale/unclear, or not supported |
| Safety note | Confirmation that the extracted content stays governance-level and non-operational |

## Priority source targets

### Tier 1 — NIST / US AISI source-of-record checks

Evidence-log IDs: GOV-E-001, GOV-E-002, GOV-E-003, GOV-E-009

Questions to answer:

1. What is the current exact title, version, and date of the NIST AI Risk Management Framework material?
2. What functions/categories does the NIST AI RMF define, and can they be safely paraphrased at a governance-process level?
3. Are there current NIST or U.S. AI Safety Institute documents related to generative/frontier AI governance or evaluation guidance? If yes, what are their exact titles, dates, and status?
4. Does any source explicitly say it is voluntary, non-binding, guidance, a profile, or otherwise limited in legal force?

Search/source strategy:

- Start with the official NIST AI RMF page already listed in the evidence log.
- Prefer official NIST or U.S. AI Safety Institute pages over secondary summaries.
- Record exact document titles and dates; do not infer legal effect.

### Tier 2 — Frontier-lab preparedness / responsible-scaling / frontier-safety frameworks

Evidence-log IDs: GOV-E-004, GOV-E-010, GOV-E-011

Questions to answer:

1. For at least two public lab frameworks, what are the exact current document titles, versions/dates, and URLs?
2. What high-level governance dimensions do they describe: trigger/risk categories, decision authority, review cadence, deployment/release gates, disclosure controls, oversight/audit, monitoring, and update process?
3. Are the frameworks presented as voluntary organizational policies, external commitments, legal obligations, or something else?
4. Does the local risk-tier table in `dangerous_capability_eval_governance_checklist_v0.md` need relabeling to avoid implying consensus or standardization?

Candidate organizations from the evidence log:

- Anthropic Responsible Scaling Policy or successor public policy.
- OpenAI Preparedness Framework or successor public policy.
- Google DeepMind Frontier Safety Framework or successor public policy.

Search/source strategy:

- Use official organization pages or PDFs first.
- If an organization has a newer successor framework, cite the newer one and note that older local references may be stale.
- Extract only governance structure. Do not quote or summarize dangerous eval tasks, prompts, thresholds in operational detail, capability-enabling methods, or evasion-relevant material.

### Tier 3 — Authorization, scope control, evidence handling, and tiered disclosure

Evidence-log IDs: GOV-E-006, GOV-E-008

Questions to answer:

1. Which public sources recommend authorization, scoping, evidence handling, stop conditions, or controlled disclosure for high-risk AI evaluations/red-teaming?
2. Which public sources support tiered disclosure or controlled publication of dual-use AI evaluation results?
3. What limits do those sources place on public reporting of sensitive methods, raw evidence, vulnerabilities, or dual-use results?

Search/source strategy:

- Prefer official standards, safety institute guidance, lab policies, or widely cited governance reports.
- If using general vulnerability disclosure analogies, label them as analogy rather than direct AI-evaluation evidence.
- Keep all extracted material at the policy/governance level.

### Tier 4 — Independent review/audit and institutional roles

Evidence-log IDs: GOV-E-007, GOV-E-009

Questions to answer:

1. What credible public sources discuss benefits and limits of independent audits/reviews for high-stakes AI systems?
2. What do current AI safety institutes or standards bodies say about evaluation, convening, testing, standards, or guidance roles?
3. Which claims remain too broad or unsupported after checking primary sources?

Search/source strategy:

- Use official institute/standards-body pages for institutional roles.
- Use research or policy reports only when clearly labeled as research/synthesis rather than source-of-record authority.

## Claim-upgrade rules

- Upgrade to `Verified-current / primary` only when a current official source directly supports the claim, with title, URL/citation, date/version, and access date recorded.
- Use `Partially supported` when a source supports the general direction but not the exact local claim.
- Use `Analytical judgment, source-informed` when the worker is mapping a verified framework to a local governance recommendation.
- Use `Not supported` or `No source found in this pass` rather than stretching evidence.
- Preserve `source-needed` for legal, regulatory, compliance, or current-policy claims unless a primary legal or official source directly supports them.

## Red flags requiring caution or patching

Patch or flag the relevant local artifact if source verification finds any of the following:

- A local artifact names an outdated framework or organization.
- A voluntary framework is described as binding or legally required.
- A local risk-tier or governance-gate table appears to be presented as a standard rather than a local placeholder.
- NIST AI RMF language is used as if it were designed specifically for dangerous-capability evaluation oversight without source support.
- Disclosure guidance could be read as permission for uncontrolled public release of sensitive evaluation details.
- A claim implies evidence of x-risk reduction effectiveness when only process/auditability support exists.

## Patch targets after verification

If sources are verified, update in this order:

1. `ai_governance_framework_source_verification_v0.md` — canonical record of checked sources.
2. `ai_governance_framework_evidence_log_v0.md` — claim statuses and confidence labels.
3. `ai_governance_framework_mini_brief_v0.md` — only narrowly patch verified citations/claims.
4. `dangerous_capability_eval_governance_checklist_v0.md` — relabel any placeholder tiering or gates if needed.
5. `artifact_index_and_usage_guide_v0.md` — update readiness status.

## Acceptance checklist for the browsing-enabled pass

- [ ] NIST AI RMF-related document names, dates/versions, URLs, and access date recorded.
- [ ] At least two public lab preparedness/responsible-scaling/frontier-safety frameworks checked from official sources.
- [ ] Each extracted claim has source type, confidence, support scope, and safety note.
- [ ] Legal/current-policy claims remain dated and calibrated.
- [ ] No dangerous operational detail is copied into local artifacts.
- [ ] No outreach, posting, form submission, account use, remote write, or public disclosure occurs.

## This-turn acceptance check

- Converted the existing evidence log into a concrete source-verification packet.
- Did not verify or upgrade any external factual claim.
- Did not take or recommend any external action.
- Kept the artifact focused on governance-level, non-operational source verification.
