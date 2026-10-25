---
title: "类 VbaReferenceCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.VbaReferenceCollection 类。表示 VbaReference 对象的集合"
type: docs
weight: 2880
url: /zh/net/aspose.tasks/vbareferencecollection/
---
## VbaReferenceCollection class

表示 [`VbaReference`](../vbareference/) 对象的集合。

```csharp
public class VbaReferenceCollection : ReadOnlyCollectionBase<VbaReference>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaReference) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## 示例

展示如何使用 VBA 引用集合。

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

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaReference](../vbareference/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


