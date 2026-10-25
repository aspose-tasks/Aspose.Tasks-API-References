---
title: "Asn.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 할당에서 완료된 작업량"
type: docs
weight: 400
url: /ko/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

할당에 대해 완료된 작업량.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## 예제

할당의 작업 완료 비율을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// 할당 작업 완료 비율을 출력합니다
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


