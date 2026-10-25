---
title: "클래스 VbaReference"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.VbaReference 클래스. VbaProject의 참조를 나타냅니다."
type: docs
weight: 2870
url: /ko/net/aspose.tasks/vbareference/
---
## VbaReference class

`[`VbaProject`](../vbaproject/)에 대한 참조를 나타냅니다.`

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [VbaReference](vbareference/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | 라이브러리의 식별자를 가져옵니다. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | VBA 참조의 이름을 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | `VbaReference` 객체와 이 인스턴스가 같은지 여부를 나타내는 값을 반환합니다. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | `VbaReference` 객체와 이 인스턴스가 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | 이 `VbaReference`에 대한 해시 코드 값을 반환합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


