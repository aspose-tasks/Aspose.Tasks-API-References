---
title: "IVbaModule.Name"
second_title: "Aspose.Tasks for .NET API 参考"
description: "IVbaModule 属性。获取 VBA 模块的名称"
type: docs
weight: 20
url: /zh/net/aspose.tasks/ivbamodule/name/
---
## IVbaModule.Name property

获取 VBA 模块的名称

```csharp
public string Name { get; }
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

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


