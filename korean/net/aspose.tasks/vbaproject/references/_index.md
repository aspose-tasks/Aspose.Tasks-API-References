---
title: "VbaProject.References"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaProject 속성. VbaReferenceCollection 컬렉션을 가져옵니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

`[`VbaReferenceCollection`](../../vbareferencecollection/)` 컬렉션을 가져옵니다.

```csharp
public VbaReferenceCollection References { get; }
```

## 예제

VBA 프로젝트 참조 정보를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### 또 보기

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


