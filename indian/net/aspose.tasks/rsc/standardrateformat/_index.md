---
title: "Rsc.StandardRateFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। मानक दर प्रदर्शित करने के लिए Microsoft Project द्वारा उपयोग की जाने वाली इकाइयाँ"
type: docs
weight: 630
url: /hi/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

Microsoft Project द्वारा मानक दर दिखाने के लिए उपयोग किए जाने वाले इकाइयाँ।

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## उदाहरण

दिखाता है कि Rsc.StandardRateFormat प्रॉपर्टी को कैसे पढ़ा/लिखा जाए।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


