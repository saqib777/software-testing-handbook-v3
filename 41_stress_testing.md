# Stress Testing

### What is Stress Testing?
Stress Testing checks how software behaves **beyond its normal limits** — when traffic, data, or usage suddenly spikes.  
The goal is to identify **the breaking point** and see how gracefully the system recovers after failure.

---

### Why It’s Important
Systems should fail predictably, not catastrophically.  
Stress Testing ensures:
- Stability under extreme conditions  
- Proper error handling when overloaded  
- Graceful recovery after crashes  

---

### Goals
- Find system limits and weak points  
- Test recovery mechanisms  
- Prevent total system failure under peak load  

---

### Example
Simulating 50,000 users trying to log in simultaneously to a banking app to test stability and recovery time.

---

### Tools
- JMeter  
- LoadNinja  
- Locust  
- BlazeMeter  

---

### Common Issues
- Server crashes or hangs  
- Memory exhaustion  
- Data loss during overload  
- Long recovery times  

---

### Best Practices
- Gradually increase load to observe behavior  
- Monitor for slowdowns and failure points  
- Test post-failure recovery  
- Document maximum capacity limits  

---

### Conclusion
Stress Testing ensures that your system **handles extreme conditions** gracefully, without complete failure or data loss.

---
