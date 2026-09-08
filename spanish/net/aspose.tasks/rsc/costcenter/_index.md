---
title: "Rsc.CostCenter"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Indica a qué centro de costos se deben cargar los costos acumulados por el recurso"
type: docs
weight: 230
url: /es/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

Indica a qué centro de costos se deben cargar los costos acumulados por el recurso.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.CostCenter.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


