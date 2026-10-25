---
title: "Rsc.IsCostResource"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 비용 리소스인지 여부를 결정합니다"
type: docs
weight: 390
url: /ko/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

리소스가 비용 리소스인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## 예제

Rsc.IsCostResource 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


