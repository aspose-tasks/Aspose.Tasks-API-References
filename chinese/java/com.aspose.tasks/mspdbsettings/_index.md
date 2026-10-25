---
title: "MspDbSettings"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许设置必要的选项以从 MS Project Server 数据库读取项目数据。"
type: docs
weight: 161
url: /zh/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

允许设置必要的选项以从 MS Project Server 数据库读取项目数据。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | 初始化 [MspDbSettings](../../com.aspose.tasks/mspdbsettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | 获取要读取的项目的 guid。 |
| [getSchema()](#getSchema--) | 获取 MS Project Server 的模式。 |
| [setSchema(String value)](#setSchema-java.lang.String-) | 设置 MS Project Server 的模式。 |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


初始化 [MspDbSettings](../../com.aspose.tasks/mspdbsettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| connectionString | java.lang.String | 指定的连接字符串。 |
| projectGuid | java.util.UUID | 指定要读取的项目的 guid。 |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


获取要读取的项目的 guid。

**Returns:**
java.util.UUID - 要读取的项目的 guid。
### getSchema() {#getSchema--}
```
public final String getSchema()
```


获取 MS Project Server 的模式。默认值为 "pub"。

**Returns:**
java.lang.String - MS Project Server 的模式。
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


设置 MS Project Server 的模式。默认值为 "pub"。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | MS Project Server 的模式。 |

