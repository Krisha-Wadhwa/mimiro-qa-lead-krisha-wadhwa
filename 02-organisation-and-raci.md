# 2. Organisation, structure and responsibilities

I would organise quality work so that everyone is responsible for quality, with clear roles and responsibilities.
- PO (Product Owner): Defines business priorities and decides whether the product meets business needs.
- BA (Business Analyst): Understands business needs and writes clear requirements and acceptance criteria.
- PM (Project Manager): Manages timelines, resources, dependencies, and delivery risks.
- QA (Quality Assurance): Plans the testing approach, identifies risks, improves processes, and ensures quality is considered from the beginning.
- QC (Quality Control): Executes tests, finds defects, checks results, and reports issues. Developers also perform unit and technical tests.
- Developers: Fix defects and ensure code quality.
- Operations: Monitors the system after release and supports recovery if problems occur.

## Who should be responsible for each activity?
- Requirements: The Product Owner (PO) decides what the business needs, while the Business Analyst (BA) documents the requirements clearly.
- Acceptance criteria: The PO owns the final criteria, and the BA helps define the conditions that must be met for a feature to be accepted.
- Risk assessments: QA identifies testing risks together with the PO, BA, and developers. The PO focuses on business impact, while developers focus on technical risks.
- Test plans: The Test Lead / QA is responsible for planning what to test, how to test it, and how much testing is needed.
- Test execution: QA, testers, and developers perform tests. Developers test their code, while QA checks the overall quality and business workflows.
- Defect fixing: Developers are responsible for fixing defects. QA retests the fixes to confirm that the problems are resolved.
- Production release decisions: The PO confirms business acceptance, while the designated technical or operational release owner confirms production readiness. Management should clearly name the final release authority.
- In practice: Everyone contributes to quality, but each activity should have a clear owner. The team reviews test results and remaining risks before release so that decisions are based on evidence rather than assumptions.

## RACI matrix

R = Responsible for doing the work;
A = Accountable for the outcome/decision; 
C = Consulted; 
I = Informed.

Below are some Activity and the Main Owner
- Requirements and acceptance criteria	- Product Owner (PO) or  Business Analyst (BA)
- Risk assessment	- QA, PO, BA and developers
- Test planning	- Test Lead / QA
- Test execution	QA and developers
- Defect fixing	Developers
- Production Testing - PO, BA, QA

How it works in day-to-day practice
1. Before development: The PO and BA clarify requirements and acceptance criteria. QA and developers identify risks.
2. During development: Developers write and test code, while QA prepares test plans and checks important workflows.
3. When defects are found: QA reports the issues, the team prioritises them based on impact, and developers fix them. QA then verifies the fixes.
4. Before release: The team reviews test results, open defects, and remaining risks. The PO confirms business acceptance, and the authorised release owner makes the production release decision.
5. After release: Operations monitors the system, and the team reviews incidents and improves testing where needed.

My approach: Keep responsibilities clear, involve the right people early, and make release decisions based on test evidence and business risk.