---
share: "true"
---

When a license gets invalid, you can replace the old license with a new license. Replacing a license, combines the actions to retract the "old" license and then deploy the new license into a single step. However, you can replace only licenses that have the same [license type](License%20types.md) and the same [license mode](License%20modes.md) and that are of the same kind. If you maintain several runtime environments, you need to specify the environment for which you want to replace the license.

 >[!important]
 >Only admin users can delete licenses.

1. To replace a platform or activity license for a runtime environment, switch to the Process Modeler Licenses mode.
    
2. Import the new license.
    
3. From the **Actions** column, click ... and then **Deploy**.
    
4. Select the environment to which you want to deploy the license and sign in if you are not signed in yet.
    
5. Optionally, if the system finds a similar already deployed license with the same license mode, you can't just deploy the new license. Instead, you can merge the licenses or replace it with the new license. To replace the existing license, select **Replace** so that the **Retract License** window is displayed.
    
6. Click **OK**, to replace the old license that retracts the old and deploys the new license or click **CANCEL** to close the window without replacing the license.

