---
title: "Rsc.CostCenter"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 발생한 비용이 청구될 비용 센터를 나타냅니다."
type: docs
weight: 230
url: /ko/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

리소스가 발생시킨 비용을 청구할 비용 센터를 나타냅니다.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## 예제

Rsc.CostCenter 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


