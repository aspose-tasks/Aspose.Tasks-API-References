---
title: "Rsc.HyperlinkSubAddress"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De specifieke locatie in een document in een hyperlink die aan een taak is gekoppeld"
type: docs
weight: 340
url: /nl/net/aspose.tasks/rsc/hyperlinksubaddress/
---
## Rsc.HyperlinkSubAddress field

De specifieke locatie in een document in een hyperlink die aan een taak is gekoppeld.

```csharp
public static readonly Key<string, RscKey> HyperlinkSubAddress;
```

## Opmerkingen

Het volledige adres (Hyperlink Href in Microsoft Project) van de hyperlink is een samenvoeging van HyperlinkAddress en HyperlinkSubAddress.

## Voorbeelden

Toont hoe u de hyperlink‑eigenschappen van resources kunt lezen/schrijven.

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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


