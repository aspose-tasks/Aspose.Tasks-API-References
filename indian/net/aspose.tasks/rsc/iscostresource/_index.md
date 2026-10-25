---
title: "Rsc.IsCostResource"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। निर्धारित करता है कि क्या कोई संसाधन लागत संसाधन है"
type: docs
weight: 390
url: /hi/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

निर्धारित करता है कि संसाधन लागत संसाधन है या नहीं।

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## उदाहरण

दिखाता है कि कैसे Rsc.IsCostResource प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


