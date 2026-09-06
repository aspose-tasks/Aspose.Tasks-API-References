---
title: "类 PrimaveraXerReader"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.PrimaveraXerReader 类。表示用于从 Primavera XER 文件读取项目 UID 的读取器"
type: docs
weight: 1390
url: /zh/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

表示用于从 Primavera XER 文件读取项目 UID 的读取器

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | 初始化 `PrimaveraXerReader` 类的新实例。 |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | 初始化 `PrimaveraXerReader` 类的新实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | 返回项目的简短信息对象列表。 |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | 返回项目唯一标识符的列表。 |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | 加载具有指定唯一标识符的项目。 |

## 示例

展示如何从 Primavera XER 文件检查简短项目的信息。

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### 另见

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


