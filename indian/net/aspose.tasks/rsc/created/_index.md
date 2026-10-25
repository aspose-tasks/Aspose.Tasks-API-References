---
title: "Rsc.Created"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. वह तिथि और समय जब एक संसाधन को प्रोजेक्ट में जोड़ा गया था।"
type: docs
weight: 260
url: /hi/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

संसाधन को परियोजना में जोड़े जाने की तिथि और समय।

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## उदाहरण

दिखाता है कि कैसे Rsc.Created प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


