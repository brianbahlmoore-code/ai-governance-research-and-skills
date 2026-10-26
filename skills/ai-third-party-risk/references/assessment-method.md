# AI supplier assessment method

This is an original enterprise workflow informed by AI RMF, ordinary assurance review and the previously reviewed community TPRM skill. It is not an official certification assessment or a fixed regulatory questionnaire.

## Scope the relationship

Identify the legal supplier, contracted service, plan, region, tenant settings, model(s), versions, integrations, support access and upstream providers. Understand whether the product merely suggests text, influences consequential decisions or executes actions. A familiar SaaS service can acquire a materially different risk profile when an AI feature is enabled.

Assess deployment context: external API, hosted platform, embedded SaaS, open weights on customer infrastructure, customized model, managed agent or subcontracted AI process. Self-hosting can improve certain controls while increasing patching, model integrity and operational responsibilities. Do not call open weights 'risk free' or assume the published license covers training-data rights.

## Tiering

Use the enterprise's method. Without one, propose tiers using harm severity, data sensitivity/volume, autonomy, business criticality, substitutability and concentration. A single severe dimension can justify enhanced review; do not average away potential serious harm because the vendor is inexpensive.

Enhanced: consequential decisions, sensitive data at scale, broad action authority or critical dependency. Standard: bounded internal support with controlled data and meaningful human review. Lightweight: limited low-impact use with minimal sensitive information and easy substitution. These labels are internal conventions, not legal classifications.

Unknown material facts keep the tier provisional. Ask a short set of gating questions first, then deliver a useful evidence-gap assessment rather than an unbounded document request.

## Two assurance tracks

Track A evaluates organization and service security: report scope, identity/access, encryption, vulnerability management, incident response, resilience, subprocessors, privacy terms and financial viability.

Track B evaluates AI behavior and context: permitted data uses, training/retention, model lineage, testing relevance, harmful bias, factual reliability, explainability, oversight, agent permissions, model-change controls, intellectual-property allocation and exit constraints. Passing Track A does not establish Track B.

## Review assurance documents

For a SOC 2 report check the service and system boundary, type and period, auditor's opinion, covered categories, tests and exceptions, management responses, subservice organization treatment, and customer responsibilities. Translate complementary user-entity controls into assigned customer tasks. Examine excluded upstream services and relevant evidence for them. A report can have exceptions without every exception invalidating the service; evaluate relevance, pattern and remediation.

A vendor-issued bridge letter does not extend the auditor's testing. Do not invent universal maximum gap lengths or reject solely on an arbitrary exception count. Assess freshness and continuity against the risk and upcoming assurance cycle.

For ISO certificates verify issuer, accreditation where relevant, validity, legal entity, sites and scope. A certificate for the provider's corporate information security system does not necessarily cover the particular AI product. Certification does not prove the model is fair, accurate or suitable for a customer decision.

For model/system cards identify intended and excluded uses, model/configuration version, evaluation population, test method, metrics, known limitations and provenance. Distinguish independent evaluation from provider testing or marketing. Benchmark performance should be supplemented with customer-context validation.

## Data and rights

Map prompts, attachments, retrieved records, outputs, feedback, logs, metadata, embeddings and fine-tuned weights separately. For each identify controller/processor or other applicable role, access, storage, training/evaluation use, region, retention, deletion and subprocessors. Service improvement, abuse monitoring and human review may have different terms.

Test whether contractual commitments apply to the purchased plan and enabled configuration. Record opt-outs and their effective scope. Deleting a source file may not delete embeddings, backups or derived artifacts. A provider may not be able to remove its influence from a trained model; establish realistic rights and constraints before sharing data.

## Contracts and licensing

Review permitted purposes, restrictions, customer obligations, output rights, warranties, claims limits, indemnities, liability allocation, confidentiality, security, privacy, subcontracting, geography, evaluation rights, incident notice, material changes, termination and transition. Flag clauses for counsel using business consequences and suggested negotiation objectives; do not silently rewrite agreed contracts or promise enforceability.

For AI-specific terms seek clarity on training, fine-tuning, evaluation and abuse-monitoring uses; retention; model replacements/deprecation; advance notice; evaluation restrictions; evidence access; IP defense conditions; changes in safety controls; support for disclosure/appeal duties; and export/delete capability. Whether each term is obtainable is a commercial fact to investigate, not an assumed promise.

Notification clauses must distinguish security incidents, privacy breaches and harmful AI behavior. Define triggers and timing in a way compatible with applicable obligations; do not universally equate GDPR's controller notification clock with the processor-to-customer duty.

## Concentration and fourth parties

Map common dependencies across vendors. Two resellers of the same foundation model may not provide meaningful diversification. Evaluate common hosting, region, model, identity, data and tool providers, capacity constraints, insolvency, API shutdown and service-policy changes. Compare technical portability with practical migration costs and time.

## Decision and monitoring

For each material finding state evidence, consequence, existing controls, remaining uncertainty, requested remediation and disposition. A restricted pilot must specify data limits, user cohort, allowed actions, duration, evaluation goal and stop criteria. Never allow a pilot label to mask production impact.

Refresh on model/version changes, new training purposes, subprocessors, regions, permissions, incidents, assurance findings, contract changes, new uses or population changes. Monitor performance and harms alongside SLA uptime. Agree who receives notices and what event pauses use.

## Exit

Identify export formats and rights, replacement validation, transition assistance, access revocation, credential and OAuth removal, retrieval stores, embeddings, memory, fine-tuned artifacts, logs, backups and legal holds. Test the fallback for critical services. Record what can be deleted, when, by whom and with what evidence; do not promise erasure from all upstream models without a verifiable mechanism.

## Worked example

A recruiting SaaS provides a current SOC 2 report but no evaluation for the customer's target population, uses application data for product improvement under ambiguous terms, and can replace its ranking model without notice. The security report contributes limited Track A evidence. Suggested disposition is hold for consequential automated ranking, with a possible tightly controlled evaluation using authorized non-production data. Required closure evidence includes appropriate data terms, use-case validation, candidate recourse and model-change governance. This is an illustrative scenario, not a finding about a named vendor.
