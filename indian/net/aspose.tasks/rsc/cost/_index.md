---
title: "Rsc.Cost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड. एक संसाधन के लिए कुल निर्धारित या अनुमानित लागत, जो उन कार्यों के लिए पहले से हुई लागतों पर आधारित है जो कार्यों को सौंपे गए संसाधनों द्वारा किए गए हैं, साथ ही शेष कार्य के लिए नियोजित लागतों के साथ"
type: docs
weight: 220
url: /hi/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

संसाधन के लिए कुल निर्धारित या अनुमानित लागत, जो कार्यों को सौंपे गए संसाधनों द्वारा किए गए कार्य की पहले से हुई लागत और शेष कार्य के लिए नियोजित लागतों पर आधारित है।

```csharp
public static readonly Key<decimal, RscKey> Cost;
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


