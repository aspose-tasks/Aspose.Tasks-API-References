---
title: "VbaProject.Name"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaProject 속성. 프로젝트 이름을 가져옵니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks/vbaproject/name/
---
## VbaProject.Name property

프로젝트 이름을 가져옵니다.

```csharp
public string Name { get; }
```

## 예제

VBA 프로젝트 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### 또 보기

* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


