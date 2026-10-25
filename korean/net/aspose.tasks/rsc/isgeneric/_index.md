---
title: "Rsc.IsGeneric"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 일반인지 여부를 결정합니다."
type: docs
weight: 410
url: /ko/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

리소스가 일반적인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## 예제

Rsc.IsGeneric 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


