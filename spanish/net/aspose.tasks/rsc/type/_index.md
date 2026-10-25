---
title: "Rsc.Type"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El tipo de un recurso"
type: docs
weight: 660
url: /es/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

El tipo de un recurso.

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Type.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


