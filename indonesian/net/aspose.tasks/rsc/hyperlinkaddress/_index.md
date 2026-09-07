---
title: "Rsc.HyperlinkAddress"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Alamat untuk hyperlink yang terkait dengan sebuah sumber daya"
type: docs
weight: 330
url: /id/net/aspose.tasks/rsc/hyperlinkaddress/
---
## Rsc.HyperlinkAddress field

Alamat tautan yang terkait dengan sumber daya.

```csharp
public static readonly Key<string, RscKey> HyperlinkAddress;
```

## Catatan

Alamat lengkap (Hyperlink Href dalam Microsoft Project) dari hyperlink adalah penggabungan HyperlinkAddress dan HyperlinkSubAddress.

## Contoh

Menampilkan cara membaca/menulis properti hyperlink sumber daya.

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

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


