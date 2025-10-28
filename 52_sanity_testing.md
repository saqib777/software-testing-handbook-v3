# Sanity Testing

### What is Sanity Testing?
Sanity Testing is a **quick, focused check** performed after receiving a software build to verify specific bug fixes or new functionality.  
It confirms that the targeted area works and that the build is stable enough for full testing.

---

### Why It’s Important
After small updates or bug fixes, you don’t need full regression testing.  
Sanity Testing helps:
- Quickly validate new or fixed functionality  
- Save time by testing only impacted areas  
- Ensure stability before full regression  

---

### Goals
- Verify recent bug fixes  
- Confirm that related features are not broken  
- Decide if full testing should proceed  

---

### Example
**Scenario:**  
A bug in the “Payment Page” is fixed. Testers check only that page and related checkout flow before resuming larger tests.

---

### Tools
- Selenium  
- Katalon Studio  
- TestComplete  
- Manual quick tests  

---

### Common Issues
- Confusion between smoke and sanity testing  
- Testing too many areas unnecessarily  
- Skipping sanity checks after small fixes  

---

### Best Practices
- Keep sanity test scope narrow  
- Run immediately after each build  
- Automate repeated sanity checks  

---

### Conclusion
Sanity Testing provides a **fast confidence check** after fixes or small updates, ensuring stability before more detailed testing.

---
