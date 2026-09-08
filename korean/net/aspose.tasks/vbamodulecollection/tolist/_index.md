---
title: "VbaModuleCollection.ToList"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaModuleCollection 메서드. 컬렉션 객체를 VbaModule 객체 목록으로 변환합니다"
type: docs
weight: 100
url: /ko/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

컬렉션 객체를 [`VbaModule`](../../vbamodule/) 객체 목록으로 변환합니다.

```csharp
public List<VbaModule> ToList()
```

### 반환 값

객체 목록.

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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


