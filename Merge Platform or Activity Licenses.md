---
share: "true"
---

You can merge licenses that have the same type, the same grace volume, and the same unlimited volume counters. That means you cannot merge two license when one license has unlimited documents and 10.000 pages and the either license has 100.000 documents and unlimited pages. If the licenses have different expiration dates, the merged license gets the expiration date that expires first.

You can merge licenses only that have the status **Available**. If needed, you can retract the license from an environment and merge it then.

 >[!important]
 >The ability to split or merge a license is license-specific. This feature is enabled when the license is created. The shortcut in the toolbar is displayed only, if the selected license has this feature enabled. Only admin users can maintain licenses.

1. To merge two platform or activity licenses, switch to the Process Modeler License Management mode.
    
2. Select the licenses you want to merge from the list of available platform licenses. You can merge only licenses that have the status **Available**.
    
3. From the **Actions** column, click ... from the Actions columns and then **Merge** from the context menu. The **Merge Licenses** window is displayed and shows the name and the volume counters for the merged license. Adjust the provided settings by changing the name of the resulting license for Merged License columns and the volume counters accordingly.
    
4. By default, when the licenses to be merged have different expiration dates, the new license gets the lower expiration date. That you do not merge the licenses by accident, you have to confirm that the lower expiration date is taken by selecting the **Use lower expiration date** option. When selected, the **OK** button gets enabled.
    
5. Click **OK** to create from the original license two new licenses or **CANCEL** to close the window.

