---
title: "类 VbaModuleAttributeCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.VbaModuleAttributeCollection 类。表示 VbaModuleAttribute 对象的集合"
type: docs
weight: 2830
url: /zh/net/aspose.tasks/vbamoduleattributecollection/
---
## VbaModuleAttributeCollection class

表示一个 [`VbaModuleAttribute`](../vbamoduleattribute/) 对象的集合。

```csharp
public class VbaModuleAttributeCollection : ReadOnlyCollectionBase<VbaModuleAttribute>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModuleAttribute) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## 示例

展示如何遍历 VBA 模块的属性集合。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("Attribute Name: " + attribute.Key);
        Console.WriteLine("Attribute Value: " + attribute.Value);
    }
}
```

### 另见

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModuleAttribute](../vbamoduleattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


