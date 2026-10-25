---
title: "Rsc.OvertimeCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El costo total de horas extra para un recurso en todas las tareas asignadas"
type: docs
weight: 500
url: /es/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

El costo total de horas extra para un recurso en todas las tareas asignadas.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## Ejemplos

Muestra cómo leer los valores de horas extra del recurso.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Mostrar parámetros relacionados con horas extra para todos los recursos
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


