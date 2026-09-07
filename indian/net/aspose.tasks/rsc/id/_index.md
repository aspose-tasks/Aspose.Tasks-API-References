---
title: "Rsc.Id"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। संसाधनों की सूची में एक संसाधन की स्थिति पहचानकर्ता।"
type: docs
weight: 350
url: /hi/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

संसाधनों की सूची में संसाधन की स्थिति पहचानकर्ता।

```csharp
public static readonly Key<int, RscKey> Id;
```

## उदाहरण

Rsc.Id प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


