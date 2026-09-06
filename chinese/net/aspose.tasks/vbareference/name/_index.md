---
title: "VbaReference.Name"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaReference 属性。获取或设置 VBA 引用的名称"
type: docs
weight: 30
url: /zh/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

获取或设置 VBA 引用的名称。

```csharp
public string Name { get; set; }
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


