---
title: "Asn.BCWP"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। असाइनमेंट पर किए गए कार्य की बजटेड लागत आज तक"
type: docs
weight: 120
url: /hi/net/aspose.tasks/asn/bcwp/
---
## Asn.BCWP field

असाइनमेंट पर अब तक किए गए कार्य की बजटेड लागत।

```csharp
public static readonly Key<double, AsnKey> BCWP;
```

## उदाहरण

असाइनमेंट की लागत मानों को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// रिसोर्स असाइनमेंट लागतें प्रिंट करें
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

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


