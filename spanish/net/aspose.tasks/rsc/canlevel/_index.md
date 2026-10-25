---
title: "Rsc.CanLevel"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Determina si se puede aplicar nivelación de recursos a un recurso"
type: docs
weight: 200
url: /es/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

Determina si se puede aplicar nivelación de recursos a un recurso.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.CanLevel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


