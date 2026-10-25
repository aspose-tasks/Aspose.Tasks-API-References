---
title: "IVbaModule.Name"
second_title: "Aspose.Tasks for .NET API 참조"
description: "IVbaModule 속성. VBA 모듈의 이름을 가져옵니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/ivbamodule/name/
---
## IVbaModule.Name property

VBA 모듈의 이름을 가져옵니다.

```csharp
public string Name { get; }
```

## 예제

VBA 프로젝트의 모듈을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### 또 보기

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


