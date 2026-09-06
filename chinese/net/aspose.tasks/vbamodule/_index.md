---
title: "类 VbaModule"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.VbaModule 类。表示一个 VBA 模块"
type: docs
weight: 2810
url: /zh/net/aspose.tasks/vbamodule/
---
## VbaModule class

表示一个 VBA 模块。

```csharp
public sealed class VbaModule
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | 获取模块属性的集合。 |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | 获取 VBA 模块的名称 |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | 获取或设置 VBA 模块的源代码 |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | 获取模块的类型。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | 创建一个 `VbaModule` 实例，类型为 VbaModuleType.ClassModule。 |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | 创建一个 `VbaModule` 实例，类型为 VbaModuleType.ProceduralModule。 |

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


