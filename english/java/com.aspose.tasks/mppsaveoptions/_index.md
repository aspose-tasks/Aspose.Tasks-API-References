---
title: MPPSaveOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when saving project data to MPP.
type: docs
weight: 144
url: /java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

Allows to specify additional options when saving project data to MPP.
## Constructors

| Constructor | Description |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | Initializes a new instance of the [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getProtectionPassword()](#getProtectionPassword--) | Gets a password which is used to protect a resulting MPP file. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | Gets a value indicating whether to remove invalid resource assignments when saving to MPP. |
| [getWriteFilters()](#getWriteFilters--) | Gets a value indicating whether to write filter data when saving to MPP. |
| [getWriteViewData()](#getWriteViewData--) | Gets a value indicating whether to write view data when saving to MPP. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | Sets a password which is used to protect a resulting MPP file. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | Sets a value indicating whether to remove invalid resource assignments when saving to MPP. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | Sets a value indicating whether to write filter data when saving to MPP. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | Sets a value indicating whether to write view data when saving to MPP. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


Initializes a new instance of the [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) class.

### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


Gets a password which is used to protect a resulting MPP file. Currently is supported for MS Project 2010 and newer formats.

--------------------

Null value indicates that the project file is not protected.

**Returns:**
java.lang.String - a password which is used to protect a resulting MPP file.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


Gets a value indicating whether to remove invalid resource assignments when saving to MPP.

--------------------

MS Project creates an empty resource assignment for each task. Set this flag to true to remove them on save.

**Returns:**
boolean - a value indicating whether to remove invalid resource assignments when saving to MPP.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


Gets a value indicating whether to write filter data when saving to MPP.

--------------------

Filter data includes Project.TaskFilters and Project.ResourceFilters collections.

--------------------

Currently supported for MSP 2010 or newer formats.

**Returns:**
boolean - a value indicating whether to write filter data when saving to MPP.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


Gets a value indicating whether to write view data when saving to MPP.

--------------------

View data includes Project.Views, Filters and Tables collections.

**Returns:**
boolean - a value indicating whether to write view data when saving to MPP.
### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


Sets a password which is used to protect a resulting MPP file. Currently is supported for MS Project 2010 and newer formats.

--------------------

Null value indicates that the project file is not protected.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a password which is used to protect a resulting MPP file. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


Sets a value indicating whether to remove invalid resource assignments when saving to MPP.

--------------------

MS Project creates an empty resource assignment for each task. Set this flag to true to remove them on save.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to remove invalid resource assignments when saving to MPP. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


Sets a value indicating whether to write filter data when saving to MPP.

--------------------

Filter data includes Project.TaskFilters and Project.ResourceFilters collections.

--------------------

Currently supported for MSP 2010 or newer formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to write filter data when saving to MPP. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


Sets a value indicating whether to write view data when saving to MPP.

--------------------

View data includes Project.Views, Filters and Tables collections.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to write view data when saving to MPP. |

