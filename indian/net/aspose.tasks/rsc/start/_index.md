---
title: "Rsc.Start"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। वह तिथि जब निर्धारित संसाधन को कार्य पर काम शुरू करने के लिए नियोजित किया गया है"
type: docs
weight: 640
url: /hi/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

निर्धारित संसाधन के कार्य शुरू करने के लिए नियोजित तिथि।

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## उदाहरण

दिखाता है कि Rsc.Start प्रॉपर्टी को कैसे पढ़ा/लिखा जाए।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


