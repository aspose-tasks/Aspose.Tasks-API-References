---
title: "Asn.BCWP"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 할당에 수행된 작업의 현재까지 예산 비용"
type: docs
weight: 120
url: /ko/net/aspose.tasks/asn/bcwp/
---
## Asn.BCWP field

과제에 수행된 작업의 현재까지 예산 비용.

```csharp
public static readonly Key<double, AsnKey> BCWP;
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


