# Concepts for applied governance

Original teaching notes; examples are illustrative. Use current primary sources for legal or standard-specific claims.

## AI and deployment vocabulary

AI system: the operational arrangement producing predictions, recommendations, content or actions. Model: a component encoding learned relationships. Machine learning: deriving behavior from data. Deep learning: machine learning using layered neural networks. Generative AI: producing new outputs rather than only selecting a category or score. Agent: a system using models and tools to pursue tasks over one or more steps; its authority matters as much as its intelligence.

Supervised learning uses labeled examples; unsupervised methods discover patterns; reinforcement learning uses feedback about actions. These are learning approaches, not risk tiers. Training changes model parameters. Inference applies a model. Fine-tuning further changes parameters. RAG retrieves external material at runtime. Prompting changes instructions/context without necessarily updating model parameters. RAG does not guarantee truth or access control.

Open weights describe access to model parameters; open-source status depends on license and other conditions. On-premises deployment changes who operates controls, not whether governance is needed. Multimodal systems process or generate several types of information, adding cross-modal privacy, integrity and evaluation issues.

## Data and evaluation

Training data fits the model; validation data guides development choices; a held-out test assesses final behavior. Repeatedly tuning to the test set weakens its independence. Leakage can be temporal, label-based, duplicate-record or other contamination that makes evaluation unrealistically easy.

Representativeness asks whether evaluation covers deployment conditions and people. Ground truth can itself be uncertain or biased. Data quality concerns suitability for purpose, not just completeness. Data drift is a change in inputs; concept drift concerns changes in relationships between inputs and target outcomes. Monitoring one does not completely detect the other.

For binary classification: precision asks how many predicted positives are correct; recall asks how many actual positives were found; false-positive and false-negative rates concern different errors. Accuracy can mislead when classes are imbalanced. Choose metrics based on the cost and distribution of errors, with appropriate denominators and uncertainty.

Calibration concerns whether stated probabilities match observed frequencies. A confident tone is not calibrated uncertainty. An explanation that sounds plausible can be unfaithful to the model's actual basis. Separate explanations useful to a developer from explanations useful to an affected person seeking recourse.

## Fairness and human impacts

Demographic parity compares selection rates. Equalized odds compares error behavior conditional on actual outcomes. Calibration compares probability meaning. These criteria can conflict, particularly when group outcome rates differ. Select criteria using the actual harm, law, data quality and stakeholder context; do not prescribe a universal metric for all hiring or lending systems.

Bias can enter through historical decisions, sampling, measurement, labels, features, model objectives and deployment. Removing a protected attribute can leave proxy effects and can also make evaluation harder. Collecting data for fairness evaluation may create additional privacy obligations. Evaluate intersectional and accessibility concerns where relevant, while acknowledging small-sample limits.

Automation bias is over-reliance on system output. Algorithmic aversion is excessive rejection of useful assistance. Oversight design should enable appropriate reliance, not merely maximize acceptance or override rates. Human-in-the-loop is a description of arrangement, not proof of effective control.

## Risk and assurance distinctions

Inherent risk is exposure before the assessed controls; residual risk remains after their demonstrated effect. Risk appetite is the organization's broad willingness to take risk; tolerance operationalizes boundaries. Confidence concerns evidence quality and must not be confused with low risk.

Impact assessment asks who is affected and how; risk assessment evaluates uncertain scenarios and treatment; audit evaluates evidence against criteria. Model validation evaluates fitness and limitations. Security testing does not prove fairness; a policy does not prove implementation; a certificate does not establish suitability for every use case.

Preventive controls reduce occurrence, detective controls reveal problems and corrective controls limit/recover from consequences. A warning may be appropriate but is often weak against severe irreversible harm. Prefer concrete interventions with testable mechanisms.

## GenAI and agents

Confabulation is plausible output that is wrong or unsupported. Prompt injection uses untrusted content to steer behavior outside intended authority. Data/model poisoning changes material the system learns from or relies on. Sensitive-data leakage can occur through prompts, retrieval, outputs, logs or memorized information. Excessive agency combines capability with broader authority than needed.

Agent control should include independent permissions, bounded actions, stopping conditions, review for consequential actions and recovery. Logging should support investigation while minimizing unnecessary personal data. A system prompt is not an access-control boundary, and an instruction to 'be safe' is not an adequate security control.

## Frequent reasoning traps

- 'NIST aligned' is not a NIST-issued certification.
- AIGP is personal competency; ISO 42001 concerns a scoped organizational management system.
- No-training terms do not imply zero retention, no human review or complete deletion.
- Publicly available data does not automatically mean unrestricted lawful reuse.
- Aggregate performance does not establish subgroup performance.
- Human approval does not guarantee meaningful oversight.
- A high internal tier does not automatically establish a statutory high-risk classification.
- A crosswalk does not prove equivalence; each obligation can retain unmapped conditions.
- A new model version or use may invalidate prior evidence even when the supplier name stays the same.
