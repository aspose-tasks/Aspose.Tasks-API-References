---
title: "Rsc.HyperlinkAddress"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La dirección de un hipervínculo asociado a un recurso"
type: docs
weight: 330
url: /es/net/aspose.tasks/rsc/hyperlinkaddress/
---
## Rsc.HyperlinkAddress field

La dirección de un hipervínculo asociado a un recurso.

```csharp
public static readonly Key<string, RscKey> HyperlinkAddress;
```

## Observaciones

La dirección completa (Hipervínculo Href en Microsoft Project) del hipervínculo es una concatenación de HyperlinkAddress y HyperlinkSubAddress.

## Ejemplos

Muestra cómo leer/escribir las propiedades de hipervínculo de los recursos.

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

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


