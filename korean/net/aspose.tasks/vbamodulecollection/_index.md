---
title: "클래스 VbaModuleCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.VbaModuleCollection 클래스. VbaModule 객체의 컬렉션을 나타냅니다"
type: docs
weight: 2840
url: /ko/net/aspose.tasks/vbamodulecollection/
---
## VbaModuleCollection class

[`VbaModule`](../vbamodule/) 객체의 컬렉션을 나타냅니다.

```csharp
public class VbaModuleCollection : ICollection<VbaModule>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/vbamodulecollection/count/) { get; } |  |
| [IsReadOnly](../../aspose.tasks/vbamodulecollection/isreadonly/) { get; } |  |
| [Item](../../aspose.tasks/vbamodulecollection/item/) { get; } | 지정된 인덱스에 있는 모듈을 가져옵니다. (2개의 인덱서) |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/vbamodulecollection/add/)(VbaModule) |  |
| [Clear](../../aspose.tasks/vbamodulecollection/clear/)() |  |
| [Contains](../../aspose.tasks/vbamodulecollection/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.tasks/vbamodulecollection/copyto/)(VbaModule[], int) |  |
| [GetEnumerator](../../aspose.tasks/vbamodulecollection/getenumerator/)() |  |
| [Remove](../../aspose.tasks/vbamodulecollection/remove/)(VbaModule) |  |
| [ToList](../../aspose.tasks/vbamodulecollection/tolist/)() | 컬렉션 객체를 [`VbaModule`](../vbamodule/) 객체 목록으로 변환합니다. |

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

* class [VbaModule](../vbamodule/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


