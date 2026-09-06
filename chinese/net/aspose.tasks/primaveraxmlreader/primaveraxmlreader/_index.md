---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraXmlReader 构造函数。初始化 PrimaveraXmlReader 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

初始化一个新的 [`PrimaveraXmlReader`](../) 类的实例。

```csharp
public PrimaveraXmlReader(string templatePath)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| templatePath | 字符串 | 模板的路径，Primavera Xml 项目或项目所在的位置 |

## 示例

展示如何从 Primavera XML 文件检查短项目的信息。

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### 另见

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

初始化一个新的 [`PrimaveraXmlReader`](../) 类的实例。

```csharp
public PrimaveraXmlReader(Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 包含 Primavera Xml 内容的流。 |

## 示例

展示如何从 Primavera XML 流导入项目。

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### 另见

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


