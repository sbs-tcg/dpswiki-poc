---
share: "true"
---

If you have several licenses deployed to the same runtime environment, the licenses are used in a specific order, which depends on the [license mode](License%20modes.md).

1- Renewable license
2- One-time license
3- Grace volume

>[!example] Example
You have a renewable license with a grace volume and a one-time license.
First, the counters of the renewable license are decreased until the [volume counter](volume%20counter.md) hits zero and the license is invalidated. 
After that, the counters of the one-time license are decreased until depleted.
Finally, if the one-time license is invalidated, the grace volume of the renewable license is decreased.

A license is invalidated if **ONE** of its license counts exceeds that means when the counter for work items, documents or pages is zero. So, if the page counter is used up, a license gets invalid, even if the counters for work items and documents are still greater than zero.

In general, two of the Primus runtime services, the [Process Service](Process%20Service.md) and the [Document Service](Document%20Service.md) reduce the license counters. The Process Service counts [work items](Work%20Item%20(object%20type).md) whereas the Document Service counts [media](Media%20(Object%20type).md) and [pages](Page%20(Object%20type).md). 

By default, the Primus runtime services are hosted as individual Windows services and there is no specific order which service reduces the counters first. The service that comes first reduces the counters on a valid license. As soon as one license counter of a license is exceeded, the complete license gets invalid, independent whether the license has other counters remaining. The next service that reduces license counters picks the next available valid license and reduces the counters on that license. 

>[!example] Example
>If the Document Service uses up the page counter for a renewable license, the license gets invalidated. If the Process service then updates the license counters, this service uses the next valid license, for example, a one-time license and reduces the work item counter on that license even though the invalid renewable license has work item licenses remaining.

