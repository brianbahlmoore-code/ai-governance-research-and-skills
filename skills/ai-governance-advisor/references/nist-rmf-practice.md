# NIST AI RMF profile workshop

Baseline: AI RMF 1.0 (January 2023), with an update in progress at 2026-10-23. The [official Core](https://airc.nist.gov/airmf-resources/airmf/5-sec-core/) contains the complete category/subcategory text. The [Playbook](https://airc.nist.gov/airmf-resources/playbook/) offers optional suggestions. The workshop prompts below are original implementation examples; they do not restate every subcategory or impose additional NIST requirements.

## Category index

Concise navigation labels, not official titles:

| Function | Category themes |
|---|---|
| GOVERN | 1 policies/processes; 2 accountability; 3 diverse participation and human roles; 4 risk culture; 5 engagement; 6 third parties |
| MAP | 1 context; 2 system categorization; 3 capabilities/benefits/costs; 4 components; 5 impacts |
| MEASURE | 1 methods; 2 trustworthiness evaluation; 3 ongoing tracking; 4 feedback on measurement |
| MANAGE | 1 prioritization/treatment; 2 benefit and harm strategies; 3 suppliers; 4 response/monitoring |

Governance spans the other functions; iteration is expected. Use the actual source identifiers for a formal profile and record why outcomes are selected. A partial profile can be useful if its boundaries are explicit; it must not be described as full framework coverage.

## Original workshop prompts and artifacts

### GOVERN

G1 workshop: bring a real use-case intake to the policy owner. Can the owner determine applicable review depth, decision rights, review timing and retirement responsibility without asking the policy author? Artifact: a worked decision trace and any policy ambiguity.

G2 workshop: simulate a serious harmful output during an executive's absence. Who has authority and capacity to intervene? Artifact: responsibility matrix, escalation path and observed response gap.

G3 workshop: ask a domain expert, operator and affected-person representative to identify different failure modes. Test the proposed human-review interface with realistic workload. Artifact: perspective gaps and oversight usability findings.

G4 workshop: examine whether someone can challenge an optimistic launch claim without being dismissed. Compare recorded risk decisions with actual incentives. Artifact: documented challenge and resulting action, not a culture score invented from policy wording.

G5 workshop: choose one substantive complaint and trace whether it changed evaluation, design or communication. Artifact: feedback disposition and evidence of closure.

G6 workshop: inspect a model-provider outage or policy change scenario. Artifact: dependency map, contract gaps, fallback and decision owner.

### MAP

M1 workshop: have two reviewers independently describe purpose, affected people and deployment boundary. Resolve differences before selecting metrics. Artifact: agreed context and assumptions register.

M2 workshop: diagram how inputs become outputs/actions, including retrieval and tools. Artifact: architecture and knowledge-boundary description understandable to the operating team.

M3 workshop: compare the AI option against a simpler alternative using the same benefits, errors and operating costs. Artifact: justified selection and limitations; distinguish speculative benefit from demonstrated value.

M4 workshop: follow one sensitive record through supplier, retrieval, logging and downstream action. Artifact: component-level risk and responsibility map with evidence gaps.

M5 workshop: interview a plausible affected non-user and examine reversibility and access to remedy. Artifact: impact scenarios, missing stakeholder evidence and updated requirements.

### MEASURE

ME1 workshop: ask which measurement would change the release decision. Remove metrics that cannot inform any action, while retaining diagnostic metrics when justified. Artifact: metric rationale, threshold, sampling and limitations.

ME2 workshop: test the exact deployment configuration against realistic tasks, adverse inputs, subgroup harms, safety, security, privacy and oversight questions. Artifact: reproducible test records, uncertainty and unresolved concerns. Do not substitute one aggregate score for all dimensions.

ME3 workshop: introduce a simulated population shift or a previously unseen failure. Artifact: demonstrated detection or a documented blind spot and compensating review.

ME4 workshop: compare evaluation results with real user/affected-person reports. Investigate disagreement rather than assuming either data source is complete. Artifact: changes to tests and thresholds with rationale.

### MANAGE

MA1 workshop: rank material scenarios using the approved method and explain the first funded treatment. Artifact: residual-risk decision with authority and conditions; do not hide severe harms in an average.

MA2 workshop: rehearse restriction, fallback and recovery. Artifact: evidence that the system can be disengaged without creating a larger uncontrolled problem.

MA3 workshop: simulate a provider model replacement and assess continued fitness. Artifact: supplier notice, regression evidence and scoped decision.

MA4 workshop: walk through detection, investigation, affected-person communication, remediation and restart. Artifact: incident exercise results and corrective-action effectiveness.

## Profile record

For each selected official outcome keep: source/version; use-case applicability; current evidence; evidence confidence; target outcome; gap; action/owner; acceptance test; due date; review trigger. Include rationale for not selecting an outcome, especially where another process covers it.

Separate current state from target state. Do not describe an intended contract change or planned test as an implemented control. Keep program-level controls linked to relevant system-level evidence. For a portfolio profile, investigate common dependencies and correlated failures across systems.

## Demonstration

For a policy assistant, G6/M4/MA3 prompt investigation of upstream model changes; M1/M5 establish that employees may rely on answers for employment decisions; ME1/ME2 establish task tests and authority boundaries; MA2/MA4 establish escalation and fallback. If the assistant later gains transaction tools, reopen context, impacts, evaluation and treatment. Prior assessment of text-only behavior is not adequate evidence for the expanded authority.
