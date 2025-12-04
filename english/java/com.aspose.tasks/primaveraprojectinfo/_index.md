---
title: PrimaveraProjectInfo
second_title: Aspose.Tasks for Java API Reference
description: Represents short info about a project loaded from Primavera format.
type: docs
weight: 203
url: /java/com.aspose.tasks/primaveraprojectinfo/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectInfo
```

Represents short info about a project loaded from Primavera format.
## Methods

| Method | Description |
| --- | --- |
| [getExportFlag()](#getExportFlag--) | Gets project's export flag. |
| [getName()](#getName--) | Gets project's name. |
| [getShortName()](#getShortName--) | Gets project's short name (Project ID). |
| [getUid()](#getUid--) | Gets project's Uid. |
### getExportFlag() {#getExportFlag--}
```
public final boolean getExportFlag()
```


Gets project's export flag. When a project is selected for export in Primavera, its ExportFlag is true. Some projects not explicitly selected for export may be exported to an XER file due to their relationship to the exported project.

**Returns:**
boolean - project's export flag.
### getName() {#getName--}
```
public final String getName()
```


Gets project's name.

**Returns:**
java.lang.String - project's name.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Gets project's short name (Project ID).

**Returns:**
java.lang.String - project's short name (Project ID).
### getUid() {#getUid--}
```
public final int getUid()
```


Gets project's Uid.

**Returns:**
int - project's Uid.
