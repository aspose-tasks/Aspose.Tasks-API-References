---
title: "Asn.CV"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। अर्जित मूल्य लागत विचलन। CV वह अंतर है जो असाइनमेंट के BCWP (बजटेड लागत ऑफ वर्क परफ़ॉर्म्ड) और ACWP (वास्तविक लागत ऑफ वर्क परफ़ॉर्म्ड) के बीच होता है।"
type: docs
weight: 220
url: /hi/net/aspose.tasks/asn/cv/
---
## Asn.CV field

प्राप्त मूल्य लागत विचलन। CV असाइनमेंट के BCWP (किए गए कार्य की बजटेड लागत) और ACWP (किए गए कार्य की वास्तविक लागत) के बीच अंतर है।

```csharp
public static readonly Key<double, AsnKey> CV;
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


