---
title: DbSettings
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify settings to read from project database.
type: docs
weight: 75
url: /java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

Allows to specify settings to read from project database.
## Methods

| Method | Description |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | Gets the connection string. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Sets the connection string. |
| [getDriverClassName()](#getDriverClassName--) | Returns a name of JDBC driver class. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | Sets a name of JDBC driver class. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Gets the connection string.

**Returns:**
java.lang.String - the connection string.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Sets the connection string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the connection string. |

### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


Returns a name of JDBC driver class. The default driver class name is "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - driver class string.
### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


Sets a name of JDBC driver class. The default driver class name is "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a name of JDBC driver class. |

