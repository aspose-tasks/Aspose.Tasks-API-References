---
title: "Rsc.CostPerUse"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड. वह लागत जो प्रत्येक बार संसाधन के उपयोग पर उत्पन्न होती है"
type: docs
weight: 240
url: /hi/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

संसाधन के प्रत्येक उपयोग पर उत्पन्न होने वाली लागत।

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## उदाहरण

दिखाता है कि कैसे Rsc.CostPerUse प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


