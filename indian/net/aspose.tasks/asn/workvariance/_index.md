---
title: "Asn.WorkVariance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. एक कार्य की बेसलाइन कार्य और वर्तमान में निर्धारित कार्य के बीच का अंतर"
type: docs
weight: 620
url: /hi/net/aspose.tasks/asn/workvariance/
---
## Asn.WorkVariance field

कार्य के बेसलाइन कार्य और वर्तमान में निर्धारित कार्य के बीच अंतर।

```csharp
public static readonly Key<Duration, AsnKey> WorkVariance;
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


