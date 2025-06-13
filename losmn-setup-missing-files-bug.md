# Installation Error 456: Missing setup.exe/continuesetup.dll on Multiple LOSMN Machines (LightOS 2.0 build 0001)

**Summary:**  
During installation of LightOS 2.0 build 0001 on several LOSMN-series machines, the installer abruptly restarts and/or displays the following error:  
**Error 456: could not find setup.exe/continuesetup.dll.**  
This prevents successful installation on the affected hardware.

**Affected Machines:**  
- LOSMN-2000  
- LOSMN-1999  
- LOSMN-1998  
- LOSMN-1997  
- LOSMN-1996  

**Steps to Reproduce:**  
1. Boot any of the affected machines from LightOS 2.0 build 0001 installation media.  
2. Begin installation process.  
3. At an early stage (uncertain exact step), the installer abruptly restarts or fails.  
4. Error displayed: `Error 456: could not find setup.exe/continuesetup.dll.`

**Expected Behavior:**  
Installer should proceed normally and complete installation without missing file errors.

**Actual Behavior:**  
Installer fails with Error 456, indicating missing setup.exe or continuesetup.dll, and may restart unexpectedly.

**Additional Info:**  
- Issue is consistent across all listed hardware.
- No further diagnostic info, logs, or screenshots available at this time.
- Error occurs regardless of installation media type (USB, DVD, etc.).

**Impact:**  
Prevents installation of LightOS 2.0 build 0001 on all listed LOSMN models, blocking OS deployment.

**Suggested Actions:**  
- Investigate missing or corrupted installer files in build 0001.
- Check setup media creation and integrity.
- Provide updated installation media or patch if files are missing or installer is referencing incorrect paths.

_Reported by honzik233 to LightOS.Inc_