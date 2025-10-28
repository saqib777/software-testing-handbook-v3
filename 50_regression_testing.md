# Regression Testing

### What is Regression Testing?
Regression Testing ensures that **new code changes haven’t broken existing features**.  
It verifies that updates, fixes, or enhancements don’t negatively affect the rest of the system.

---

### Why It’s Important
Every time you modify code, there’s a risk of unintentionally breaking something that previously worked.  
Regression Testing ensures:
- Stability after updates  
- Confidence in frequent releases  
- Early detection of reintroduced bugs  

---

### Goals
- Re-test existing features after code changes  
- Confirm backward compatibility  
- Maintain product quality over time  

---

### Example
**Scenario:**  
After adding a new “Search Filter,” you retest the older search functionality to ensure it still returns correct results.

---

### Tools
- Selenium  
- JUnit / TestNG  
- Jenkins (for continuous testing)  
- Katalon Studio  

---

### Common Issues
- Neglecting to update old test cases  
- Overlooking dependent modules  
- Increased execution time for large suites  

---

### Best Practices
- Maintain a prioritized regression suite  
- Automate frequently tested flows  
- Run regression tests after every build or sprint  
- Use CI/CD pipelines for efficiency  

---

### Conclusion
Regression Testing ensures that **new changes don’t break old features**, maintaining reliability release after release.

---
markdown
Copy code
# 51_smoke_testing.md

## Smoke Testing

### What is Smoke Testing?
Smoke Testing is a **preliminary check** to verify that the basic and critical features of the software work properly.  
It’s like checking if “the build is stable enough to test further.”

---

### Why It’s Important
Before spending time on detailed testing, you need to confirm the application’s core functionality works.  
Smoke Testing helps:
- Detect major issues early  
- Save time by avoiding deep tests on unstable builds  
- Ensure deployment success  

---

### Goals
- Validate basic operations (login, navigation, main workflows)  
- Ensure build stability before regression or detailed testing  

---

### Example
**Scenario:**  
After deployment, testers perform a smoke test by logging in, performing a simple transaction, and logging out — if all work, deeper testing begins.

---

### Tools
- Jenkins (for build verification)  
- Selenium  
- Katalon Studio  
- Cypress  

---

### Common Issues
- Ignoring smoke testing on minor builds  
- Running too many unnecessary tests  
- Lack of automation in build verification  

---

### Best Practices
- Focus only on high-level functions  
- Automate smoke tests as part of CI  
- Keep the suite short and fast  

---

### Conclusion
Smoke Testing ensures that your **application is ready for deeper testing**, saving time and catching major bugs early.

---
