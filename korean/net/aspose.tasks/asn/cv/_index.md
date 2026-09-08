---
title: "Asn.CV"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 획득 가치 비용 차이. CV는 할당의 BCWP(수행된 작업의 예산 비용)와 ACWP(수행된 작업의 실제 비용) 사이의 차이입니다."
type: docs
weight: 220
url: /ko/net/aspose.tasks/asn/cv/
---
## Asn.CV field

획득 가치 비용 편차. CV는 과제의 BCWP(수행된 작업의 예산 비용)와 ACWP(수행된 작업의 실제 비용) 간의 차이입니다.

```csharp
public static readonly Key<double, AsnKey> CV;
```

## 예제

과제 비용 값을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// 리소스 할당 비용 출력
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine(assignment.Get(Asn.Cost));
    Console.WriteLine(assignment.Get(Asn.ACWP));

    // CV = BCWP - ACWP
    Console.WriteLine(assignment.Get(Asn.CV));

    Console.WriteLine(assignment.Get(Asn.BCWP));
    Console.WriteLine(assignment.Get(Asn.BCWS));

    // SV = BCWP - BCWS
    Console.WriteLine(assignment.Get(Asn.SV));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


