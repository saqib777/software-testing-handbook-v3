## Integration Testing

### What is Integration Testing?
Integration Testing checks **how different modules or components work together**.  
It focuses on interactions between units that have already passed unit testing.

---

### Why It’s Important
Even if individual modules work fine, problems can occur when they interact.  
Integration Testing ensures:
- Data flows correctly between modules  
- Interfaces and APIs connect properly  
- No mismatched formats or logic errors  

---

### Goals
- Validate module communication  
- Detect interface defects early  
- Ensure combined functionality works  

---

### Example
**Scenario:**  
Testing how the payment module interacts with the order module and database after a transaction.

---

### Approaches
- **Big Bang:** Test everything together at once  
- **Incremental:** Test step by step (Top-Down or Bottom-Up)  

---

### Tools
- JUnit / TestNG  
- Postman  
- Selenium (for UI-level integration)  

---

### Common Issues
- Incompatible data formats  
- Missing APIs or wrong endpoints  
- Integration delays or failures  

---

### Best Practices
- Test interfaces early  
- Use stubs and drivers for unavailable components  
- Automate frequent integration flows  

---

### Conclusion
Integration Testing ensures **smooth cooperation between modules**, reducing surprises during system testing.

---
