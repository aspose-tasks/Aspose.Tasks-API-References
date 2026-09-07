---
title: "Rsc.CanLevel"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। निर्धारित करता है कि क्या संसाधन लेवलिंग किसी संसाधन पर की जा सकती है"
type: docs
weight: 200
url: /hi/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

निर्धारित करता है कि क्या संसाधन लेवलिंग संसाधन पर की जा सकती है।

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## उदाहरण

दिखाता है कि कैसे पढ़ें/लिखें Rsc.CanLevel प्रॉपर्टी।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


