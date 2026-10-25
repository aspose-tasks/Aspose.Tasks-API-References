---
title: "Rsc.Guid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스에 대해 생성된 고유 식별 코드를 포함합니다."
type: docs
weight: 310
url: /ko/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

리소스에 대해 생성된 고유 식별 코드를 포함합니다.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## 예제

Rsc.Guid 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


