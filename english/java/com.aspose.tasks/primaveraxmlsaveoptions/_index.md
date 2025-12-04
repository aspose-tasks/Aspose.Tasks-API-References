---
title: PrimaveraXmlSaveOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when saving project to Primavera xml format.
type: docs
weight: 211
url: /java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Allows to specify additional options when saving project to Primavera xml format.
## Constructors

| Constructor | Description |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | Initializes a new instance of the [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | Gets a value indicating whether to save a root task or not. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Gets a value indicating whether assignments of resources to summary tasks should be skipped during export. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | Sets a value indicating whether to save a root task or not. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Sets a value indicating whether assignments of resources to summary tasks should be skipped during export. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


Initializes a new instance of the [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) class.

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


Gets a value indicating whether to save a root task or not.

**Returns:**
boolean - a value indicating whether to save a root task or not.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Gets a value indicating whether assignments of resources to summary tasks should be skipped during export.

Primavera software doesn't support assignments of resources to summary (WBS) tasks. Thus, export of such assignments can result in an invalid file according to Primavera's model. If true, assignments to summary tasks are skipped during export. If false (the default value), an exception will be thrown if assignment to a summary task is encountered during export.

**Returns:**
boolean - a value indicating whether assignments of resources to summary tasks should be skipped during export.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


Sets a value indicating whether to save a root task or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to save a root task or not. |

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

