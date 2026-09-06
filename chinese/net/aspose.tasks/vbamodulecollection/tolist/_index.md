---
title: "VbaModuleCollection.ToList"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaModuleCollection 方法。将集合对象转换为 VbaModule 对象的列表"
type: docs
weight: 100
url: /zh/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

将集合对象转换为 [`VbaModule`](../../vbamodule/) 对象的列表。

```csharp
public List<VbaModule> ToList()
```

### 返回值

对象列表。

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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


