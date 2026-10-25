---
title: "Rsc.BCWP"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। एक संसाधन द्वारा परियोजना के लिए आज तक किए गए कार्य की बजटेड लागत"
type: docs
weight: 140
url: /hi/net/aspose.tasks/rsc/bcwp/
---
## Rsc.BCWP field

परियोजना के वर्तमान तक संसाधन द्वारा किए गए कार्य की बजटेड लागत।

```csharp
public static readonly Key<double, RscKey> BCWP;
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


