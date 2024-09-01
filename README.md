
---

# Windows Setup and Maintenance Guide

This guide provides essential commands and resources for activating, optimizing, and maintaining a Windows environment.

## Activations

1. **Windows Activation (Massgrave)**
   - Use this command to activate your Windows system:
   ```powershell
   irm https://massgrave.dev/get | iex
   ```

2. **Windows Activation (Activated.win)**
   - An alternative activation method:
   ```powershell
   irm https://get.activated.win | iex
   ```

## Utilities

1. **WinUtil**
   - A comprehensive utility tool for Windows customization:
   ```powershell
   irm https://christitus.com/win | iex
   ```

2. **Windows 10 Debloat**
   - Remove unnecessary bloatware from Windows 10:
   ```powershell
   iwr -useb https://git.io/debloat | iex
   ```

## Links

1. **All Windows Resources**
   - A broad collection of Windows resources:
     [tb.rg-adguard.net/public.php](https://tb.rg-adguard.net/public.php)

2. **Windows Server Dump**
   - Find Windows Server images and updates:
     [uupdump.net](https://uupdump.net)

3. **Mac Activation**
   - Activate Office for Mac:
     [massgrave.dev/office_for_mac](https://massgrave.dev/office_for_mac)

## Commands

1. **Install WingetUI**
   - Install a graphical user interface for managing packages via Winget:
   ```powershell
   winget install -e --id SomePythonThings.WingetUIStore
   ```

2. **Upgrade All Packages**
   - Upgrade all installed packages and accept agreements automatically:
   ```powershell
   winget upgrade --all --accept-package-agreements
   ```

## System Maintenance

### SFC (System File Checker) Process

1. **Step 1: Run SFC /Scannow**
   - Check for and repair corrupted system files:
   ```powershell
   sfc /scannow
   ```

2. **Step 2: If Errors Found, Run DISM**
   - Repair the Windows image to resolve deeper issues:
   ```powershell
   DISM /Online /Cleanup-Image /RestoreHealth
   ```

3. **Step 3: Run SFC /Scannow Again**
   - Re-run the System File Checker to ensure all issues are resolved:
   ```powershell
   sfc /scannow
   ```

### Windows Update Management

1. **Check for Updates**
   - Ensure your system is up-to-date:
   ```powershell
   wuauclt /detectnow
   ```

2. **Install Updates**
   - Install any pending updates:
   ```powershell
   Start-WindowsUpdate -Install
   ```

3. **Restart After Updates**
   - Restart the system if required after installing updates:
   ```powershell
   shutdown /r /t 0
   ```

---
