---
title: "Rsc.OvertimeRateFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। ओवरटाइम दर दिखाने के लिए Microsoft Project द्वारा उपयोग किए जाने वाले इकाइयाँ"
type: docs
weight: 520
url: /hi/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

Microsoft Project द्वारा ओवरटाइम दर दिखाने के लिए उपयोग की जाने वाली इकाइयाँ।

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
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
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


