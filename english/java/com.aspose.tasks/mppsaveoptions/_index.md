---
title: MPPSaveOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when saving project data to MPP.
type: docs
weight: 148
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
| [getClearVba()](#getClearVba--) | Gets a value indicating whether to remove existing VBA macros data when saving a project to MPP format. |
| [getProtectionPassword()](#getProtectionPassword--) | Gets a password which is used to protect a resulting MPP file. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | Gets a value indicating whether to remove invalid resource assignments when saving to MPP. |
| [getWriteFilters()](#getWriteFilters--) | Gets a value indicating whether to write filter data when saving a project to MPP for format. |
| [getWriteGroups()](#getWriteGroups--) | Gets a value indicating whether to write groups data when saving a project to MPP for format. |
| [getWriteVba()](#getWriteVba--) | Gets a value indicating whether to update existing VBA macros data in MPP file. |
| [getWriteViewData()](#getWriteViewData--) | Gets a value indicating whether to write view data when saving a project to MPP format. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | Sets a value indicating whether to remove existing VBA macros data when saving a project to MPP format. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | Sets a password which is used to protect a resulting MPP file. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | Sets a value indicating whether to remove invalid resource assignments when saving to MPP. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | Sets a value indicating whether to write filter data when saving a project to MPP for format. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | Sets a value indicating whether to write groups data when saving a project to MPP for format. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | Sets a value indicating whether to update existing VBA macros data in MPP file. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | Sets a value indicating whether to write view data when saving a project to MPP format. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


Initializes a new instance of the [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) class.

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


Gets a value indicating whether to remove existing VBA macros data when saving a project to MPP format.

**Returns:**
boolean - a value indicating whether to remove existing VBA macros data when saving a project to MPP format.
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


Gets a value indicating whether to write filter data when saving a project to MPP for format.

--------------------

Filter data includes Project.TaskFilters and Project.ResourceFilters collections.

--------------------

Currently supported for MSP 2010 or newer formats.

**Returns:**
boolean - a value indicating whether to write filter data when saving a project to MPP for format.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


Gets a value indicating whether to write groups data when saving a project to MPP for format.

--------------------

Group data includes Project.TaskGroups and Project.ResourceGroups collections.

**Returns:**
boolean - a value indicating whether to write groups data when saving a project to MPP for format.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


Gets a value indicating whether to update existing VBA macros data in MPP file. Currently writing of VbaModule.SourceCode is supported.

**Returns:**
boolean - a value indicating whether to update existing VBA macros data in MPP file.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


Gets a value indicating whether to write view data when saving a project to MPP format.

--------------------

View data includes Project.Views, Filters and Tables collections.

**Returns:**
boolean - a value indicating whether to write view data when saving a project to MPP format.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


Sets a value indicating whether to remove existing VBA macros data when saving a project to MPP format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to remove existing VBA macros data when saving a project to MPP format. |

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


Sets a value indicating whether to write filter data when saving a project to MPP for format.

--------------------

Filter data includes Project.TaskFilters and Project.ResourceFilters collections.

--------------------

Currently supported for MSP 2010 or newer formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to write filter data when saving a project to MPP for format. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


Sets a value indicating whether to write groups data when saving a project to MPP for format.

--------------------

Group data includes Project.TaskGroups and Project.ResourceGroups collections.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to write groups data when saving a project to MPP for format. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


Sets a value indicating whether to update existing VBA macros data in MPP file. Currently writing of VbaModule.SourceCode is supported.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to update existing VBA macros data in MPP file. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


Sets a value indicating whether to write view data when saving a project to MPP format.

--------------------

View data includes Project.Views, Filters and Tables collections.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to write view data when saving a project to MPP format. |

