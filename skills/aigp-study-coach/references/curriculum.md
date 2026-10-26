# Complete competency coverage: original learning curriculum

Aligned to the user's supplied AIGP BoK v2.1 and the checked official blueprint. This is original explanatory coverage, not a replacement copy of the BoK or paid course. [coverage-map.csv](../assets/coverage-map.csv) maps every one of the 58 study objectives; use it to track gaps.

## I.A — AI concepts, harms and responsible principles

Understand the difference between a model, an AI system and a business use. Distinguish classification, regression, recommendation, generation and agents acting through tools. Explain why probabilistic behavior, opaque learned relationships, scale, changing data and delegated authority complicate governance. Traditional software controls remain useful but do not fully evaluate learned behavior or societal effects.

Analyze consequences for the enterprise and for affected people separately. Harm can arise despite technically accurate output, such as an intrusive surveillance use. Translate fairness, safety, privacy, security, transparency and accountability into observable outcomes. Explain the tradeoff when making a system more transparent risks exposing sensitive data. Exercise: compare a spelling assistant with an automated employment ranking system and justify different review depth.

## I.B — Accountability and organizational expectations

Assign responsibilities across business, engineering, data, security, privacy, legal, procurement, risk and assurance. A committee does not replace an accountable business owner. Distinguish the roles of organizations building models, supplying systems, deploying them and using their outputs; one organization can perform several roles.

Design collaboration that brings domain knowledge and affected-party perspectives into decisions. Training must match actual duties: executives set appetite, developers evaluate, procurement checks terms, and users recognize limitations and escalation routes. Governance should scale with the organization's resources and impact, rather than treating every use as a board matter. Exercise: create decision rights for a vendor model update and explain who can suspend use.

## I.C — Lifecycle policies and third parties

Connect intake, development/acquisition, data, validation, release, operation, incident management and retirement. Reuse privacy, security, IP, HR and procurement policies while addressing AI-specific gaps. Policy should specify who decides, which evidence is needed and what happens when conditions change.

Third-party risk remains with the enterprise even when technical work is outsourced. Contracts, supplier assessments and acceptable-use rules must align with actual configuration and purpose. Exercise: identify why a no-training promise alone fails to address retention, human review, subcontractors or harmful outputs.

## II.A — Privacy law and AI

Reason about lawful processing, notice, choice, purpose limitations and minimization. Determine whether a training purpose differs from the purpose for which data was collected. Privacy by design concerns architecture and defaults, not merely a notice appended before launch.

Understand organizational roles, processor arrangements, transfers, rights requests, records, impact assessments and incident obligations. Sensitive data, biometric uses and consequential automated decisions need separate trigger analysis. Do not assume publicly accessible information has unrestricted reuse rights, pseudonymized data is anonymous, or a nominal reviewer resolves automated-decision concerns. Exercise: map prompts, outputs, logs, embeddings and feedback through a cloud assistant and identify unanswered legal questions.

## II.B — Existing non-AI laws

Examine rights in training material, software, model artifacts and generated outputs without assuming they are interchangeable. Contractual output ownership cannot create rights the supplier does not possess. Evaluate nondiscrimination obligations in consequential settings and understand why removing protected attributes may leave proxies.

Consumer protection can be implicated by unsupported capability claims, deceptive interfaces or misleading outputs. Product liability can concern design, warnings and failures in integrated products. The governing jurisdiction and facts determine the actual rule; do not memorize one global liability answer. Exercise: separate an unsupported 'bias-free' marketing claim from a proven disparate-outcome finding and identify the evidence needed for each.

## II.C — AI-specific law

Learn to establish territorial scope, actor, use and date before categorization. For the EU approach, distinguish prohibited practices, high-risk systems, transparency duties and general-purpose-model obligations; these are not interchangeable labels. Understand why risk management, data governance, documentation, conformity/impact processes, quality management, oversight and records become relevant.

Study enforcement and potential penalties through current official materials rather than memorizing stale amounts. Compare provider, deployer, importer and distributor responsibilities. The current syllabus explicitly includes South Korea and relevant US AI laws; study the core approach and refresh details for the exam date. Exercise: analyze a company that materially changes a purchased system's purpose and identify how responsibilities may change. Keep current law separate from confirmed exam coverage.

