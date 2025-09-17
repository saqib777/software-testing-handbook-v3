**Comprehensive Introduction to Software Testing**
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

**SDLC vs STLC (how testing fits)**

*SDLC (Software Development Life Cycle) — phases where software is conceived, built, deployed.
*STLC (Software Testing Life Cycle) — testing-specific lifecycle:

     1. Requirements analysis (testability, clarify ambiguous requirements)
     2. Test planning (scope, approach, schedule, resources)
     3. Test case design & test data preparation
     4. Test environment setup
     5. Test execution
     6. Defect reporting & tracking
     7. Test cycle closure & metrics

Outputs: test plan, test cases, test data, environment config, test reports.

**Testing Levels (what to test and when)**

**Unit Testing**

     1. Tests: individual functions/methods.
     2. Who: developers (often).
     3. Tools: pytest, JUnit, unittest.
     4. Example: verify add(a, b) returns correct sum for various inputs.

**Integration Testing**

     1. Tests: interactions between modules/services.
     2. Example: login component + database + session management.

**System Testing**

     1. Tests: entire application end-to-end in production-like environment.
     2. Example: full ATM flow — card insert → PIN → balance check → withdrawal.

**Acceptance Testing**

     1. Tests: satisfies business requirements; done by customer or product owner.
     2. Example: client validates checkout workflow on e-commerce site.
