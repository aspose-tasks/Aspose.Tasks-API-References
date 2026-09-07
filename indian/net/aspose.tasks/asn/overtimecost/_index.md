---
title: "Asn.OvertimeCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. असाइनमेंट की वास्तविक और शेष ओवरटाइम लागत का योग"
type: docs
weight: 370
url: /hi/net/aspose.tasks/asn/overtimecost/
---
## Asn.OvertimeCost field

असाइनमेंट की वास्तविक और शेष ओवरटाइम लागत का योग।

```csharp
public static readonly Key<decimal, AsnKey> OvertimeCost;
```

## उदाहरण

दिखाता है कि असाइनमेंट की ओवरटाइम/शेष कार्य/लागत कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// असाइनमेंट ओवरटाइम प्रिंट करें
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

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


