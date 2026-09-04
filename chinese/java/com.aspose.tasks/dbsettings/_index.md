---
title: "DbSettings"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许指定从项目数据库读取的设置。"
type: docs
weight: 75
url: /zh/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

允许指定从项目数据库读取的设置。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | 获取连接字符串。 |
| [getDriverClassName()](#getDriverClassName--) | 返回 JDBC 驱动程序类的名称。 |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | 设置连接字符串。 |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | 设置 JDBC 驱动程序类的名称。 |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


获取连接字符串。

**Returns:**
java.lang.String - 连接字符串。
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


返回 JDBC 驱动程序类的名称。默认的驱动程序类名是 "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - 驱动程序类字符串。
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


设置连接字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 连接字符串。 |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


设置 JDBC 驱动程序类的名称。默认的驱动程序类名是 "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | JDBC 驱动程序类的名称。 |

