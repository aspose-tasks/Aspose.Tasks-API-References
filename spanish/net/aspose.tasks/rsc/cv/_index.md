---
title: "Rsc.CV"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La variación del costo del valor ganado hasta la fecha de estado del proyecto. CV es la diferencia entre el BCWP (costo presupuestado del trabajo realizado) de la tarea y el ACWP (costo real del trabajo realizado)."
type: docs
weight: 270
url: /es/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

La variación del costo del valor ganado, hasta la fecha de estado del proyecto. CV es la diferencia entre el BCWP (costo presupuestado del trabajo realizado) y el ACWP (costo real del trabajo realizado) de la tarea.

```csharp
public static readonly Key<double, RscKey> CV;
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


