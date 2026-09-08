---
title: "Rsc.OvertimeWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La cantidad de tiempo extra programado que debe ser realizado por un recurso en una tarea y cobrado a las tarifas de tiempo extra de los recursos involucrados"
type: docs
weight: 530
url: /es/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

La cantidad de horas extra programada para ser realizada por un recurso en una tarea y cobrada a las tarifas de horas extra de los recursos involucrados.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


