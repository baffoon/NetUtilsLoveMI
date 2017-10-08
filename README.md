# NetUtilsLoveMI

## Initial Description:

NetUtilsLoveMI is a little PowerShell prank that I cooked up. This will create a Microsoft.Powershell_profile file into an
individual's Documents\WindowsPowershell directory. It creates a function named NetUtilsLoveMI which is the Mission Impossible
theme and adds it to the user's profile. Then, it adds an alias for commonly used network utilities that point to the function in
the file.

## Getting it to run:

If you haven't already, it would be a good idea to set the execution policy so that you can run the script.

If the person's Execution Policy is Unrestricted, your good to go.

```PowerShell
PS C:\Users\$user> Get-ExecutionPolicy
Unrestricted
```

If their execution isn't Unrestricted, here is how to change that in an Administrative PowerShell Session.

```PowerShell
PS C:\WINDOWS\system32> Set-ExecutionPolicy -ExecutionPolicy Unrestricted

Execution Policy Change
The execution policy helps protect you from scripts that you do not trust. Changing the execution policy might expose you to the
security risks described in the about_Execution_Policies help topic at http://go.microsoft.com/fwlink/?LinkID=135170. Do you want to
change the execution policy?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): Y
PS C:\WINDOWS\system32> Get-ExecutionPolicy
Unrestricted
```

Now you should be able to run the script.

## If it doesn't work right away:

This will not work right away. If this script is being copied into a PowerShell session, you will need to open up a new
session and execute the aliass.
