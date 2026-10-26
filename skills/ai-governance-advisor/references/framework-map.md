# Framework selection and integration

Research baseline: 2026-10-23. Sources are linked in [sources.md](sources.md). The selection and implementation architecture below are original recommendations.

## Use each instrument for its actual purpose

| Instrument | Role in the program | Appropriate output | What it does not establish |
|---|---|---|---|
| IAPP AIGP, BoK v2.1 | Individual governance knowledge and learning coverage | Competency plan and applied exercises | Organizational certification or product approval |
| ISO/IEC 42001:2023 | Organizational AI management system | AIMS scope, policy, accountability and assurance process | Automatic compliance with every law or safety of every product |
| NIST AI RMF 1.0 | Voluntary AI risk-management outcomes | Context-specific risk profile and evidence map | A NIST certification or mandatory checklist |
| NIST AI 600-1 (2024) | Generative AI risk profile | GenAI-specific threats, harms and evaluation priorities | A complete security or legal assessment |
| ISO/IEC 23894:2023 | AI risk-management guidance | A risk method integrated with enterprise risk management | A replacement for 42001 requirements |
| ISO/IEC 42005:2025 | AI system impact-assessment guidance | Documented impacts on people and society | A replacement for a legally required DPIA or other statutory assessment |
| ISO/IEC 22989:2022 | Common concepts and terminology | Consistent inventory and governance vocabulary | A technical assurance result |
| OECD AI Principles, updated 2024 | International values and policy direction | Responsible-AI principles translated into decisions | Binding legislation by themselves |
| UNESCO Recommendation on AI Ethics (2021) | Human-rights and societal lens | Stakeholder and impact considerations | A supplier assurance certificate |
| OWASP LLM Top 10 (2025 baseline) | Application security threat coverage | Threat model and adversarial test cases | Complete fairness, privacy or lifecycle governance |
| NIST SP 800-218A (2024) | Secure AI development practices | Engineering assurance evidence | General enterprise governance |
| IMDA Agentic AI Framework (2026) | Agent deployment governance | Authority boundaries and human-accountability design | A universal agent safety guarantee |
| NIST Cybersecurity and Privacy Frameworks | Existing cyber and privacy integration | Shared enterprise controls and reporting | Coverage of all AI-specific harms |
| Applicable legislation and contractual commitments | Binding obligations in scope | Applicability register and evidence obligations | A globally uniform risk classification |

ISO's public descriptions establish the scope of its standards; this pack does not reproduce their normative text. Exact editions, amendments and clause references must be checked when undertaking a formal assessment.

## One evidence system, multiple views

Maintain a canonical chain:

`Use-case ID -> system/version -> role and jurisdiction -> harm scenario -> obligation/control -> test -> evidence -> residual risk -> decision -> monitoring trigger`.

Give controls organization-owned identifiers such as GOV-01 rather than masquerading as official ISO or NIST controls. A control can support several frameworks, but record mapping strength: direct-topic, partial-topic or contextual. Explain the unmapped remainder. A policy document and an operating-effectiveness test answer different questions.

Example: GOV-12 is a supplier model-change control. Procurement obtains advance notice; engineering records version changes; the product owner determines impact; validation runs regression tests; the authorized owner decides whether continued use is acceptable. Evidence includes contractual notice terms, a version log, test results and the decision record. This helps supplier management, lifecycle monitoring and risk treatment simultaneously. None of those mappings proves all associated framework requirements are met.

## NIST operating interpretation

The four functions are GOVERN, MAP, MEASURE and MANAGE. GOVERN is cross-cutting; the functions are iterative, not four sequential approval gates. Read the official Core tables for exact categories and subcategories. The Playbook offers optional implementation suggestions, not requirements to complete in full. NIST's site reported an ongoing revision at the research date; do not label a draft as the final successor. [N1, N2, N3]

For an internal profile, select relevant outcomes, explain exclusions, record current evidence, set a target state and assign gaps. Keep risk appetite, system performance and organizational maturity separate. A high maturity score does not make a high-impact use case safe.

## Integration priorities

Start with AIMS accountability and scope, NIST risk reasoning, human impact analysis, and vendor due diligence. Add GenAI and agent controls where the architecture needs them. Reuse existing information security, privacy, procurement and change-management mechanisms where effective. Do not create another committee or questionnaire merely because a new framework has been added.

For financial institutions, assess current model-risk and third-party guidance; SR 26-2 superseded SR 11-7 in April 2026. The 2026 TPRM proposal found during research remains a proposal unless a later final source says otherwise. These are sector overlays, not the default governing rules for every enterprise. [F1, F2, F3]
