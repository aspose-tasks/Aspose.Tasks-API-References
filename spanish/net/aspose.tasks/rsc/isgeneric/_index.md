---
title: "Rsc.IsGeneric"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Determina si un recurso es genérico o no"
type: docs
weight: 410
url: /es/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

Determina si un recurso es genérico o no.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.IsGeneric.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


