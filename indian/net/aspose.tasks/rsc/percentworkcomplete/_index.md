---
title: "Rsc.PercentWorkComplete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड. सभी कार्यों में पूर्ण किए गए कार्य का प्रतिशत"
type: docs
weight: 550
url: /hi/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

सभी कार्यों में पूर्ण किए गए कार्य का प्रतिशत।

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## उदाहरण

दिखाता है कि कैसे संसाधन के कार्य पूर्णता प्रतिशत को पढ़ें।

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// सभी संसाधनों के लिए कार्य प्रतिशत पूर्णता प्रदर्शित करें
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


