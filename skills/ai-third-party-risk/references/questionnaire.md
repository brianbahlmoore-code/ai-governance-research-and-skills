# AI vendor due-diligence question bank

Original questions. Select by use case and tier; these are not licensed SIG questions. Record answer, evidence ID, scope/version, assessor conclusion, gap, owner and follow-up. 'Yes' without supporting evidence is a claim.

## Service and supply chain
1. Which legal entity, product, plan and deployment region does the answer cover? Request the service boundary and applicable terms.
2. Which models and versions serve this workload? Request the model inventory and routing/update policy.
3. Which upstream model, hosting, data, retrieval and tool providers are involved? Request the dependency map and subprocessors.
4. Which intended or excluded uses apply? Request use restrictions and relevant system/model cards.
5. Which customer configurations change responsibility or assurance coverage? Request a shared-responsibility matrix.

## Data handling and rights
6. Are prompts, outputs, attachments or feedback used for training, fine-tuning or evaluation? Request plan-specific contractual commitments and settings.
7. What is retained for service operation, abuse monitoring and human review? Request distinct retention schedules and access controls.
8. Where is each data category processed and stored, including support and backups? Request region/transfer details.
9. What provenance and use-rights evidence is available for training data and third-party components? Request evidence boundaries where disclosure is restricted.
10. How are customer data, embeddings and fine-tuned artifacts isolated? Request architecture and test evidence.
11. How are deletion and return implemented across active stores, caches, backups and upstream providers? Request tested procedures and exceptions.
12. How are sensitive data and data-subject requests handled? Request applicable roles, processes and contractual assistance.

## Performance and human impact
13. What evaluations support the customer's actual task and population? Request methods, datasets, versions and limitations.
14. What is known about harmful error rates and subgroup performance? Request uncertainty and sampling information.
15. How are unsupported outputs detected and handled? Request task-specific results and escalation behavior.
16. Which distribution shifts and edge cases were evaluated? Request robustness findings.
17. What explanation, notice and recourse features can the customer configure? Request demonstrations and user testing.
18. Which human interventions are possible before consequential action? Request evidence of authority, usability and response time.
19. How does the vendor evaluate downstream use and misuse? Request impact assessment summaries and restrictions.

## Security and agent authority
20. How are prompt-injection and retrieval trust boundaries tested? Request scoped adversarial results and remediation.
21. Are tool calls enforced by independent permissions and validated parameters? Request authorization architecture and negative tests.
22. Can the customer bound transactions, destinations, spend, rate and retries? Request configuration and limit tests.
23. How are identities, secrets and customer-scoped credentials managed? Request control evidence without disclosing live secrets.
24. How are models, dependencies and updates verified for origin and integrity? Request change and provenance records.
25. What protects retrieval stores against cross-tenant access and poisoning? Request access and integrity tests.
26. Can agent actions be stopped, deduplicated, reversed or safely recovered? Request a recovery exercise.

## Assurance and incidents
27. Which independent reports/certificates cover this service and period? Request full applicable scope and exceptions.
28. What customer controls and excluded subservice controls are required? Request responsibility and evidence mapping.
29. What material security or harmful-AI incidents affected this service? Request relevant history, lessons and closure evidence.
30. What triggers customer notification, and how quickly? Request binding terms for security, privacy and AI behavior incidents.
31. Can the vendor support regulatory inquiries, impact assessments and affected-person remedies? Request commitments and service channels.

## Changes and monitoring
32. Which changes receive advance notice? Request coverage of models, safety behavior, data uses, regions and providers.
33. Can customers pin versions or validate changes before adoption? Request limitations, deprecation periods and rollback options.
34. Which performance, harm and usage metrics can the customer obtain? Request sample reports and access methods.
35. What happens when a model is suspended, deprecated or capacity constrained? Request continuity and communication plans.

## Commercial terms and exit
36. Which IP rights, warranties, indemnities and exclusions apply to inputs and outputs? Request the executed or proposed terms.
37. Do evaluation, benchmarking or disclosure restrictions prevent adequate assurance? Request the permitted review process.
38. What export formats, migration assistance and deletion evidence are available? Request a tested exit plan.
39. What dependencies make replacement difficult or create concentration? Request realistic migration estimates and constraints.
40. Which commitments survive termination and which artifacts cannot be fully removed? Request the retention and survival clauses.

## Closing the assessment

Convert unanswered material questions into specific evidence gaps. Distinguish 'not applicable with rationale' from 'not disclosed' and 'not implemented.' Avoid aggregate vendor scores that conceal a critical failure. Record customer-side actions alongside supplier remediation.
