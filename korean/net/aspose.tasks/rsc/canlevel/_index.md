---
title: "Rsc.CanLevel"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스에 대해 리소스 레벨링을 수행할 수 있는지 여부를 결정합니다."
type: docs
weight: 200
url: /ko/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

리소스에 대해 리소스 레벨링을 수행할 수 있는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## 예제

Rsc.CanLevel 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


