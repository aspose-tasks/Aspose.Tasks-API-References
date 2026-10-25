---
title: "Asn.StartVariance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. एक असाइनमेंट की प्रारंभ तिथि का बेसलाइन प्रारंभ तिथि से वैरिएंस"
type: docs
weight: 510
url: /hi/net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

एक असाइनमेंट की प्रारंभ तिथि का बेसलाइन प्रारंभ तिथि से विचलन।

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


