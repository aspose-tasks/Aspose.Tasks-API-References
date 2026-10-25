---
title: "PrimaveraBaseReader"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示可用于从多项目 Primavera XER 或 XML 文件读取项目 UID 的基础读取器。"
type: docs
weight: 196
url: /zh/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

表示可用于从多项目 Primavera XER 或 XML 文件读取项目 UID 的基础读取器。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | 返回项目短信息对象的列表。 |
| [getProjectUids()](#getProjectUids--) | 返回项目唯一标识符的列表。 |
| [loadProject(int projectUid)](#loadProject-int-) | 加载具有指定唯一标识符的项目。 |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


返回项目短信息对象的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - 项目简要信息对象的列表
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


返回项目唯一标识符的列表。

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - 项目唯一标识符的列表。
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


加载具有指定唯一标识符的项目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectUid | int | 要加载的项目的唯一标识符。 |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
