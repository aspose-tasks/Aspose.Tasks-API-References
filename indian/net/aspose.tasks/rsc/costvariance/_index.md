---
title: "Rsc.CostVariance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड. एक संसाधन के लिए बेसलाइन लागत और कुल लागत के बीच अंतर"
type: docs
weight: 250
url: /hi/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

संसाधन के लिए बेसलाइन लागत और कुल लागत के बीच अंतर।

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## उदाहरण

दिखाता है कि कैसे Rsc.CostVariance प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


