---
title: "Prj.EarnedValueMethod"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 획득 가치 계산을 위한 기본 방법"
type: docs
weight: 310
url: /ko/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

획득 가치를 계산하는 기본 방법.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## 예제

Prj.EarnedValueMethod 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


