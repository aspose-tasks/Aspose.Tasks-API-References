---
title: "Rsc.OvertimeCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 모든 할당된 작업에 대한 리소스의 총 초과 근무 비용"
type: docs
weight: 500
url: /ko/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

리소스가 할당된 모든 작업에 대한 총 초과 근무 비용입니다.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## 예제

리소스 초과 근무 값을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// 모든 리소스에 대한 초과 근무 관련 매개변수를 표시합니다.
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


