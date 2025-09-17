Comprehensive Introduction to Software Testing
What is Software Testing?

Software testing is the process of executing a program or system to evaluate its behavior and verify that it meets specified requirements and quality criteria. Testing aims to discover defects (bugs), ensure the product works as intended, and provide confidence to stakeholders that the software is reliable and fit for purpose.

**Why testing matters**
1. Finds defects before customers do (reduces cost & reputation damage).
2. Verifies requirements and business needs are met.
3. Improves product quality, reliability, and user experience.
4. Helps teams move faster with confidence via automation and CI.

**Core Concepts & Terminology**

1. Defect (Bug): A deviation between expected and actual behavior.
2. Error: A human mistake in code, design, or requirements.
3. Failure: When the system behaves incorrectly during execution.
4. Verification vs Validation
     Verification: "Are we building the product right?" (e.g., code reviews, static analysis).
     Validation: "Are we building the right product?" (e.g., system tests, UAT).
5. Testability: How easy it is to test a component (clear outputs, deterministic behavior).
6. Test Case: Steps, input, expected result to verify a particular behavior.

**Principles of Software Testing (practical distilled list)**

1. Testing shows the presence of defects, not their absence. Passing tests don’t guarantee zero bugs.
2. Exhaustive testing is impossible. Use risk-based selection and heuristics.
3. Start testing early. Shift-left: test during requirements and design phases.
4. Defect clustering. Often a small number of modules contain the majority of defects.
5. Pesticide paradox. Running the same tests repeatedly will stop finding new bugs — update tests.
6. Context matters. Testing approach varies by domain (banking vs game vs embedded).
7. Avoid “absence of errors” fallacy. A system may meet all tests but still fail user expectations.
