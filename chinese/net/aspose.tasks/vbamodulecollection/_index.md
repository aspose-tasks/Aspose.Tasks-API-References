---
title: "类 VbaModuleCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.VbaModuleCollection 类。表示 VbaModule 对象的集合"
type: docs
weight: 2840
url: /zh/net/aspose.tasks/vbamodulecollection/
---
## VbaModuleCollection class

表示一个 [`VbaModule`](../vbamodule/) 对象的集合。

```csharp
public class VbaModuleCollection : ICollection<VbaModule>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/vbamodulecollection/count/) { get; } |  |
| [IsReadOnly](../../aspose.tasks/vbamodulecollection/isreadonly/) { get; } |  |
| [Item](../../aspose.tasks/vbamodulecollection/item/) { get; } | 获取指定索引处的模块。（2 个索引器） |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/vbamodulecollection/add/)(VbaModule) |  |
| [Clear](../../aspose.tasks/vbamodulecollection/clear/)() |  |
| [Contains](../../aspose.tasks/vbamodulecollection/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.tasks/vbamodulecollection/copyto/)(VbaModule[], int) |  |
| [GetEnumerator](../../aspose.tasks/vbamodulecollection/getenumerator/)() |  |
| [Remove](../../aspose.tasks/vbamodulecollection/remove/)(VbaModule) |  |
| [ToList](../../aspose.tasks/vbamodulecollection/tolist/)() | 将集合对象转换为 [`VbaModule`](../vbamodule/) 对象的列表。 |

## 示例

展示如何遍历 VBA 模块。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (VbaModule module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Module Type: " + module.Type);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}
```

### 另见

* class [VbaModule](../vbamodule/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


