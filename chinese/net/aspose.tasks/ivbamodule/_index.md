---
title: "接口 IVbaModule"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.IVbaModule 接口。表示包含 VBA 代码的模块"
type: docs
weight: 880
url: /zh/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

表示包含 VBA 代码的模块。

```csharp
public interface IVbaModule
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | 获取 [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) 的集合 |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | 获取 VBA 模块的名称 |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | 获取 VBA 模块的源代码 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


