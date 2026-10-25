---
title: "MpdSettings"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许设置读取 MPD 格式 MS Access 数据库文件中项目数据所需的选项。"
type: docs
weight: 160
url: /zh/java/com.aspose.tasks/mpdsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MpdSettings extends DbSettings
```

允许设置必要的选项以从 MPD 格式（MS Access 数据库文件格式）读取项目数据。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [MpdSettings(String connectionString, int projectId)](#MpdSettings-java.lang.String-int-) | 初始化 `MpdSettings` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getProjectId()](#getProjectId--) | 返回要读取的项目的 id。 |
### MpdSettings(String connectionString, int projectId) {#MpdSettings-java.lang.String-int-}
```
public MpdSettings(String connectionString, int projectId)
```


初始化 `MpdSettings` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| connectionString | java.lang.String | 指定的连接字符串。 |
| projectId | int | 要读取的项目的指定 id。 |

### getProjectId() {#getProjectId--}
```
public int getProjectId()
```


返回要读取的项目的 id。

**Returns:**
int - 要读取的项目的 id。
