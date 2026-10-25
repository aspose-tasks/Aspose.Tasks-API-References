---
title: "VbaReference.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaReference 메서드. 이 인스턴스가 지정된 VbaReference 객체와 같은지 여부를 나타내는 값을 반환합니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

이 인스턴스가 지정된 [`VbaReference`](../) 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public bool Equals(VbaReference other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | VbaReference | 이 인스턴스와 비교할 지정된 [`VbaReference`](../) 객체. |

### 반환 값

이 인스턴스가 지정된 [`VbaReference`](../) 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.

## 예제

VBA 참조 동등성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// 참조의 동등성은 해당 참조의 이름을 기준으로 확인됩니다.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### 또 보기

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

이 인스턴스가 지정된 [`VbaReference`](../) 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 지정된 [`VbaReference`](../) 객체. |

### 반환 값

이 인스턴스가 지정된 [`VbaReference`](../) 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.

## 예제

VBA 참조 동등성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// 참조의 동등성은 해당 참조의 이름을 기준으로 확인됩니다.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### 또 보기

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


