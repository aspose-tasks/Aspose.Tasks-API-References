---
title: "Rsc.ActualCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। संसाधनों द्वारा उनके कार्यों पर पहले से किए गए काम के लिए उत्पन्न लागत, साथ ही कार्य से संबंधित किसी भी अन्य दर्ज लागत।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

रिसोर्स द्वारा उनके टास्क पर पहले से किए गए कार्य के लिए हुए खर्च, साथ ही टास्क से जुड़े अन्य रिकॉर्ड किए गए खर्च।

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## उदाहरण

Rsc.ActualCost प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


