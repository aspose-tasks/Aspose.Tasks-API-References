---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraBaseReader 方法。加载具有指定唯一标识符的项目"
type: docs
weight: 30
url: /zh/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

加载具有指定唯一标识符的项目。

```csharp
public virtual Project LoadProject(int projectUid)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectUid | Int32 | 要加载的项目的唯一标识符。 |

### 返回值

从指定的多项目文件中获取具有指定唯一标识符的项目。如果项目不存在，则返回 Null。

## 示例

展示如何在已知项目 UID 时从 Primavera XML 文件加载项目。

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

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

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


