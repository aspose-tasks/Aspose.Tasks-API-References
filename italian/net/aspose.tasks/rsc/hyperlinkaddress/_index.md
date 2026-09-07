---
title: "Rsc.HyperlinkAddress"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. L'indirizzo di un collegamento ipertestuale associato a una risorsa"
type: docs
weight: 330
url: /it/net/aspose.tasks/rsc/hyperlinkaddress/
---
## Rsc.HyperlinkAddress field

L'indirizzo di un collegamento ipertestuale associato a una risorsa.

```csharp
public static readonly Key<string, RscKey> HyperlinkAddress;
```

## Osservazioni

L'indirizzo completo (Hyperlink Href in Microsoft Project) del collegamento ipertestuale è una concatenazione di HyperlinkAddress e HyperlinkSubAddress.

## Esempi

Mostra come leggere/scrivere le proprietà dei collegamenti ipertestuali delle risorse.

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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


