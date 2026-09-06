---
title: "VbaProject.References"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaProject 属性。获取 VbaReferenceCollection 集合"
type: docs
weight: 70
url: /zh/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

获取 [`VbaReferenceCollection`](../../vbareferencecollection/) 的集合。

```csharp
public VbaReferenceCollection References { get; }
```

## 示例

展示如何读取 VBA 项目引用信息。

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

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


