---
title: "Rsc.Guid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Contiene el código de identificación único generado para el recurso"
type: docs
weight: 310
url: /es/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

Contiene el código de identificación único generado para el recurso.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Guid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


