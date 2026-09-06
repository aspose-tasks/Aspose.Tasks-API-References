---
title: "Asn.Stop"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Asn field. التاريخ الذي يتم فيه إيقاف التكليف"
type: docs
weight: 520
url: /ar/net/aspose.tasks/asn/stop/
---
## Asn.Stop field

التاريخ الذي تُوقف فيه المهمة.

```csharp
public static readonly Key<DateTime, AsnKey> Stop;
```

## الأمثلة

يعرض كيفية قراءة تواريخ إيقاف/استئناف التكليف.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// اطبع تواريخ إيقاف واستئناف تكليف المورد
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


