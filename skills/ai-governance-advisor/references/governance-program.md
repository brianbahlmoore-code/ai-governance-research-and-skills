# Enterprise governance operating model

This is a proposed operating design, to be tailored to the enterprise. It is not a reproduction of a framework's mandatory requirements.

## Establish the decision structure

Make a business executive accountable for each use case. The system owner maintains implementation and monitoring; data owners establish permitted uses and quality; security tests threats; privacy evaluates personal-data impacts; legal determines applicable obligations; procurement manages vendor commitments; risk provides challenge; independent assurance evaluates whether the process works. Smaller enterprises can combine roles, while documenting conflicts and preserving proportionate independent challenge for consequential decisions.

A governance forum should decide material exceptions and portfolio priorities, not review every low-impact draft. Its charter should define jurisdiction, escalation, quorum, decision rights, reporting and expiry of exceptions. Executive oversight should address aggregate concentration, unresolved severe harms and resources needed to treat risks.

## Build an inventory that can support decisions

Record systems already operating as well as proposed systems, embedded AI in purchased SaaS and employee use of general-purpose tools. Inventory rows should include business purpose, affected population, system and model identifiers, model version, deployment geography, organizational roles, personal/sensitive data, vendors and upstream providers, tool permissions, lifecycle status, risk owner, assessment links and next review trigger.

Do not assume every spreadsheet is AI or that only internally trained models count. Establish a practical intake definition, keep uncertain entries provisional and reconcile the register against procurement, software catalogs, cloud services and business-owner attestations within the user's authorized scope.

## Policy architecture

| Policy area | Decision it must support | Evidence of operation |
|---|---|---|
| Acceptable use | Which tasks, data and tools employees may use | Approved-tool catalog, training and exception records |
| AI procurement | What must be verified before purchase or expansion | Tiered assessment, terms and conditional acceptance |
| Development and validation | Which evidence is needed for release | Versioned test plan, results and review findings |
| Data governance | Whether data can lawfully and appropriately be used | Provenance, permitted-purpose and quality records |
| Human oversight | Who can intervene and how | Tested intervention, escalation and fallback |
| Changes and monitoring | When prior approval ceases to be reliable | Change log, regression results and thresholds |
| Incident response | How harm is contained and investigated | Incident records, recovery tests and corrective action |
| Retirement | How dependencies and retained data are handled | Exit rehearsal, deletion evidence and access removal |

Translate principles into operational tests. 'Fairness' becomes a justified choice of evaluation slices and metrics, review of limitations, and a remedy path. 'Human oversight' becomes competent reviewers with time, authority, information and an effective intervention mechanism.

## Suggested lifecycle gates

1. Intake: establish purpose, benefit, owner, alternatives and initial affected-party analysis.
2. Design or acquisition: set requirements, risk hypotheses, vendor conditions and test thresholds before building or buying.
3. Validation: evaluate the deployed configuration with representative data; resolve material findings or document justified conditions.
4. Release: record decision, scope, version, limitations, operational readiness, fallback and monitoring ownership.
5. Operation: review indicators, incidents, complaints, data/model changes and vendor changes; reassess when the original assumptions cease to hold.
6. Retirement: manage replacement, exported records, access, retained data, model artifacts and downstream dependencies.

These are organizational workflow suggestions. Do not present them as the sequence mandated by NIST.

## A practical first 90 days

Days 1-30: agree scope and ownership; identify the highest-impact uses; launch an inventory; define provisional risk criteria; assess two representative use cases; collect current supplier terms. Output a short charter, usable register and prioritized gaps.

Days 31-60: implement proportionate release and procurement gates; test evidence capture; establish incident escalation and minimum monitoring; train owners using actual scenarios. Pilot with one internally developed system and one purchased AI service.

Days 61-90: evaluate whether controls operated; test a model-change and shutdown scenario; review material exceptions; report portfolio exposures; adjust thresholds and resourcing. A 90-day plan is a starting implementation period, not a promise of certification.

## Meaningful reporting

Prefer material-risk exposure, overdue high-severity treatments, assessment coverage of consequential uses, vendor concentration, incidents by harm type, unresolved appeals, unauthorized model changes, and demonstrated fallback capability. Counts of policies written or employees trained alone are weak indicators.

For every metric specify denominator, scope, measurement window, limitations, owner and action threshold. Example: '3 of 12 consequential deployments lack current independent evaluation' is more decision-useful than '75% governance compliant.' Keep risk aggregation explainable; shared upstream providers can make nominally independent systems fail together.
