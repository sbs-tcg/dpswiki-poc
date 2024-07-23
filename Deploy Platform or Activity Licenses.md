---
share: "true"
---

You can deploy any platform or activity license from your license pool to one of the available runtime environments. However, you first import the license to the license pool and then you can deploy it. You do not have to deploy a design-time license. This is valid after the import. For a password design-time license, you can assign the license to a process as needed after import.

You can deploy only one license of each license mode. That means, one one-time and one renewable license with or with out grace volume. When you deploy a license to a runtime and there is a license that has the same mode already deployed on the system, you get the option to merge these licenses, to replace the already-deployed license, or to merge and replace the license.

>[!important] Important
>Only administrator users can maintain licenses

1. To deploy a platform or activity license to your runtime environment, switch to the Process Modeler **Licenses** mode. If the runtime is not available in Process Modeler yet, switch **Environments** mode and register a runtime environment so that you then can deploy a license.
    
2. Select the license you want to deploy from the list of available platform or activity licenses.

>[!note]
 >You can deploy only licenses that have the status _Available_. If a license is already deployed, you first have to retract so that you can deploy it to a different environment. However, you can deploy licenses only to a registered runtime.
    
3. From the Actions column, click ... then **Deploy** from the context menu. The **Select environment** window is displayed.
    
4. Select the environment you want to deploy the license to and click **OK** window or click **CANCEL** to close the window without deploying the license.
    
5. If you are not signed-in to the environment already, you need to sign in first and then the **Deploy license** window is displayed.
    
6. Click **OK**, to deploy the license to the runtime environment or **CANCEL** to close the window.

