---
title: "Rsc.BCWP"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El costo presupuestado de un trabajo realizado por un recurso para el proyecto hasta la fecha"
type: docs
weight: 140
url: /es/net/aspose.tasks/rsc/bcwp/
---
## Rsc.BCWP field

El costo presupuestado de un trabajo realizado por un recurso para el proyecto hasta la fecha.

```csharp
public static readonly Key<double, RscKey> BCWP;
```

## Ejemplos

Muestra cómo leer los costos de los recursos.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// Mostrar todos los costos de los recursos
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


