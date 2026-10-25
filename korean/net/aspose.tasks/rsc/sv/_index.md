---
title: "Rsc.SV"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 프로젝트 상태 날짜까지의 획득 가치 일정 편차. SV는 수행된 작업의 예산 비용(BCWP)과 예정된 작업의 예산 비용(BCWS) 사이의 차이입니다."
type: docs
weight: 650
url: /ko/net/aspose.tasks/rsc/sv/
---
## Rsc.SV field

프로젝트 상태 날짜까지의 획득 가치 일정 편차. SV는 수행된 작업의 예산 비용(BCWP)과 예정된 작업의 예산 비용(BCWS) 사이의 차이입니다.

```csharp
public static readonly Key<double, RscKey> SV;
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


