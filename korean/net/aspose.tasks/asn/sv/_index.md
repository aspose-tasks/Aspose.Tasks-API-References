---
title: "Asn.SV"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 프로젝트 상태 날짜까지의 획득 가치 일정 편차. 일정 편차 SV는 BCWP와 BCWS의 차이입니다"
type: docs
weight: 540
url: /ko/net/aspose.tasks/asn/sv/
---
## Asn.SV field

프로젝트 상태 날짜까지의 획득 가치 일정 편차. 일정 편차(SV)는 BCWP와 BCWS 사이의 차이입니다.

```csharp
public static readonly Key<double, AsnKey> SV;
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


