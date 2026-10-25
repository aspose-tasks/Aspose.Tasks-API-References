---
title: "PrimaveraDbReader"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示用于从 Primavera 数据库读取项目信息的读取器"
type: docs
weight: 200
url: /zh/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

表示用于从 Primavera 数据库读取项目信息的读取器
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | 初始化 [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | 加载具有指定唯一标识符的项目。 |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


初始化 [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | 指定如何连接到 Primavera DB 的设置。 |

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
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
