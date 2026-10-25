---
title: "Rsc.MaterialLabel"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। सामग्री संसाधन के लिए माप इकाई"
type: docs
weight: 440
url: /hi/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

सामग्री संसाधन की माप इकाई।

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## उदाहरण

दिखाता है कि कैसे Rsc.MaterialLabel प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


