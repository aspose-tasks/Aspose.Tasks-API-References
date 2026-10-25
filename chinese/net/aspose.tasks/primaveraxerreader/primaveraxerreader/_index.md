---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraXerReader 构造函数。初始化 PrimaveraXerReader 类的新实例。"
type: docs
weight: 10
url: /zh/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

初始化 [`PrimaveraXerReader`](../) 类的新实例。

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| xerFilePath | 字符串 | Primavera 项目或多个项目所在的 .xer 文件路径。 |

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

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

初始化 [`PrimaveraXerReader`](../) 类的新实例。

```csharp
public PrimaveraXerReader(Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 包含 Primavera XER 内容的流。 |

### 另见

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


