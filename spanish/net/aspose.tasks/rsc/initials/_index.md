---
title: "Rsc.Initials"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Las iniciales de un recurso"
type: docs
weight: 370
url: /es/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

Las iniciales de un recurso.

```csharp
public static readonly Key<string, RscKey> Initials;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rrc.Initials.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


