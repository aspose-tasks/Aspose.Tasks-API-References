---
title: MspDbSettings
second_title: Aspose.Tasks for Java API Reference
description: Allows to set necessary options to read project data from MS Project Server database.
type: docs
weight: 160
url: /java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

Allows to set necessary options to read project data from MS Project Server database.
## Constructors

| Constructor | Description |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | Initializes a new instance of the [MspDbSettings](../../com.aspose.tasks/mspdbsettings) class. |
## Methods

| Method | Description |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | Gets the guid of the project to read. |
| [getSchema()](#getSchema--) | Gets the schema of the MS Project Server. |
| [setSchema(String value)](#setSchema-java.lang.String-) | Sets the schema of the MS Project Server. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


Initializes a new instance of the [MspDbSettings](../../com.aspose.tasks/mspdbsettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| connectionString | java.lang.String | the specified connection string. |
| projectGuid | java.util.UUID | the specified guid of a project to read. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Gets the guid of the project to read.

**Returns:**
java.util.UUID - the guid of the project to read.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


Gets the schema of the MS Project Server. The default value is "pub".

**Returns:**
java.lang.String - the schema of the MS Project Server.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


Sets the schema of the MS Project Server. The default value is "pub".

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the schema of the MS Project Server. |

