---
title: "Rsc.Cost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El costo total programado o proyectado para un recurso basado en los costos ya incurridos por el trabajo realizado por los recursos asignados a las tareas, además de los costos planificados para el trabajo restante"
type: docs
weight: 220
url: /es/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

El costo total programado o proyectado para un recurso, basado en los costos ya incurridos por el trabajo realizado por los recursos asignados a las tareas, además de los costos planificados para el trabajo restante.

```csharp
public static readonly Key<decimal, RscKey> Cost;
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


