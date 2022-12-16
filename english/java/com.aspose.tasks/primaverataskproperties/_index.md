---
title: PrimaveraTaskProperties
second_title: Aspose.Tasks for Java API Reference
description: Represents Primavera-specific properties for a task read from Primavera format XER of P6XML.
type: docs
weight: 185
url: /java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Represents Primavera-specific properties for a task read from Primavera format (XER of P6XML).
## Methods

| Method | Description |
| --- | --- |
| [getActivityId()](#getActivityId--) | Gets an activity id field - a task's unique identifier used by Primavera. |
| [getRawActivityType()](#getRawActivityType--) | Gets raw text representation (as in source file) of 'Activity Type' field of the activity. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Gets raw text representation (as in source file) of '% Complete Type' field of the activity. |
| [getRawDurationType()](#getRawDurationType--) | Gets raw text representation (as in source file) of 'Duration Type' field of the activity. |
| [getRawStatus()](#getRawStatus--) | Gets raw text representation (as in source file) of 'Status' field of the activity. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Gets remaining early finish date - the date when the remaining work for the activity is scheduled to be finished. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Gets remaining early start date - the date when the remaining work for the activity is scheduled to begin. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Gets remaining late finish date. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Gets remaining late start date. |
| [getSequenceNumber()](#getSequenceNumber--) | Gets the sequence number of the WBS item (summary tasks). |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Gets an activity id field - a task's unique identifier used by Primavera.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
java.lang.String - an activity id field - a task's unique identifier used by Primavera.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Gets raw text representation (as in source file) of 'Activity Type' field of the activity.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
java.lang.String - raw text representation (as in source file) of 'Activity Type' field of the activity.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Gets raw text representation (as in source file) of '% Complete Type' field of the activity.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
java.lang.String - raw text representation (as in source file) of '% Complete Type' field of the activity.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Gets raw text representation (as in source file) of 'Duration Type' field of the activity.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
java.lang.String - raw text representation (as in source file) of 'Duration Type' field of the activity.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Gets raw text representation (as in source file) of 'Status' field of the activity.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
java.lang.String - raw text representation (as in source file) of 'Status' field of the activity.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Gets remaining early finish date - the date when the remaining work for the activity is scheduled to be finished.

**Returns:**
java.util.Date - remaining early finish date - the date when the remaining work for the activity is scheduled to be finished.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Gets remaining early start date - the date when the remaining work for the activity is scheduled to begin.

**Returns:**
java.util.Date - remaining early start date - the date when the remaining work for the activity is scheduled to begin.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Gets remaining late finish date.

**Returns:**
java.util.Date - remaining late finish date.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Gets remaining late start date.

**Returns:**
java.util.Date - remaining late start date.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


Gets the sequence number of the WBS item (summary tasks). It is used to sort summary tasks in Primavera.

--------------------

Applicable to WBS items (summary tasks).

**Returns:**
int - the sequence number of the WBS item (summary tasks).