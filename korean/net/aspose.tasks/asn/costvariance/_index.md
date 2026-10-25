---
title: "Asn.CostVariance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 할당에 대한 기준 비용과 총 비용 사이의 차이"
type: docs
weight: 200
url: /ko/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

과제의 기준 비용과 총 비용 간의 차이.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
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
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


