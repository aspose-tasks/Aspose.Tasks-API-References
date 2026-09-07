---
title: "Rsc.SV"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। प्रोजेक्ट स्थिति तिथि तक अर्जित मूल्य शेड्यूल वैरिएंस। SV वह अंतर है जो कार्य किए गए बजटेड लागत (BCWP) और शेड्यूल किए गए बजटेड लागत (BCWS) के बीच है"
type: docs
weight: 650
url: /hi/net/aspose.tasks/rsc/sv/
---
## Rsc.SV field

परियोजना स्थिति तिथि तक अर्जित मूल्य शेड्यूल विचलन। SV वह अंतर है जो कार्य के निष्पादित बजट लागत (BCWP) और नियोजित कार्य के बजट लागत (BCWS) के बीच होता है।

```csharp
public static readonly Key<double, RscKey> SV;
```

## उदाहरण

दिखाता है कि संसाधन लागतें कैसे पढ़ी जाएँ।

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// सभी संसाधन लागतें प्रदर्शित करें
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


