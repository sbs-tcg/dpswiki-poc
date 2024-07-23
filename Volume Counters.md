---
share: "true"
---


A volume counter sums the total number of created or processed work items, documents, pages, and media. In general for a runtime license, one volume counter only is set to a maximum number that you can process. All other counters are set then to _unlimited_.

![z-license counters.png](z-license%20counters.png)

During processing, the platform decrements the configured counter for each processed item, which can either be a work item, a document, a page, or a media. It also takes care that the activity volume counter are decremented. Which counter an activity license requires depends on the activity. For further information also refer to the activity help.

### Invalidating a license

A license is invalidated when **ONE** of its volume counters exceeds its limit. It can then no longer be used to process your work items, even if the license contains other counters that have volume counters remaining.

In addition, a license can have an expiration date and gets invalid when the date is exceeded.

