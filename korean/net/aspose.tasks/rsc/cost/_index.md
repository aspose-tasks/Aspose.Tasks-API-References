---
title: "Rsc.Cost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 작업에 할당된 리소스가 수행한 작업에 이미 발생한 비용과 남은 작업에 대해 계획된 비용을 합산한, 리소스에 대한 전체 예정 또는 예상 비용"
type: docs
weight: 220
url: /ko/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

작업에 할당된 리소스가 수행한 작업에 대해 이미 발생한 비용과 남은 작업에 대해 계획된 비용을 합산한, 리소스에 대한 총 예정 또는 예상 비용.

```csharp
public static readonly Key<decimal, RscKey> Cost;
```

## 예제

리소스 비용을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// 모든 리소스 비용을 표시합니다.
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


