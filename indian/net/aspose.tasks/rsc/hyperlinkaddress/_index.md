---
title: "Rsc.HyperlinkAddress"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. एक संसाधन से जुड़ी हाइपरलिंक का पता।"
type: docs
weight: 330
url: /hi/net/aspose.tasks/rsc/hyperlinkaddress/
---
## Rsc.HyperlinkAddress field

संसाधन से जुड़े हाइपरलिंक का पता।

```csharp
public static readonly Key<string, RscKey> HyperlinkAddress;
```

## टिप्पणियाँ

हाइपरलिंक का पूर्ण पता (Microsoft Project में Hyperlink Href) HyperlinkAddress और HyperlinkSubAddress का संयोजन है।

## उदाहरण

दिखाता है कि कैसे संसाधन की हाइपरलिंक प्रॉपर्टीज़ को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Hyperlink, "Click to visit our site");
resource.Set(Rsc.HyperlinkAddress, "https://products.aspose.com");
resource.Set(Rsc.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + resource.Get(Rsc.Hyperlink));
Console.WriteLine("Hyperlink Address: " + resource.Get(Rsc.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + resource.Get(Rsc.HyperlinkSubAddress));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


