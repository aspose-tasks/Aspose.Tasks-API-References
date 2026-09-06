---
title: "VbaProject.Description"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaProject 属性。获取项目描述"
type: docs
weight: 20
url: /zh/net/aspose.tasks/vbaproject/description/
---
## VbaProject.Description property

获取项目描述。

```csharp
public string Description { get; }
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


