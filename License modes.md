---
share: "true"
---


For design-time licenses, we distinguish between system and password licenses. For runtime licenses, platform and activity, there are one-time and renewable licenses.

### System

A system license defines the number of environments that you can maintain as well as the number of processes and activities that you can create and publish. For the number of processes, the platform considers only the activities of the last publish process version.

### Password

A password license is a specific design-time license that allows you to display and modify a process with its activity settings only when entering a password. Also for importing a password-protected process, you require a password, otherwise a user can't import the process. You can [create one or more passwords for a process](Password-protect%20a%20process.md). 

The first password that you enter is the administrator password. However, you can also configure additional passwords as needed. When you export a password-protected process, you have to provide an additional password for the created archive. When you import the process, you then have to provide the archive-password. To modify the process, you either enter the Administrator or one of the additional passwords, if available.  

A password license can either protect all processes or specific processes only. For a license for specific processes, you need to provide the process type GUID of the processes that you want to protect. For example, in the license request, you can enter the process type GUIDs in the description area.

### One-Time

A one-time license exceeds after one of the volume counters is exceeded and can not be extended. The license can have an expiration date that means that the license gets invalid after the date is reached independent from its license counters.

### Renewable and Renewable with Grace

For a renewable license, the volume counters are set back to the initial maximum volume count every year on January, 1st at 0:00 am. However, when one of the license counters exceeds, the license gets invalid and cannot be used for processing. On the renewal date, the counters are reset and the license is valid again. For example, if you have a license with 10000 pages and you have processed 10000 pages until December, 24th, the license gets invalid until the January, 1st.

For a renewable license, you can have a grace volume that is a certain percentage of the maximum volume count. The grace volume is volume that you can use in advance from the volume of the next year. The platform uses the grace volume when the license counter for the current year expires. For example, if you have 10% grace volume for a 10000 pages license, you can process another 1000 pages when the current license counter exceeds. When the license renews for the next year, the number of processed pages from the grace volume are then counted as already "used" volume.