---
title: "Rsc.AccrueAt"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। निर्धारित करता है कि कैसे और कब संसाधन मानक और ओवरटाइम लागतों को कार्य की लागत में चार्ज या संचित किया जाए"
type: docs
weight: 10
url: /hi/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

निर्धारित करता है कि कब और कैसे रिसोर्स के मानक और ओवरटाइम लागतों को टास्क की लागत में चार्ज या संचित किया जाए।

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## उदाहरण

दिखाता है कि कैसे पढ़ें/लिखें Rsc.AccrueAt प्रॉपर्टी।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


