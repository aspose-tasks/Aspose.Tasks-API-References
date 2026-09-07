---
title: "Rsc.AvailableFrom"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। वह प्रारंभिक तिथि जब एक संसाधन वर्तमान समय अवधि के लिए निर्दिष्ट इकाइयों पर काम के लिए उपलब्ध होता है।"
type: docs
weight: 120
url: /hi/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

वह प्रारंभ तिथि जब संसाधन वर्तमान समय अवधि के लिए निर्दिष्ट इकाइयों पर कार्य के लिए उपलब्ध होता है।

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## उदाहरण

Rsc.AvailableFrom प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


