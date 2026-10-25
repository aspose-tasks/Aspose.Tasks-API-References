---
title: "Rsc.IsNull"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 null인지 여부를 결정합니다"
type: docs
weight: 420
url: /ko/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

리소스가 null인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## 예제

Rsc.IsNull 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


