### Markdown (.md) Format

```markdown
# Activations

1. **Windows Activation (Massgrave)**
   ```powershell
   irm https://massgrave.dev/get | iex
   ```

2. **Windows Activation (Activated.win)**
   ```powershell
   irm https://get.activated.win | iex
   ```

# Utilities

1. **WinUtil**
   ```powershell
   irm https://christitus.com/win | iex
   ```

2. **Windows 10 Debloat**
   ```powershell
   iwr -useb https://git.io/debloat | iex
   ```

# Links

1. **All Windows Resources**
   - [tb.rg-adguard.net/public.php](https://tb.rg-adguard.net/public.php)

2. **Windows Server Dump**
   - [uupdump.net](https://uupdump.net)

3. **Mac Activation**
   - [massgrave.dev/office_for_mac](https://massgrave.dev/office_for_mac)

# Commands

1. **Install WingetUI**
   ```powershell
   winget install -e --id SomePythonThings.WingetUIStore
   ```

2. **Upgrade All Packages**
   ```powershell
   winget upgrade --all --accept-package-agreements
   ```

# SFC (System File Checker) Process

1. **Step 1: Run SFC /Scannow**
   ```powershell
   sfc /scannow
   ```

2. **Step 2: If Errors Found, Run DISM**
   ```powershell
   DISM /Online /Cleanup-Image /RestoreHealth
   ```

3. **Step 3: Run SFC /Scannow Again**
   ```powershell
   sfc /scannow
   ```
```

You can save these to `.txt` and `.md` files respectively. Let me know if you need any further adjustments!
