---
title: "VbaReference.Name"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaReference 속성. VBA 참조의 이름을 가져오거나 설정합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

VBA 참조의 이름을 가져오거나 설정합니다.

```csharp
public string Name { get; set; }
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


