---
title: "类 PrimaveraDbReader"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.PrimaveraDbReader 类。表示用于从 Primavera DB 读取项目信息的读取器。"
type: docs
weight: 1350
url: /zh/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

表示用于从 Primavera 数据库读取项目信息的读取器

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | 初始化 [`PrimaveraXerReader`](../primaveraxerreader/) 类的新实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | 返回项目的简短信息对象列表。 |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | 返回项目唯一标识符的列表。 |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | 加载具有指定唯一标识符的项目。 |

## 示例

展示如何从 Primavera 数据库获取项目的简要信息。

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### 另见

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