## II.D — Standards, frameworks and tools

Explain OECD principles, NIST's four functions and how categories/subcategories support a chosen risk profile. GOVERN applies throughout; the Playbook is optional guidance. Know that ISO 22989 supports vocabulary, ISO 42001 addresses a management system and ISO 42005 addresses system impacts. ISO 23894 is a useful operational extension for risk management.

The key exam skill is choosing the appropriate instrument for the problem. A certificate, a voluntary framework, a legal obligation and a competency credential provide different kinds of assurance. Exercise: explain why aligning one control to three frameworks does not prove compliance with three entire frameworks.

## III.A — Govern design and construction

Start with the business problem, alternatives, affected people and success criteria. Perform impact analysis early enough to change the design. Select architecture and models based on purpose, constraints, risks and evidence, not benchmark reputation alone.

Define human oversight and evaluation thresholds before release. Consider stakeholder input, operational controls and the hierarchy of risk treatments: removing a harmful feature may be more reliable than warning users. Document assumptions, design decisions and limitations. Exercise: decide whether an agent needs write access to complete a task and compare a narrower design.

## III.B — Govern training and testing data

Establish rights, provenance, quality, relevance and representativeness. More data is not automatically better data. Separate training, validation and final test sets; prevent leakage and track transformations. Data lineage records where data came from and how it changed; provenance supports origin and custody claims.

Plan tests for components and the integrated system: functionality, performance, security, robustness, bias, interpretability and user interaction. Define ground truth, appropriate metrics, sampling and limitations. Investigate problems and document results rather than selectively reporting favorable benchmarks. Exercise: explain why a model tested on training records appears excellent but provides weak evidence of generalization.

## III.C — Release, monitor and maintain

Prepare versioned documentation, evidence of fitness, known limits, operating instructions and applicable conformity work. Check operational readiness, monitoring, incident response and fallback before release. A model card is useful documentation but is not itself a test result or certification.

Monitor performance, harms, drift and changed conditions. Use periodic assurance, threat modeling and authorized adversarial testing appropriate to risk. Investigate failures with engineering and business stakeholders; causes may include data quality, brittle assumptions, population shift or inadequate testing. Prepare appropriate external information without confusing transparency with publishing confidential material. Exercise: build a decision record for a degraded model after a population change.

## IV.A — Choose deployment approach

Establish business objectives, performance requirements, available data, ethical constraints and workforce capability. Compare conventional predictive and generative models; proprietary and open-weight options; model size; and language or multimodal capabilities. 'Larger' is not always better for the task.

Compare cloud, on-premises and edge deployment in terms of control, latency, capacity, security, privacy, maintenance and cost. Understand using models directly, fine-tuning, RAG and agents. Each changes risk and responsibility. Exercise: identify what changes when an internal Q&A assistant gains the ability to update customer accounts.

## IV.B — Assess the selected system and supplier

Reassess impacts in the customer's actual deployment. Provider evaluations may not cover the local population, integration or purpose. Examine vendor and license terms for permitted use, data, outputs, evaluation rights, model changes, responsibility and exit.

Building a proprietary model can increase control and also increase development, evidence and maintenance obligations. Buying a model does not transfer all accountability. Exercise: review a supplier with strong security assurance but weak AI performance evidence and write a conditional decision without treating the two assurance types as equivalent.

## IV.C — Govern live use and retirement

Apply policies in production through access, training, evidence capture and decision accountability. Monitor the entire system, schedule maintenance and reassess material changes. Periodic assurance must include realistic behavior and downstream effects, not only service uptime.

Maintain incident and risk records, post-deployment monitoring and external communication plans. Consider secondary use: a harmless summarizer can become consequential if its output is reused for dismissals. Define deactivation, localization or restriction criteria where appropriate, and preserve continuity and required records. Exercise: rehearse switching off an agent's transaction authority while maintaining a manual service and investigating harm.

## Curriculum completion

Completion means every coverage-map objective has been examined, with demonstrated reasoning recorded. It does not mean the learner is guaranteed to pass or that the enterprise is compliant. Use independent official practice material if available to calibrate preparation, without importing protected exam questions into this skill.
