---
title: "Rsc.Created"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La fecha y hora en que un recurso fue añadido al proyecto"
type: docs
weight: 260
url: /es/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

La fecha y hora en que un recurso fue añadido al proyecto.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Created.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


