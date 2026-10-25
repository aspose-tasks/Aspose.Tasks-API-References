---
title: "Rsc.Type"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। किसी संसाधन का प्रकार"
type: docs
weight: 660
url: /hi/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

संसाधन का प्रकार।

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## उदाहरण

दिखाता है कि कैसे Rsc.Type प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


