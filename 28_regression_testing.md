## Regression Testing

### What is Regression Testing?
Regression Testing is performed to ensure that **new changes in the code (like bug fixes, updates, or new features)** haven’t accidentally broken the existing functionality of the application.  
In simple words — every time you make a change, you test again to make sure everything that used to work still works.

---

### Why is Regression Testing Important?
When developers add or modify features, there’s always a risk that something else might stop working.  
Regression Testing helps to:
- Catch unintended side effects early  
- Maintain software stability after updates  
- Ensure old features still function correctly  
- Build confidence before each new release  

---

### When is it Performed?
Regression Testing is done:
- After bug fixes or feature enhancements  
- After code refactoring or optimization  
- Before major releases or deployments  
- During continuous integration (CI/CD) cycles  

---

### Types of Regression Testing
1. **Corrective Regression Testing**  
   When no changes are made to the existing code, but tests are rerun to ensure everything still works.

2. **Progressive Regression Testing**  
   Done when new features are added and new test cases are created to ensure compatibility with old features.

3. **Selective Regression Testing**  
   Only tests affected parts of the system instead of retesting everything.

4. **Partial Regression Testing**  
   Ensures that the new code works correctly without affecting the existing modules.

5. **Complete Regression Testing**  
   A full re-execution of all test cases to verify system-wide stability (usually done before major releases).

---

### Common Issues Found
- Old bugs reappearing after a new update  
- Integration issues between new and old modules  
- Broken UI elements or workflows  
- Failing automated test scripts due to changes in dependencies  

---

### Tools Used
- **Selenium**  
- **JUnit / TestNG**  
- **Cypress**  
- **Appium**  
- **Jenkins** (for continuous regression in CI/CD)  

---

### Best Practices
- Automate regression test cases to save time  
- Maintain a well-organized regression test suite  
- Prioritize frequently used and business-critical features  
- Run regression tests after every code change  
- Keep test cases updated as the application evolves  

---

### Example
**Scenario:** Testing an e-commerce website  
- Developers fix a bug in the “Apply Coupon” feature  
- Regression Testing is performed to ensure:  
  - Checkout and payment still work correctly  
  - The cart updates properly  
  - Discount calculations remain accurate  
  - No new issues are introduced  

---

### Benefits of Regression Testing
- Prevents recurring bugs  
- Improves product stability  
- Saves time through automation  
- Builds user trust in new releases  

---

### Conclusion
Regression Testing ensures that improvements don’t come at the cost of breaking what already works.  
It’s like a **safety net** — protecting the quality and reliability of your product after every change.

---
