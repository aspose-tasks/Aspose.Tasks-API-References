---
title: MpdSettings
second_title: Aspose.Tasks for Java API Reference
description: Allows to set necessary options to read project data from MPD format MS Access database file format.
type: docs
weight: 155
url: /java/com.aspose.tasks/mpdsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MpdSettings extends DbSettings
```

Allows to set necessary options to read project data from MPD format (MS Access database file format).
## Constructors

| Constructor | Description |
| --- | --- |
| [MpdSettings(String connectionString, int projectId)](#MpdSettings-java.lang.String-int-) | Initializes a new instance of the `MpdSettings` class. |
## Methods

| Method | Description |
| --- | --- |
| [getProjectId()](#getProjectId--) | Returns id of the project to read. |
### MpdSettings(String connectionString, int projectId) {#MpdSettings-java.lang.String-int-}
```
public MpdSettings(String connectionString, int projectId)
```


Initializes a new instance of the `MpdSettings` class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| connectionString | java.lang.String | the specified connection string. |
| projectId | int | the specified id of a project to read. |

### getProjectId() {#getProjectId--}
```
public int getProjectId()
```


Returns id of the project to read.

**Returns:**
int - id of the project to read.
