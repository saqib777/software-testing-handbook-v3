# 14. Static vs Dynamic Testing

## Overview

In software testing, all testing activities can be broadly classified into two major categories — **Static Testing** and **Dynamic Testing**.  
These two types complement each other: one focuses on *prevention* (before execution), and the other focuses on *detection* (during execution).

Together, they ensure a more complete quality assurance process — identifying defects early, saving cost, and ensuring reliability.

---

## 1. Static Testing

### Definition
Static testing is a **verification process** that checks code, documents, or design *without executing the program*.  
It aims to catch defects early in the development lifecycle, even before the code runs.

### Objective
To find errors in:
- Requirements
- Design
- Code syntax
- Test cases
- Documentation  

### Key Activities
| Activity | Description |
|-----------|-------------|
| **Reviews** | Formal evaluation of documents or code by peers or QA team. |
| **Walkthroughs** | Informal sessions where the author explains the work to stakeholders for feedback. |
| **Inspections** | Systematic examination of documents/code to detect defects early. |
| **Static Code Analysis** | Automated tools check for syntax errors, coding standards, or potential bugs. |

### Example
- Reviewing a **requirement document** to ensure no ambiguity (e.g., “The system should be fast” → too vague).  
- Running **SonarQube** on a codebase to find unused variables or security vulnerabilities before compilation.

### Tools
- **SonarQube**
- **Checkstyle**
- **PMD**
- **Lint**
- **CodeClimate**

### Advantages
- Detects errors early (before runtime).  
- Reduces rework and overall project cost.  
- Improves documentation quality and code maintainability.  
- Saves time during later testing stages.

### Limitations
- Cannot find runtime errors or performance issues.  
- Relies on human expertise and peer reviews.  
- May miss logic errors that appear only during execution.

---

## 2. Dynamic Testing

### Definition
Dynamic testing is a **validation process** that involves executing the code to check its behavior, functionality, and performance.  
It verifies that the software works according to requirements.

### Objective
To detect defects that occur **during runtime** — related to logic, flow, data handling, and user interaction.

### Key Activities
| Activity | Description |
|-----------|-------------|
| **Unit Testing** | Testing individual components or functions. |
| **Integration Testing** | Testing the interaction between integrated modules. |
| **System Testing** | Testing the complete application as a whole. |
| **Acceptance Testing** | Validating that the system meets business needs. |

### Example
- Running a **login module** with valid and invalid credentials to verify user authentication.  
- Checking a **payment gateway** under different input conditions to ensure smooth transactions.

### Tools
- **Selenium**
- **JUnit / TestNG**
- **Cypress**
- **Postman (for API testing)**
- **LoadRunner / JMeter** (for performance)

### Advantages
- Ensures the system performs correctly under real conditions.  
- Identifies issues missed during static testing.  
- Confirms software meets user expectations.  
- Enables validation of functional and non-functional requirements.

### Limitations
- Performed later in the SDLC (more expensive to fix).  
- Requires test environments and data setup.  
- Time-consuming, especially for large systems.

---

## Comparison Table: Static vs Dynamic Testing

| **Aspect** | **Static Testing** | **Dynamic Testing** |
|-------------|--------------------|---------------------|
| **Nature** | Verification (without execution) | Validation (with execution) |
| **Performed On** | Documents, code, design | Running software/application |
| **Objective** | Prevent defects early | Detect defects during runtime |
| **Examples** | Code review, walkthrough, static analysis | Unit, integration, system testing |
| **Performed By** | Developers, QA reviewers | Testers, QA engineers |
| **When** | Early stages (before code runs) | Later stages (after build) |
| **Tools** | SonarQube, PMD, Checkstyle | Selenium, JUnit, JMeter |
| **Type of Defects Found** | Syntax, design, documentation issues | Logic, performance, runtime errors |
| **Cost of Fixing** | Low | High |
| **Output** | Review reports, static analysis reports | Test execution results, defect logs |

---

## Relationship Between Static and Dynamic Testing

These two are not competitors — they’re **complementary** parts of a robust QA strategy.

| **Static Testing** | → Prevents defects before code runs |
|---------------------|-------------------------------------|
| **Dynamic Testing** | → Detects defects after code runs |

- Static testing ensures code quality and compliance with standards.  
- Dynamic testing ensures the system behaves as expected in real scenarios.  
- Using both improves **defect prevention and detection** across the SDLC.

---

## Example Scenario

> **Project:** Online Shopping Cart  
> **Static Testing Example:** Reviewing requirement documents to ensure “Add to Cart” feature clearly specifies quantity, price updates, and stock validation.  
> **Dynamic Testing Example:** Actually running the “Add to Cart” feature and verifying the total price updates correctly when multiple items are added or removed.

---

## Notes & Best Practices

- Always perform **static testing first** — it’s cheaper and faster to fix defects early.  
- Automate **static code analysis** in CI pipelines.  
- Pair static reviews with **dynamic test execution** for maximum coverage.  
- Encourage **peer reviews** before merge or deployment.  
- Maintain logs of both static and dynamic findings for traceability.

---

## Final Thoughts

Static and dynamic testing together form the backbone of a **complete testing lifecycle**.  
Static testing prevents bugs; dynamic testing detects them.  
A balance of both ensures that software is not just working — but is **robust, maintainable, and future-proof**.

---

*End of File — 14_static_vs_dynamic_testing.md*
