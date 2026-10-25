---
title: "Asn.FinishVariance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 기준 완료 날짜와 비교한 할당 완료 날짜의 차이"
type: docs
weight: 250
url: /ko/net/aspose.tasks/asn/finishvariance/
---
## Asn.FinishVariance field

과제 종료 날짜가 기준 종료 날짜와 차이(분산)입니다.

```csharp
public static readonly Key<Duration, AsnKey> FinishVariance;
```

## 예제

할당 변동을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// 할당 변동을 출력합니다
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


