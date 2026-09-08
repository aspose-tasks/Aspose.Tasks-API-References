---
title: "Rsc.Uid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El identificador único de un recurso"
type: docs
weight: 670
url: /es/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

El identificador único de un recurso.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Uid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


