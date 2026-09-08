---
title: "클래스 VbaReferenceCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.VbaReferenceCollection 클래스. VbaReference 객체의 컬렉션을 나타냅니다."
type: docs
weight: 2880
url: /ko/net/aspose.tasks/vbareferencecollection/
---
## VbaReferenceCollection class

[`VbaReference`](../vbareference/) 객체의 컬렉션을 나타냅니다.

```csharp
public class VbaReferenceCollection : ReadOnlyCollectionBase<VbaReference>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaReference) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## 예제

VBA 참조 컬렉션을 사용하는 방법을 보여줍니다.

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

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaReference](../vbareference/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


