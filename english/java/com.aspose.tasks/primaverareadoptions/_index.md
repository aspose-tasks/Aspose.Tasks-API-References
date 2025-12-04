---
title: PrimaveraReadOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when reading Primavera Xml or Primavera Xer files.
type: docs
weight: 205
url: /java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Allows to specify additional options when reading Primavera Xml or Primavera Xer files.
## Constructors

| Constructor | Description |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | Initializes a new instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | Gets a flag that specifies whether original unique identifiers of entities should be preserved. |
| [getProjectUid()](#getProjectUid--) | Gets the UID of a project to read from file containing multiple projects. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | Gets a flag that specifies whether baseline projects should be loaded. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | Specifies the behavior used to process tasks with undefined constraints read from XER format. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | Sets a flag that specifies whether original unique identifiers of entities should be preserved. |
| [setProjectUid(int value)](#setProjectUid-int-) | Sets the UID of a project to read from file containing multiple projects. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | Sets a flag that specifies whether baseline projects should be loaded. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | Specifies the behavior used to process tasks with undefined constraints read from XER format. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


Initializes a new instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class.

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


Gets a flag that specifies whether original unique identifiers of entities should be preserved.

**Returns:**
boolean - a flag that specifies whether original unique identifiers of entities should be preserved.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


Gets the UID of a project to read from file containing multiple projects.

**Returns:**
int - the UID of a project to read from file containing multiple projects.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


Gets a flag that specifies whether baseline projects should be loaded. The default value is true.

--------------------

The flag is applicable to Primavera XML files containing baseline projects (baselines are not supported by XER format). The option can be set to false to speed up loading of a large project with baselines when baseline data is not needed.

**Returns:**
boolean - a flag that specifies whether baseline projects should be loaded.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


Specifies the behavior used to process tasks with undefined constraints read from XER format.

**Returns:**
int - the behavior used to process tasks with undefined constraints read from XER format.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


Sets a flag that specifies whether original unique identifiers of entities should be preserved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a flag that specifies whether original unique identifiers of entities should be preserved. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


Sets the UID of a project to read from file containing multiple projects.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the UID of a project to read from file containing multiple projects. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


Sets a flag that specifies whether baseline projects should be loaded. The default value is true.

--------------------

The flag is applicable to Primavera XML files containing baseline projects (baselines are not supported by XER format). The option can be set to false to speed up loading of a large project with baselines when baseline data is not needed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a flag that specifies whether baseline projects should be loaded. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


Specifies the behavior used to process tasks with undefined constraints read from XER format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the behavior used to process tasks with undefined constraints read from XER format. |

