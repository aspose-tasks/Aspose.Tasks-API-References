---
title: "Rsc.Hyperlink"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynakla ilişkili bir köprünün (hyperlink) başlığı veya açıklayıcı metni."
type: docs
weight: 320
url: /tr/net/aspose.tasks/rsc/hyperlink/
---
## Rsc.Hyperlink field

Kaynakla ilişkili bir köprünün başlığı veya açıklayıcı metni.

```csharp
public static readonly Key<string, RscKey> Hyperlink;
```

## Örnekler

Kaynakların köprü (hyperlink) özelliklerinin nasıl okunup yazılacağını gösterir.

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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


