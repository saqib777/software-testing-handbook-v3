# Test Plan vs Test Strategy

## 1. Introduction

In software testing, two key documents guide the overall testing effort — **Test Plan** and **Test Strategy**.  
Although often used interchangeably, they are **not the same**.  
Each serves a different purpose and audience, helping teams align testing goals, scope, and execution strategy.

---

## 2. What is a Test Plan?

A **Test Plan** is a *project-level document* that defines **what to test, how to test, who will test, and when testing will happen**.  
It is typically created by a **Test Lead or QA Manager** for a specific project or release.

**Purpose:**  
To describe the **scope**, **approach**, **resources**, **schedule**, and **deliverables** of the testing activities.

---

### 📋 Example Contents of a Test Plan

| Section | Description |
|----------|--------------|
| **Test Plan ID** | Unique identifier for traceability |
| **Introduction** | Brief about the project/module |
| **Test Items** | Features or functionalities to be tested |
| **Features Not to be Tested** | Out-of-scope items |
| **Test Approach** | Manual, Automation, Performance, etc. |
| **Test Environment** | Hardware/software setup details |
| **Test Schedule** | Timelines for test execution |
| **Entry & Exit Criteria** | When to start and stop testing |
| **Deliverables** | Test cases, reports, bug logs, etc. |
| **Roles & Responsibilities** | Assigned QA team members |
| **Risks & Mitigation** | Potential issues and how to handle them |

---

### 📘 Example:

> **Project:** Online Banking App  
> **Objective:** Validate login, transactions, and account summary features before release.  
> **Test Scope:** Functional testing on web and mobile.  
> **Approach:** Manual + Automation (Selenium).  
> **Timeline:** 15th Oct – 25th Oct.  
> **Team:** 4 QA Engineers, 1 Lead.  
> **Deliverables:** Test summary report, defect log, automation scripts.  

---

## 3. What is a Test Strategy?

A **Test Strategy** is a *high-level organizational document* that defines **how testing will be done across all projects**.  
It acts as a **master guideline** for the QA process, ensuring **consistency and quality standards** across teams.

**Purpose:**  
To define **testing principles, tools, levels, and quality metrics** applicable to all projects in an organization.

---

### 📋 Example Contents of a Test Strategy

| Section | Description |
|----------|--------------|
| **Testing Objectives** | What quality goals are to be achieved |
| **Test Levels** | Unit, Integration, System, UAT |
| **Test Types** | Functional, Regression, Performance, Security, etc. |
| **Testing Tools** | JIRA, Selenium, Postman, JMeter, etc. |
| **Defect Management** | How bugs are reported, tracked, and closed |
| **Test Metrics** | Defect density, test coverage, pass/fail ratio |
| **Configuration Management** | Version control, data handling, environments |
| **Test Deliverables** | Standards for documentation and reporting |

---

### 📘 Example:

> **Organization:** FinTech Solutions Ltd.  
> **Objective:** Define a unified QA process across all development teams.  
> **Tools:** Jira, TestRail, Selenium, Jenkins.  
> **Approach:** Shift-left testing with automation-first strategy.  
> **Metrics:** 95% automation coverage for regression suites.  
> **Compliance:** ISO 25010 Quality Model.  

---

## 4. Key Differences Between Test Plan and Test Strategy

| Criteria | Test Plan | Test Strategy |
|-----------|-------------|----------------|
| **Definition** | Project-level document describing testing activities for a specific release | Organization-level document defining QA approach for all projects |
| **Owner** | QA Lead / Test Manager | QA Director / Organization QA Head |
| **Scope** | Specific to one project | Applies to multiple projects |
| **Purpose** | Guides execution | Defines overall approach |
| **Level of Detail** | High (with schedules, roles, deliverables) | Conceptual (principles and policies) |
| **Change Frequency** | Updated frequently | Updated rarely |
| **Approval** | By Project Manager / Client | By Organization QA Head |
| **Focus Area** | Execution & management | Process & methodology |
| **Example** | Banking app test plan | Company-wide QA strategy document |

---

## 5. Relationship Between Test Plan and Test Strategy

Think of the **Test Strategy** as the **master rulebook**,  
and the **Test Plan** as a **specific match plan** based on those rules.

