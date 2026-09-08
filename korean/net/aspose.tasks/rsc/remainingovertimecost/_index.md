---
title: "Rsc.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스에 대한 남은 예정 초과 근무 비용"
type: docs
weight: 590
url: /ko/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

리소스에 대한 남은 예정 초과 근무 비용.

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## 예제

Rsc.RemainingOvertimeCost 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


