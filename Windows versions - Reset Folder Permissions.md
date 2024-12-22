## Option 1: Verify Ownership and Permissions
Right-click the "Documents" folder, select Properties, then go to the Security tab.

Click Advanced to open the Advanced Security Settings.

Check the Owner at the top. If your account isn't listed, click Change next to "Owner."

Type your account name, click Check Names, and click OK.
Check Replace owner on subcontainers and objects and click Apply.
Ensure your account has Full Control:

Back in the Security tab, select your account name.
Click Edit, ensure Full Control is checked, and click Apply.

## Option 2: Reset Folder Permissions

The issue can occur on Windows 11 due to file or folder permission problems, corruption in the user profile, or interference from system settings. Here are some steps to troubleshoot and resolve the issue:

Run a command in PowerShell to reset permissions for the Documents folder:

NOTE: Open PowerShell as Administrator.

```icacls "C:\Users\YourUsername\Documents" /reset /t /c /q```
