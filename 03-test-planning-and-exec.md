# 3. Test planning and execution

## 3.1 Describe how you would establish a test process that runs from needs and requirements through to production release and follow-up.
I would establish a clear testing process that starts when a requirement is discussed and continues until after the feature is released. The goal is to find problems early, protect data quality, and release changes safely.

1. Understand requirements and risks
- The PO and BA define business needs and acceptance criteria.
- QA and developers identify possible risks and agree on what needs testing.
- High-risk changes receive more testing than low-risk changes.

2. Test levels and types of testing
- Unit testing: Developers test individual pieces of code.
- Integration testing: Check that connected systems exchange data correctly.
- End-to-end testing: QA test the complete business workflow across systems.
- Regression testing: Ensure new changes do not break existing features.
- Acceptance testing: Confirm that the solution meets business requirements.
- Exploratory testing: Test manually to discover unexpected problems.

3. Manual testing versus automated testing.
I would automate repetitive tests and important regression scenarios because they save time and provide fast feedback. Manual testing is useful for exploratory testing, usability, and new features where expected behaviour is not yet fully understood.

4. Risk-based and change-based prioritisation.
- Test critical data flows, business rules, and integrations first.
- Focus on the areas affected by the change and check related features for side effects.
- Use lightweight testing for low-risk changes and deeper testing for high-risk changes.

5. Test data, test environments and test coverage.
- Use realistic, controlled test data, including valid, invalid, missing, and duplicate records.
- Keep test environments stable and as close to production as practical.
- Track test coverage to make sure important requirements, risks, and workflows are tested.

6. Handling of defects, deviations and reopened issues.
- Record each defect with steps to reproduce it, its impact, and supporting evidence.
- Prioritise defects based on business impact and severity.
- Developers fix the issue, and QA verifies the fix and runs relevant regression tests.
- If an issue happens again, reopen it and investigate the root cause.

7. Define entry, exit, and release criteria
Entry criteria — before testing starts:
- Requirements and acceptance criteria are clear.
- The build, environment, and test data are ready.

Exit criteria — before testing is considered complete:
- Planned critical tests have passed.
- No unresolved critical defects remain.
- Important risks and any accepted deviations are documented.

Production release criteria:
- Required tests have passed and business acceptance is confirmed.
- Remaining risks are understood and approved by the appropriate owners.
- Monitoring and rollback or recovery plans are ready where needed.

8. Monitor after release
After release, I would monitor errors, data quality, and system performance. Any production issues would be investigated, and the lessons learned would be used to improve tests and prevent similar problems.

Example: Making sure farm data reaches the right system
Imagine a farmer uses System A to record milk production on a farm. This data is sent to System B, where it is used to create reports and help farmers make better decisions.

Here is how I would test this process:
1. Understand the requirement: Make sure milk production data is transferred correctly and reaches System B on time.
2. Test the calculation: Check that System A calculates and prepares the milk production data correctly.
3. Test the connection: Check that System B receives the data sent by System A.
4. Check data quality: Make sure no records are missing, duplicated, or incorrect.
5. Test the complete journey: Enter milk production data in System A and confirm that the correct value appears in System B's report.
6. Check existing features: Make sure the change has not broken other reports or data transfers.
7. Release and monitor: Once the important tests pass, release the change and monitor the systems to detect missing data or delays.
For example: If System A sends 500 litres of milk but System B displays 450 litres, the test should detect the mismatch before it affects the farmer's report.

This approach helps us catch problems early, protect data quality, and give farmers reliable information they can trust.