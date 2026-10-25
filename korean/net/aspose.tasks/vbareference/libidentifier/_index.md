---
title: "VbaReference.LibIdentifier"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaReference 속성. 라이브러리 식별자를 가져옵니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

라이브러리의 식별자를 가져옵니다.

```csharp
public string LibIdentifier { get; }
```

## 예제

VBA 참조를 읽는 방법을 보여줍니다.

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

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


