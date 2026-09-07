---
title: "Asn.SV"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. प्रोजेक्ट स्थिति तिथि तक अर्जित मूल्य शेड्यूल वैरिएंस। शेड्यूल वैरिएंस SV, BCWP और BCWS के बीच का अंतर है"
type: docs
weight: 540
url: /hi/net/aspose.tasks/asn/sv/
---
## Asn.SV field

परियोजना स्थिति तिथि तक अर्जित मूल्य अनुसूची विचलन। अनुसूची विचलन (SV) BCWP और BCWS के बीच का अंतर है।

```csharp
public static readonly Key<double, AsnKey> SV;
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


