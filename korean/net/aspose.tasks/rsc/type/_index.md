---
title: "Rsc.Type"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스 유형"
type: docs
weight: 660
url: /ko/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

리소스 유형.

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## 예제

Rsc.Type 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


