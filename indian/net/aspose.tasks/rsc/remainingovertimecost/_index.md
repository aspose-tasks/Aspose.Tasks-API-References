---
title: "Rsc.RemainingOvertimeCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। किसी संसाधन के लिए शेष निर्धारित ओवरटाइम खर्च"
type: docs
weight: 590
url: /hi/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

संसाधन के लिए शेष निर्धारित ओवरटाइम खर्च।

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## उदाहरण

दिखाता है कि कैसे Rsc.RemainingOvertimeCost प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


