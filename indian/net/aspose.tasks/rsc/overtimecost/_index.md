---
title: "Rsc.OvertimeCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। एक संसाधन के सभी असाइन किए गए कार्यों पर कुल ओवरटाइम लागत"
type: docs
weight: 500
url: /hi/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

सभी सौंपे गए कार्यों पर संसाधन की कुल ओवरटाइम लागत।

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## उदाहरण

दिखाता है कि कैसे पढ़ें संसाधन ओवरटाइम मान।

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// सभी संसाधनों के लिए ओवरटाइम संबंधित पैरामीटर प्रदर्शित करें
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


