---
title: "类 VbaProject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.VbaProject 类。表示 VbaProject"
type: docs
weight: 2860
url: /zh/net/aspose.tasks/vbaproject/
---
## VbaProject class

表示 `VbaProject`。

```csharp
public class VbaProject
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | 获取条件编译参数 |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | 获取项目描述。 |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | 获取项目帮助上下文 ID |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | 获取帮助文件名 |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | 获取 [`VbaModuleCollection`](../vbamodulecollection/) 的集合 |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | 获取项目名称 |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | 获取 [`VbaReferenceCollection`](../vbareferencecollection/) 的集合 |

## 示例

展示如何读取 VBA 项目属性。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


