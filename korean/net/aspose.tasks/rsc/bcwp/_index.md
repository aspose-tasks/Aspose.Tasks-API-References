---
title: "Rsc.BCWP"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 프로젝트에 수행한 작업에 대한 현재까지의 예산 비용"
type: docs
weight: 140
url: /ko/net/aspose.tasks/rsc/bcwp/
---
## Rsc.BCWP field

리소스가 프로젝트를 위해 수행한 작업의 현재까지 예산 비용.

```csharp
public static readonly Key<double, RscKey> BCWP;
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


