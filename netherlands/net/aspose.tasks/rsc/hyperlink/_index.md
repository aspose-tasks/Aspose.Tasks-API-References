---
title: "Rsc.Hyperlink"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De titel of toelichtende tekst van een hyperlink die aan een resource is gekoppeld."
type: docs
weight: 320
url: /nl/net/aspose.tasks/rsc/hyperlink/
---
## Rsc.Hyperlink field

De titel of verklarende tekst van een hyperlink die aan een resource is gekoppeld.

```csharp
public static readonly Key<string, RscKey> Hyperlink;
```

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


