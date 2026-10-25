---
title: "VbaReference.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaReference 메서드. 이 VbaReference에 대한 해시 코드 값을 반환합니다"
type: docs
weight: 50
url: /ko/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

이 [`VbaReference`](../)에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

VBA 참조의 해시 코드를 얻는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// 참조의 해시 코드는 내부 참조 GUID의 해시 코드입니다.
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### 또 보기

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


