## Installation and Configuration Testing

### What is Installation and Configuration Testing?
Installation and Configuration Testing is done to make sure the software **installs, updates, uninstalls, and configures correctly** on all supported systems.  
In short — it’s checking whether users can set up your app easily and get it running without issues.

---

### Why is it Important?
Even the best application fails if it can’t be installed properly.  
This testing ensures:
- Smooth installation and setup  
- No missing files, crashes, or errors during installation  
- Proper working after updates or patches  
- Clean uninstallation without leftover data  

---

### Goals of Installation Testing
- Verify that installation steps complete without errors  
- Ensure the app runs correctly after installation  
- Check if updates install without breaking functionality  
- Confirm proper rollback if installation fails  
- Validate correct configuration options (like language, path, settings)

---

### Types of Installation Testing
1. **Clean Installation**  
   Installing the application on a fresh system where no previous version exists.

2. **Upgrade Installation**  
   Installing a new version over an older one to check compatibility and data preservation.

3. **Uninstallation Testing**  
   Ensuring that uninstalling removes all files, shortcuts, and registry entries.

4. **Patch Installation**  
   Testing smaller updates or fixes to confirm they apply correctly.

5. **Network Installation**  
   Verifying installation over a network or from a shared server.

---

### Common Issues Found
- Missing or corrupt files during setup  
- Installer not detecting previous versions  
- Application not launching after installation  
- Incorrect permissions or registry entries  
- Uninstaller leaving residual files or data  

---

### Tools Used
- **InstallShield**  
- **Inno Setup**  
- **NSIS (Nullsoft Scriptable Install System)**  
- **WiX Toolset**  
- **Advanced Installer**

---

### Best Practices
- Test on different OS versions and configurations  
- Simulate both successful and failed installations  
- Check installation under limited user permissions  
- Validate default paths and custom path options  
- Ensure rollback works correctly on failure  
- Verify system resources (disk space, memory) before and after installation  

---

### Example
**Scenario:** Installing an accounting software  
- Run the installer on Windows 10 and Windows 11  
- Choose both default and custom installation paths  
- Reboot system to check auto-start behavior  
- Uninstall and confirm all files
