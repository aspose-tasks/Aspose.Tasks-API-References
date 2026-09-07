---
title: "Rsc.CostCenter"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड. दर्शाता है कि संसाधन द्वारा संचित लागतें किस लागत केंद्र में चार्ज की जानी चाहिए"
type: docs
weight: 230
url: /hi/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

निर्दिष्ट करता है कि संसाधन द्वारा संचित लागतें किस लागत केंद्र में चार्ज की जानी चाहिए।

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## उदाहरण

दिखाता है कि कैसे Rsc.CostCenter प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


