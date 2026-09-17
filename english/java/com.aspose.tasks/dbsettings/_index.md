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
| [getDriverClassName()](#getDriverClassName--) | Returns a name of JDBC driver class. |
| [getProjectLoadingCallback()](#getProjectLoadingCallback--) | Gets the callback to be invoked during project loading operations. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Sets the connection string. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | Sets a name of JDBC driver class. |
| [setProjectLoadingCallback(IProgressNotificationCallback value)](#setProjectLoadingCallback-com.aspose.tasks.IProgressNotificationCallback-) | Sets the callback to be invoked during project loading operations. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Gets the connection string.

**Returns:**
java.lang.String - the connection string.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


Returns a name of JDBC driver class. The default driver class name is "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - driver class string.
### getProjectLoadingCallback() {#getProjectLoadingCallback--}
```
public final IProgressNotificationCallback getProjectLoadingCallback()
```


Gets the callback to be invoked during project loading operations.

**Returns:**
[IProgressNotificationCallback](../../com.aspose.tasks/iprogressnotificationcallback) - the callback to be invoked during project loading operations.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Sets the connection string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the connection string. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


Sets a name of JDBC driver class. The default driver class name is "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a name of JDBC driver class. |

### setProjectLoadingCallback(IProgressNotificationCallback value) {#setProjectLoadingCallback-com.aspose.tasks.IProgressNotificationCallback-}
```
public final void setProjectLoadingCallback(IProgressNotificationCallback value)
```


Sets the callback to be invoked during project loading operations.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IProgressNotificationCallback](../../com.aspose.tasks/iprogressnotificationcallback) | the callback to be invoked during project loading operations. |

