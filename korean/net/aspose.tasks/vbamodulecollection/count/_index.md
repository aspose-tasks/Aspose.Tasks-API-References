---
title: "VbaModuleCollection.Count"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaModuleCollection 속성."
type: docs
weight: 10
url: /ko/net/aspose.tasks/vbamodulecollection/count/
---
## VbaModuleCollection.Count property

```csharp
public int Count { get; }
```

## 예제

VBA 모듈을 반복하는 방법을 보여줍니다.

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

### 또 보기

* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


