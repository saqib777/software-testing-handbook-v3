# 13. Test Types in Software Testing

## Overview

While *test levels* describe **when** testing is performed, *test types* describe **what kind** of testing is done.  
Each test type focuses on a specific aspect of the system — functionality, performance, security, usability, and more.  
Understanding these helps ensure that testing covers all critical areas of software quality.

---

## 1. Functional Testing

**Purpose:**  
To verify that each feature of the software works according to the defined requirements.

**Performed By:** Testers / Automation engineers  
**Focus:** Input, output, and user interactions  
**Example:** Ensuring a “Login” button correctly validates credentials and grants access.  
**Tools:** Selenium, Cypress, Playwright

**Notes:**
- Based on black-box testing techniques.  
- Verifies “what” the system does, not “how.”  
- Includes smoke, sanity, and regression testing.

---

## 2. Non-Functional Testing

**Purpose:**  
To assess the performance, reliability, scalability, and usability of the software.

**Performed By:** QA engineers, performance testers  
**Focus:** System behavior under different conditions.  
**Example:** Measuring how long it takes for the site to load under heavy traffic.  
**Tools:** JMeter, LoadRunner, K6, Lighthouse

**Notes:**
- Focuses on system *quality attributes*.  
- Often conducted after functional stability is confirmed.  
- Includes performance, stress, and usability testing.

---

## 3. Regression Testing

**Purpose:**  
To ensure that new code changes have not adversely affected existing functionality.

**Performed By:** QA Team / Automation tools  
**Focus:** Re-running existing tests after changes.  
**Example:** After fixing a login bug, rechecking if the signup page still works.  
**Tools:** Selenium, TestNG, Jenkins, GitHub Actions

**Notes:**
- Best candidate for automation.  
- Prevents “fix one, break one” issues.  
- Should be part of every CI/CD pipeline.

---

## 4. Smoke Testing

**Purpose:**  
To quickly verify that the major functionalities of an application are working after a build or deployment.

**Performed By:** QA or developers  
**Focus:** Critical paths and high-level functions.  
**Example:** Verifying that the application launches and main screens open properly.  

**Notes:**
- Also called “build verification testing.”  
- Saves time before deeper testing begins.  
- If smoke fails → stop testing immediately.

---

## 5. Sanity Testing

**Purpose:**  
To confirm that recent bug fixes or minor changes work as expected and haven’t introduced new issues.

**Performed By:** QA Team  
**Example:** After updating the profile module, confirming that profile editing still works.  

**Notes:**
- Subset of regression testing.  
- Typically unscripted and quick.  
- Acts as a confidence check before full testing resumes.

---

## 6. Performance Testing

**Purpose:**  
To evaluate the system’s responsiveness, stability, and scalability under a specific workload.

**Performed By:** Performance testers / DevOps  
**Focus:** Response time, throughput, resource usage.  
**Example:** Simulating 1,000 users submitting forms simultaneously.  
**Tools:** Apache JMeter, Gatling, K6

**Notes:**
- Includes load, stress, and endurance testing.  
- Helps identify bottlenecks early.  
- Essential for production readiness.

---

## 7. Security Testing

**Purpose:**  
To identify vulnerabilities, threats, and risks in the system to prevent data breaches or attacks.

**Performed By:** Security testers / ethical hackers  
**Focus:** Authentication, authorization, data encryption, access control.  
**Example:** Checking if unauthorized users can access admin pages.  
**Tools:** OWASP ZAP, Burp Suite, Nessus

**Notes:**
- Ensures compliance with standards like OWASP, ISO 27001.  
- Must include penetration testing.  
- High-priority for financial, healthcare, and government apps.

---

## 8. Usability Testing

**Purpose:**  
To evaluate how easy and intuitive the application is for end-users.

**Performed By:** UX researchers / testers  
**Focus:** User experience, design flow, accessibility.  
**Example:** Observing how users navigate a form and identifying confusion points.  

**Notes:**
- Measures user satisfaction and efficiency.  
- Should include accessibility (WCAG) checks.  
- Conducted using real user feedback or eye-tracking studies.

---

## 9. Compatibility Testing

**Purpose:**  
To verify that the software works across various devices, browsers, operating systems, and screen sizes.

**Performed By:** QA testers  
**Example:** Checking if a web app displays properly on Chrome, Safari, and mobile browsers.  
**Tools:** BrowserStack, LambdaTest, Sauce Labs

**Notes:**
- Critical for web and mobile applications.  
- Helps catch environment-specific issues.  
- Should include backward compatibility tests.

---

## 10. Exploratory Testing

**Purpose:**  
To discover defects not covered by formal test cases through creative, unscripted testing.

**Performed By:** Experienced testers  
**Focus:** Intuitive testing using domain knowledge.  
**Example:** Randomly entering unexpected data into a form to see system behavior.  

**Notes:**
- Encourages tester creativity and insight.  
- Effective when documentation is limited.  
- Best suited for agile environments.

---

## Summary Table

| **Test Type**        | **Goal**                                     | **Who Performs**      | **Example**                                         |
|-----------------------|----------------------------------------------|------------------------|----------------------------------------------------|
| Functional            | Verify each function meets requirements      | QA / Automation Eng.   | Login, form submission                             |
| Non-Functional        | Assess quality attributes                    | QA / Perf testers      | Load, response time                                |
| Regression            | Ensure existing functionality works          | QA / CI pipelines      | Retest checkout flow after updates                 |
| Smoke                 | Basic build verification                     | QA / Dev               | App opens, menus load                              |
| Sanity                | Quick validation of bug fixes                | QA                     | Profile update check                               |
| Performance           | Check speed and scalability                  | Perf team              | Load test with 1k users                            |
| Security              | Identify system vulnerabilities              | Security experts       | SQL injection, XSS                                 |
| Usability             | Evaluate user experience                     | UX team                | Navigation clarity                                 |
| Compatibility         | Ensure cross-platform consistency            | QA                     | Browser/device checks                              |
| Exploratory           | Unscripted, creative defect discovery        | QA                     | Random input, boundary checks                      |

---

## Notes & Recommendations

- Each test type addresses a **specific risk area** — choose types based on system criticality.  
- Combine functional and non-functional testing for complete coverage.  
- Automate repetitive tests like regression and smoke.  
- Always perform **security and performance testing** before release.  
- Encourage **exploratory sessions** to uncover hidden defects.

---

## Final Thoughts

A well-rounded test strategy uses multiple test types to ensure robustness, reliability, and user trust.  
By applying these strategically, teams can deliver software that not only functions — but performs, scales, and delights users.

---

*End of File — 13_test_types_in_software_testing.md*
