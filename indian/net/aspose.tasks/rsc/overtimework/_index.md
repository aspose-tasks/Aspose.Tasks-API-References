---
title: "Rsc.OvertimeWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड. एक कार्य पर संसाधन द्वारा किए जाने वाले निर्धारित ओवरटाइम की मात्रा और संबंधित संसाधनों की ओवरटाइम दरों पर चार्ज की जाती है"
type: docs
weight: 530
url: /hi/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

किसी कार्य पर संसाधन द्वारा निर्धारित ओवरटाइम की मात्रा और शामिल संसाधनों की ओवरटाइम दरों पर चार्ज की गई।

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


