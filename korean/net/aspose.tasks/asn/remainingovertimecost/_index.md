---
title: "Asn.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 할당을 완료하는 데 남은 예상 초과 근무 비용"
type: docs
weight: 440
url: /ko/net/aspose.tasks/asn/remainingovertimecost/
---
## Asn.RemainingOvertimeCost field

할당을 완료하는 데 남은 예상 초과 근무 비용.

```csharp
public static readonly Key<decimal, AsnKey> RemainingOvertimeCost;
```

## 예제

할당의 초과/남은 작업/비용을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// 할당 초과 시간을 출력합니다
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


