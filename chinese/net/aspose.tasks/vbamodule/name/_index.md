---
title: "VbaModule.Name"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaModule 属性。获取 VBA 模块的名称"
type: docs
weight: 40
url: /zh/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

获取 VBA 模块的名称

```csharp
public string Name { get; set; }
```

## 示例

展示如何读取 VBA 项目的模块。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### 另见

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


