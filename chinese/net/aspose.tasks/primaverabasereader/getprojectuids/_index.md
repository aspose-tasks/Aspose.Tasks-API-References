---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraBaseReader 方法。返回项目唯一标识符的列表"
type: docs
weight: 20
url: /zh/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

返回项目唯一标识符的列表。

```csharp
public List<int> GetProjectUids()
```

### 返回值

项目唯一标识符列表。

## 示例

展示如何从 Primavera XML 文件导入项目。

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### 另见

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


