---
title: "Rsc.Hyperlink"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. एक संसाधन से जुड़ी हाइपरलिंक का शीर्षक या व्याख्यात्मक पाठ।"
type: docs
weight: 320
url: /hi/net/aspose.tasks/rsc/hyperlink/
---
## Rsc.Hyperlink field

संसाधन से जुड़े हाइपरलिंक का शीर्षक या व्याख्यात्मक पाठ।

```csharp
public static readonly Key<string, RscKey> Hyperlink;
```

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


