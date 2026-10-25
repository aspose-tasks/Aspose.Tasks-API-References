---
title: "Rsc.SV"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. La variación del cronograma del valor ganado hasta la fecha de estado del proyecto. SV es la diferencia entre el costo presupuestado del trabajo realizado (BCWP) y el costo presupuestado del trabajo programado (BCWS)."
type: docs
weight: 650
url: /es/net/aspose.tasks/rsc/sv/
---
## Rsc.SV field

La variación del cronograma del valor ganado, hasta la fecha de estado del proyecto. SV es la diferencia entre el costo presupuestado del trabajo realizado (BCWP) y el costo presupuestado del trabajo programado (BCWS).

```csharp
public static readonly Key<double, RscKey> SV;
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


