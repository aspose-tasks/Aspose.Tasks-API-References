---
title: "VbaProject.HelpContextId"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaProject 属性。获取项目帮助上下文 ID"
type: docs
weight: 30
url: /zh/net/aspose.tasks/vbaproject/helpcontextid/
---
## VbaProject.HelpContextId property

获取项目帮助上下文 ID

```csharp
public int HelpContextId { get; }
```

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

* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


