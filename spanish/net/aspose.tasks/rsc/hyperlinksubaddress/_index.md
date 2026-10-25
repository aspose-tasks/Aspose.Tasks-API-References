---
title: "Rsc.HyperlinkSubAddress"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. La ubicación específica en un documento en un hipervínculo asociado a una tarea"
type: docs
weight: 340
url: /es/net/aspose.tasks/rsc/hyperlinksubaddress/
---
## Rsc.HyperlinkSubAddress field

La ubicación específica en un documento en un hipervínculo asociado a una tarea.

```csharp
public static readonly Key<string, RscKey> HyperlinkSubAddress;
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


