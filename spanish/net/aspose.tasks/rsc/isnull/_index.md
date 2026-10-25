---
title: "Rsc.IsNull"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Determina si un recurso es nulo"
type: docs
weight: 420
url: /es/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

Determina si un recurso es nulo.

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.IsNull.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


