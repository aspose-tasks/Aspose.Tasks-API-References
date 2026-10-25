---
title: "PrimaveraDbSettings"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许设置读取 Primavera 数据库中项目数据所需的选项。"
type: docs
weight: 201
url: /zh/java/com.aspose.tasks/primaveradbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class PrimaveraDbSettings extends DbSettings
```

允许设置读取 Primavera 数据库中项目数据所需的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PrimaveraDbSettings(String connectionString, int projectId)](#PrimaveraDbSettings-java.lang.String-int-) | 初始化一个新的 [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getProjectId()](#getProjectId--) | 获取要读取的项目的 id。 |
### PrimaveraDbSettings(String connectionString, int projectId) {#PrimaveraDbSettings-java.lang.String-int-}
```
public PrimaveraDbSettings(String connectionString, int projectId)
```


初始化一个新的 [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) 类实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| connectionString | java.lang.String | 指定的连接字符串。 |
| projectId | int | 要读取的项目的指定 id。 |

### getProjectId() {#getProjectId--}
```
public final int getProjectId()
```


获取要读取的项目的 id。

**Returns:**
int - 要读取的项目的 id。
