---
title: "Asn.CostVariance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. एक असाइनमेंट के लिए बेसलाइन लागत और कुल लागत के बीच का अंतर"
type: docs
weight: 200
url: /hi/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

असाइनमेंट के लिए बेसलाइन लागत और कुल लागत के बीच अंतर।

```csharp
public static readonly Key<double, AsnKey> CostVariance;
```

## उदाहरण

असाइनमेंट के वैरिएंस को कैसे पढ़ें दिखाता है।

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// असाइनमेंट वैरिएंस प्रिंट करें
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


