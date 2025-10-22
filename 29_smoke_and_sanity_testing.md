## Smoke and Sanity Testing

### What is Smoke Testing?
Smoke Testing is a **quick, initial check** to verify that the basic and most important functions of an application work correctly.  
It’s like turning on a new device for the first time — you just check if it powers up and the main features run without crashing.

**Example:**  
After a new build, testers quickly check if login, homepage, and basic navigation work.  
If these fail, there’s no point testing further — the build is rejected.

---

### Why is Smoke Testing Important?
- Saves time by catching major issues early  
- Prevents wasting effort on unstable builds  
- Ensures the build is ready for deeper testing  
- Helps maintain stable integration between modules  

---

### When is Smoke Testing Done?
- After every new build release  
- Before starting functional or regression testing  
- During CI/CD pipelines after code merges  

---

### What is Sanity Testing?
Sanity Testing is a **focused check** done after minor code changes or bug fixes to verify that specific functionalities work as expected.  
In short — it’s a narrow and deep test to confirm that the “fixed” area is actually working now.

**Example:**  
If a developer fixes a login issue, testers will run a sanity test only on the login module to ensure the issue is resolved — not on the whole application.

---

### Why is Sanity Testing Important?
- Confirms that recent changes didn’t break existing functionality  
- Saves time by testing only affected areas  
- Acts as a quick validation before full regression testing  

---

### Key Differences Between Smoke and Sanity Testing

| Aspect | Smoke Testing | Sanity Testing |
|--------|----------------|----------------|
| **Purpose** | To check if the build is stable for testing | To verify specific fixes or changes |
| **Scope** | Broad and shallow | Narrow and deep |
| **Performed on** | New builds | Modified builds |
| **Focus** | Overall system stability | Particular functionality |
| **Automation** | Often automated | Usually manual |
| **Outcome** | Accept or reject the build | Decide whether to proceed with detailed testing |

---

### Common Issues Found
- Application not launching or crashing at startup  
- Login or core functionality failures  
- Missing majo
