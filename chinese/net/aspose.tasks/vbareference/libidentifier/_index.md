---
title: "VbaReference.LibIdentifier"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaReference 属性。获取库的标识符"
type: docs
weight: 20
url: /zh/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

获取库的标识符。

```csharp
public string LibIdentifier { get; }
```

## 示例

展示如何读取 VBA 引用。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### 另见

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


