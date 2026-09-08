---
title: "IVbaModule.SourceCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "IVbaModule 속성. VBA 모듈의 소스 코드를 가져옵니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/ivbamodule/sourcecode/
---
## IVbaModule.SourceCode property

VBA 모듈의 소스 코드를 가져옵니다.

```csharp
public string SourceCode { get; }
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


