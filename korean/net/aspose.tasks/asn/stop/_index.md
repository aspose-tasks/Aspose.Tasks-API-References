---
title: "Asn.Stop"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 할당이 중단되는 날짜"
type: docs
weight: 520
url: /ko/net/aspose.tasks/asn/stop/
---
## Asn.Stop field

할당이 중단되는 날짜.

```csharp
public static readonly Key<DateTime, AsnKey> Stop;
```

## 예제

할당의 중단/재개 날짜를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// 리소스 할당의 중단 및 재개 날짜를 출력합니다.
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


