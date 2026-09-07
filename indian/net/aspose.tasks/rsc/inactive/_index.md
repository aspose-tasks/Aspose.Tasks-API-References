---
title: "Rsc.Inactive"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. निर्धारित करता है कि क्या किसी संसाधन को प्रशासनिक अधिकार वाले उपयोगकर्ता द्वारा निष्क्रिय किया गया था"
type: docs
weight: 360
url: /hi/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

निर्धारित करता है कि क्या संसाधन को प्रशासनिक अधिकार वाले उपयोगकर्ता द्वारा निष्क्रिय किया गया था।

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## उदाहरण

दिखाता है कि Rsc.Inactive प्रॉपर्टी को कैसे पढ़ें/लिखें.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


