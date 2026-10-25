---
title: "Rsc.CV"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। प्रोजेक्ट स्थिति तिथि तक अर्जित मूल्य लागत वैरिएंस। CV कार्य किए गए कार्य की बजटेड लागत (BCWP) और वास्तविक लागत (ACWP) के बीच का अंतर है"
type: docs
weight: 270
url: /hi/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

परियोजना स्थिति तिथि तक अर्जित मूल्य लागत विचलन। CV कार्य के BCWP (किए गए कार्य की बजटेड लागत) और ACWP (किए गए कार्य की वास्तविक लागत) के बीच अंतर है।

```csharp
public static readonly Key<double, RscKey> CV;
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


