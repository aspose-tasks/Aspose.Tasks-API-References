---
title: PrimaveraSaveOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when saving project to Primavera XER format.
type: docs
weight: 207
url: /java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Allows to specify additional options when saving project to Primavera XER format.
## Constructors

| Constructor | Description |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | Initializes a new instance of the [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | Gets the increment used in renumbering of activity IDs. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | Gets the prefix used in renumbering of activity IDs. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | Gets the suffix used in renumbering of activity IDs. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | Gets a value indicating whether is need to renumbers activity IDs. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Gets a value indicating whether assignments of resources to summary tasks should be skipped during export. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | Sets the increment used in renumbering of activity IDs. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | Sets the prefix used in renumbering of activity IDs. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | Sets the suffix used in renumbering of activity IDs. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | Sets a value indicating whether is need to renumbers activity IDs. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Sets a value indicating whether assignments of resources to summary tasks should be skipped during export. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


Initializes a new instance of the [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) class.

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


Gets the increment used in renumbering of activity IDs.

**Returns:**
int - the increment used in renumbering of activity IDs.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


Gets the prefix used in renumbering of activity IDs.

**Returns:**
java.lang.String - the prefix used in renumbering of activity IDs.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


Gets the suffix used in renumbering of activity IDs.

**Returns:**
int - the suffix used in renumbering of activity IDs.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


Gets a value indicating whether is need to renumbers activity IDs.

**Returns:**
boolean - a value indicating whether is need to renumbers activity IDs.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Gets a value indicating whether assignments of resources to summary tasks should be skipped during export.

Primavera software doesn't support assignments of resources to summary (WBS) tasks. Thus, export of such assignments can result in an invalid file according to Primavera's model. If true, assignments to summary tasks are skipped during export. If false (the default value), an exception will be thrown if assignment to a summary task is encountered during export.

**Returns:**
boolean - a value indicating whether assignments of resources to summary tasks should be skipped during export.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


Sets the increment used in renumbering of activity IDs.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the increment used in renumbering of activity IDs. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


Sets the prefix used in renumbering of activity IDs.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the prefix used in renumbering of activity IDs. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


Sets the suffix used in renumbering of activity IDs.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the suffix used in renumbering of activity IDs. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


Sets a value indicating whether is need to renumbers activity IDs.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether is need to renumbers activity IDs. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Sets a value indicating whether assignments of resources to summary tasks should be skipped during export.

Primavera software doesn't support assignments of resources to summary (WBS) tasks. Thus, export of such assignments can result in an invalid file according to Primavera's model. If true, assignments to summary tasks are skipped during export. If false (the default value), an exception will be thrown if assignment to a summary task is encountered during export.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether assignments of resources to summary tasks should be skipped during export. |

