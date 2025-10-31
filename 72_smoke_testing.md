# Smoke Testing

### What is Smoke Testing?
Smoke Testing (also known as “Build Verification Testing”) is a **quick initial test** to ensure the basic functionalities of the software work before deeper testing begins.

---

### Why It’s Important
It saves time and effort by catching major issues early.  
Smoke Testing ensures:
- The build is stable enough for further testing  
- Core features are functional  
- No critical blockers exist  

---

### Goals
- Verify basic functionality of main features  
- Detect major failures quickly  
- Approve or reject a build for further QA  

---

### Example
**Scenario:**  
Checking if the app launches, login works, and main navigation opens without errors before detailed testing.

---

### Tools
- Jenkins (for CI smoke builds)  
- Selenium  
- Katalon Studio  
- Manual test checklists  

---

### Common Issues
- Builds with missing dependencies  
- Incomplete deployments causing early failures  

---

### Best Practices
- Automate smoke tests in CI/CD pipeline  
- Keep the suite small and fast  
- Run smoke tests on every build  

---

### Conclusion
Smoke Testing ensures your software **is ready for deeper testing** by verifying essential functionality early.

---
