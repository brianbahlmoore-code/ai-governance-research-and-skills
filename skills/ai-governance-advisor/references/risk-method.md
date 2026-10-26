# AI risk and impact assessment method

Use NIST AI RMF as the outcome framework and ISO 23894/42005 as relevant guidance families. The scales, gates and templates here are original enterprise suggestions, not official framework scoring rules. Read [sources.md](sources.md) for source status.

## Separate the assessment objects

- Model: learned component and version.
- System: model plus data, retrieval, prompts, user interface, rules, people, tools and infrastructure.
- Use case: a specific decision or activity in a real organizational and social setting.
- Impact assessment: who may benefit or be harmed, how, and with what opportunity for participation and remedy.
- Risk assessment: scenarios, likelihood/uncertainty, consequences, controls and residual exposure.
- Legal assessment: whether a defined actor, activity, territory and date trigger an obligation.

A general model benchmark cannot establish fitness for a new workflow. A supplier's assurance report cannot establish the customer's configuration is safe. Privacy, equality, safety, security and model performance can fail independently.

## Define the context and counterfactual

Document the intended outcome, affected people, vulnerable groups, decision authority, data flow, deployment conditions, scale and error consequences. Compare the system with a feasible non-AI or existing-process baseline. Ask whether the benefit requires AI at all and whether a narrower application delivers most benefits with less harm.

Include indirect users and non-users: rejected applicants, people described in documents, employees monitored by the system and communities exposed to aggregate effects. Document consultation performed, missing perspectives and accessible routes for challenge.

## Write specific harm scenarios

Use: because of [cause], under [conditions], [system behavior] may cause [consequence] to [affected party]. Identify the component, lifecycle stage and evidence supporting plausibility.

Weak: 'Bias risk is high.' Better: 'The screening model was validated only on historical successful applicants; applying it to a new region may disproportionately reject qualified local applicants, who have no effective appeal.' The better formulation identifies evaluation, data and recourse needs.

Cover validity, reliability, safety, security, privacy, harmful bias, transparency, interpretability, accountability, misuse, accessibility, environmental costs and supply-chain dependency where relevant. Do not mechanically include every category when the use case cannot reasonably expose it.

## Assess inherent exposure and uncertainty

Use the organization's approved method if available. Otherwise propose a qualitative rubric and obtain adoption through the organization's ordinary decision process:

| Severity | Illustrative anchor |
|---|---|
| Limited | Easily corrected inconvenience with little consequential impact |
| Material | Meaningful loss, exclusion or operational disruption with feasible remedy |
| Severe | Significant rights, financial, health or safety harm; difficult remediation |
| Critical | Life-threatening, systemic or widespread harm with limited reversibility |

Likelihood should refer to a stated period and exposure: unlikely, plausible, likely or observed. Explain supporting evidence. Record confidence separately: strong, partial or weak. Unknown probability does not mean low risk. Low-frequency catastrophic harm warrants explicit escalation rather than being averaged away in a matrix.

If a numerical matrix is requested, label ordinal multiplication as a prioritization convention, not measured probability. Do not use an unexplained percentage reduction to convert inherent into residual risk. Evaluate what each control actually changes in the causal scenario.

## Design controls and evaluations together

For each material scenario identify preventive, detective and corrective controls. Prefer eliminating an unnecessary harmful function, narrowing authority or limiting deployment before relying solely on user warnings. Define owner, mechanism, evidence, test, failure response and dependencies.

| Question | Practical evaluation design |
|---|---|
| Does it work for the intended task? | Representative held-out tasks, defensible ground truth, baseline and error analysis |
| Does performance differ materially between affected groups? | Justified subgroup analysis, sample sizes, uncertainty, failure costs and privacy safeguards |
| Does it remain reliable outside ideal inputs? | Distribution shift, missing inputs, edge cases and stress conditions |
| Can humans meaningfully oversee it? | Reviewer comprehension, intervention time, workload, authority and fallback exercises |
| Can hostile content cause unauthorized action? | Scoped adversarial tests of trust boundaries and tool permissions |
| Can the provider change the risk without warning? | Contract review, version tracking and change-triggered regression |

Select fairness criteria based on the harm and context; no single metric is universally correct. Demographic parity, error-rate parity and calibration answer different questions and can conflict. An overall accuracy score can hide severe group-level failures. Include uncertain estimates for small populations, and do not invent sample sufficiency.

For generative outputs, measure task validity, unsupported statements, harmful outputs, disclosure effectiveness and escalation behavior. Evaluate the full application, not only the foundation model. Use expert review when automated graders cannot reliably determine correctness. Document limitations of the graders themselves.

## Evidence states

Classify each assertion as observed evidence, third-party attestation, vendor claim, assumption, missing or contradicted. Record artifact ID, issuer, scope, version, period, method and limitations. A policy can support control design but cannot by itself prove operation. A certificate outside the assessed service scope may add no meaningful assurance.

## Residual risk and disposition

After testing controls, reassess plausible residual harms and remaining uncertainty. Specify the acceptance authority and rationale. Suggested dispositions:

- Proceed: material evidence supports intended deployment within tolerance.
- Proceed with conditions: enforceable limitations and tracked closure evidence address bounded gaps.
- Restricted pilot: limited data, users and authority; defined evaluation objective and stop rules.
- Hold: missing evidence or unresolved material concerns prevent a defensible decision.
- Stop: use is prohibited in the applicable context, violates a binding constraint or exceeds tolerance without feasible treatment.

These recommendations do not replace the accountable person's decision. Missing critical evidence can justify a hold without pretending the adverse outcome is certain.

## Continuous review

Define metric, baseline, threshold, sampling interval, owner and response for each monitored risk. Reassess on material changes to model, prompts, retrieval corpus, data rights, population, geography, tool permissions, suppliers, contracts or intended purpose. Include complaints and near misses, not just technical outages.

For an incident preserve necessary evidence proportionately, contain the harmful capability, establish affected parties and severity, apply the relevant notification process, investigate causes, test remediation and obtain authorization for restart. Avoid logging unnecessary personal data merely to create an audit trail.

## Worked example: employee policy assistant

Intended use is answering internal policy questions using approved documents. It must not decide disciplinary action or send messages as employees. Main scenarios: obsolete retrieval produces incorrect advice; employee documents disclose sensitive information across groups; injected document text induces an unauthorized tool call; an unannounced model update changes refusal behavior.

Suggested controls: document-level authorization applied before retrieval; versioned policy corpus; source-grounded responses with escalation for unresolved questions; tool access disabled for the initial release; representative tests covering permissions and stale documents; vendor no-training terms and change notifications.

Illustrative disposition: restricted pilot until access-boundary tests and policy-owner review are complete. This is a demonstration of reasoning, not a completed assessment or evidence about a real supplier.
