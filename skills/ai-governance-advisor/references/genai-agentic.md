# Generative and agentic AI assurance

Baseline sources: NIST AI 600-1 (2024), OWASP LLM Top 10 (2025), NIST SP 800-218A (2024), and IMDA's 2026 agentic-framework announcement. The detailed controls below are original recommendations, not quotations or an assertion that every source mandates them.

## Expand beyond model accuracy

NIST's GenAI profile covers risks including confabulation, data privacy, information integrity/security, harmful content and bias, intellectual property, human-AI relationships, environmental effects, dangerous capabilities and value-chain integration. Use the official profile to select relevant actions; do not substitute this brief overview for its complete taxonomy. [N4]

The verified OWASP 2025 baseline covers prompt injection, sensitive-information disclosure, supply chain, poisoning, improper output handling, excessive agency, system-prompt leakage, vector/embedding weaknesses, misinformation and unbounded consumption. It is security-oriented and complements broader governance. [O1]

## Configuration matters

Assess model-only behavior separately from retrieval, tool use, memory, routing and human review. RAG introduces document provenance, access-control and stale-source risks. Fine-tuning introduces training-data rights, retention and model-change risks. Agentic workflows add delegated authority, repeated actions, state and third-party tool dependencies. A local or open-weight model still needs legal, data and security analysis.

## Original control design patterns

| Risk scenario | Design question | Useful evidence |
|---|---|---|
| Plausible but unsupported output | Can the task tolerate error, and when must the system abstain or escalate? | Task-specific evaluation, source checking and escalation tests |
| Cross-user disclosure through retrieval | Are permissions enforced before retrieval and at every data boundary? | Negative authorization tests and data-flow diagrams |
| Instruction embedded in an untrusted document | Can retrieved text alter privileges or cause execution? | Adversarial tests across content/tool boundaries |
| Unsafe downstream execution | Is model output validated as untrusted input by the receiving service? | Typed interfaces, constrained parameters and rejection logs |
| Excessive agent authority | What actions can it take, under whose authority, and within what limits? | Permission inventory, scoped identities and action policies |
| Irreversible or repeated action | Can actions be previewed, bounded, deduplicated, stopped and recovered? | Approval/transaction controls, budgets and rollback exercises |
| Vendor model update | Can the enterprise identify the change before sensitive deployment? | Version records, notices and regression evidence |
| Compromised dependency or model artifact | How are origin, integrity and updates verified? | Supplier provenance, artifact verification and change review |
| Misleading synthetic content | Do users understand the interaction and output provenance? | User comprehension tests and disclosure review |

## Human oversight design

Choose the oversight pattern by consequence and reversibility. A reviewer needs enough context to detect errors, sufficient time, authority to reject, an escalation route and a workable alternative. A confirmation click after an irreversible action is not effective oversight. Evaluate automation bias, workload, accessibility and whether reviewers actually intervene appropriately.

For agents define a scope contract: task, permitted data, tools, action classes, financial/time/rate limits, approval points, prohibited actions, stop conditions, identity, logs and responsible person. Every downstream tool should enforce permissions independently of the model's reasoning or system prompt. Keep credentials out of prompts and untrusted content.

## Evaluation release pack

Record model identifier/version, deployment parameters, prompts, retrieval corpus version, tool configuration, test environment and dates. Include normal tasks, boundary conditions, misuse scenarios, denied actions, unavailable dependencies, conflicting instructions, partial failures and recovery. State sampling and coverage limits. A red-team pass is evidence about tested conditions, not a proof of absence of vulnerabilities.

Thresholds should reflect the harm and acceptable exposure; avoid universal '95% accuracy is safe' rules. Track harmful errors separately from cosmetic errors, use-case utility separately from refusal rate, and new versions against the same regression set plus newly discovered failures.

## Monitoring and retirement

Watch for task drift, output failures, permission changes, cost spikes, sensitive-data exposure, provider changes and user complaints. Define an emergency route to disable consequential actions while preserving appropriate evidence and business continuity. When retiring, consider memories, embeddings, uploaded files, logs, caches, fine-tuned artifacts, connected tools and upstream retention. A no-training statement is not a zero-retention guarantee.
