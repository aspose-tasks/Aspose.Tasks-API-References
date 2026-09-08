---
title: "Rsc.Hyperlink"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El título o texto explicativo de un hipervínculo asociado a un recurso"
type: docs
weight: 320
url: /es/net/aspose.tasks/rsc/hyperlink/
---
## Rsc.Hyperlink field

El título o texto explicativo de un hipervínculo asociado a un recurso.

```csharp
public static readonly Key<string, RscKey> Hyperlink;
```

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


