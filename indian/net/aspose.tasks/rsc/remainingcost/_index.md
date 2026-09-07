---
title: "Rsc.RemainingCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। शेष निर्धारित खर्च जो शेष निर्धारित कार्य को पूरा करने में आएगा"
type: docs
weight: 580
url: /hi/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

शेष निर्धारित कार्य को पूरा करने में होने वाला शेष निर्धारित खर्च।

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## उदाहरण

दिखाता है कि कैसे Rsc.RemainingCost प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


