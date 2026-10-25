---
title: "Rsc.HyperlinkAddress"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. L’adresse d’un hyperlien associé à une ressource"
type: docs
weight: 330
url: /fr/net/aspose.tasks/rsc/hyperlinkaddress/
---
## Rsc.HyperlinkAddress field

L'adresse d'un hyperlien associé à une ressource.

```csharp
public static readonly Key<string, RscKey> HyperlinkAddress;
```

## Remarques

L’adresse complète (Hyperlink Href dans Microsoft Project) de l’hyperlien est une concaténation de HyperlinkAddress et HyperlinkSubAddress.

## Exemples

Montre comment lire/écrire les propriétés d’hyperlien des ressources.

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

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


