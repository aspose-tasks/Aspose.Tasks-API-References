---
title: "인터페이스 IVbaModule"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.IVbaModule 인터페이스. VBA 코드가 포함된 모듈을 나타냅니다."
type: docs
weight: 880
url: /ko/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

VBA 코드가 포함된 모듈을 나타냅니다.

```csharp
public interface IVbaModule
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | `[`VbaModuleAttributeCollection`](../vbamoduleattributecollection/)` 컬렉션을 가져옵니다. |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | VBA 모듈의 이름을 가져옵니다. |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | VBA 모듈의 소스 코드를 가져옵니다. |

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


