---
title: "클래스 VbaModule"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.VbaModule 클래스. VBA 모듈을 나타냅니다"
type: docs
weight: 2810
url: /ko/net/aspose.tasks/vbamodule/
---
## VbaModule class

VBA 모듈을 나타냅니다.

```csharp
public sealed class VbaModule
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | 모듈의 속성 컬렉션을 가져옵니다. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | VBA 모듈의 이름을 가져옵니다. |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | VBA 모듈의 소스 코드를 가져오거나 설정합니다. |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | 모듈의 유형을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | `VbaModule`의 인스턴스를 VbaModuleType.ClassModule 유형으로 생성합니다. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | `VbaModule`의 인스턴스를 VbaModuleType.ProceduralModule 유형으로 생성합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


