---
title: "클래스 VbaProject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.VbaProject 클래스. VbaProject를 나타냅니다."
type: docs
weight: 2860
url: /ko/net/aspose.tasks/vbaproject/
---
## VbaProject class

`VbaProject`를 나타냅니다.

```csharp
public class VbaProject
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | 조건부 컴파일 인수를 가져옵니다 |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | 프로젝트 설명을 가져옵니다. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | 프로젝트 도움말 컨텍스트 ID를 가져옵니다. |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | 도움말 파일 이름을 가져옵니다. |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | [`VbaModuleCollection`](../vbamodulecollection/) 컬렉션을 가져옵니다. |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | 프로젝트 이름을 가져옵니다. |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | [`VbaReferenceCollection`](../vbareferencecollection/) 컬렉션을 가져옵니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


