---
title: "Asn.RemainingCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. असाइनमेंट पूरा करने की शेष अनुमानित लागत"
type: docs
weight: 430
url: /hi/net/aspose.tasks/asn/remainingcost/
---
## Asn.RemainingCost field

एक असाइनमेंट को पूरा करने की शेष अनुमानित लागत।

```csharp
public static readonly Key<decimal, AsnKey> RemainingCost;
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


