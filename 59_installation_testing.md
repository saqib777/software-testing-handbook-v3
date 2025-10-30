# Installation Testing

### What is Installation Testing?
Installation Testing verifies that the software **installs, updates, and uninstalls correctly** in various environments.  
It ensures that setup processes are **smooth, complete, and error-free**.

---

### Why It’s Important
A product that doesn’t install properly can’t be used at all.  
Installation Testing ensures:
- Correct setup and configuration  
- All components and dependencies are installed  
- Clean uninstallation without leftover files  

---

### Goals
- Validate setup wizard and installer scripts  
- Check system compatibility during installation  
- Ensure version upgrades work smoothly  

---

### Example
**Scenario:**  
Testing a desktop application installer — verifying correct file paths, shortcuts, and registry entries are created, and that uninstallation removes them.

---

### Tools
- InstallShield  
- NSIS (Nullsoft Scriptable Install System)  
- Windows Installer (MSI)  
- Docker (for deployment validation)  

---

### Common Issues
- Missing dependencies or libraries  
- Wrong installation directory  
- Permission or access issues  
- Incomplete uninstall  

---

### Best Practices
- Test both fresh installs and upgrades  
- Simulate limited permissions or disk space  
- Validate rollback if installation fails  

---

### Conclusion
Installation Testing ensures your software can be **installed, updated, and removed easily** — without errors or leftover clutter.

---
