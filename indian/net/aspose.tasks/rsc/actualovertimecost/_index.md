---
title: "Rsc.ActualOvertimeCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। असाइन किए गए संसाधनों द्वारा कार्यों पर पहले से किए गए ओवरटाइम कार्य की लागत"
type: docs
weight: 40
url: /hi/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

असाइन किए गए रिसोर्स द्वारा टास्क पर पहले से किए गए ओवरटाइम कार्य के लिए हुए खर्च।

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## उदाहरण

दिखाता है कि कैसे पढ़ें/लिखें Rsc.ActualOvertimeCost प्रॉपर्टी।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


