---
title: "Rsc.Id"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El identificador de posición de un recurso dentro de la lista de recursos"
type: docs
weight: 350
url: /es/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

El identificador de posición de un recurso dentro de la lista de recursos.

```csharp
public static readonly Key<int, RscKey> Id;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Id.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


