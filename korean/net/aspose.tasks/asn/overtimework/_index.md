---
title: "Asn.OvertimeWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 할당의 예정 초과 근무 작업"
type: docs
weight: 380
url: /ko/net/aspose.tasks/asn/overtimework/
---
## Asn.OvertimeWork field

과제의 예정 초과 근무 작업.

```csharp
public static readonly Key<Duration, AsnKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


