---
title: "Prj.HonorConstraints"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 작업이 제약 날짜를 준수하는지 여부를 결정합니다."
type: docs
weight: 370
url: /ko/net/aspose.tasks/prj/honorconstraints/
---
## Prj.HonorConstraints field

작업이 제약 날짜를 준수하는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> HonorConstraints;
```

## 예제

Prj.HonorConstraints 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.HonorConstraints, true);

Console.WriteLine("Honor Constraints: " + project.Get(Prj.HonorConstraints));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


