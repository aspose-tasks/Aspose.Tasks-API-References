---
title: "Rsc.IsGeneric"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. निर्धारित करता है कि कोई संसाधन सामान्य है या नहीं।"
type: docs
weight: 410
url: /hi/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

निर्धारित करता है कि संसाधन सामान्य है या नहीं।

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## उदाहरण

दिखाता है कि कैसे Rsc.IsGeneric प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


