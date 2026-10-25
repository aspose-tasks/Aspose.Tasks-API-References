---
title: "Rsc.Name"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। किसी संसाधन का नाम"
type: docs
weight: 460
url: /hi/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

संसाधन का नाम।

```csharp
public static readonly Key<string, RscKey> Name;
```

## उदाहरण

दिखाता है कि Rsc.Name प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


