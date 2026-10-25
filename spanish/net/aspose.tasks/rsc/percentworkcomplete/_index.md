---
title: "Rsc.PercentWorkComplete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El porcentaje de trabajo completado en todas las tareas"
type: docs
weight: 550
url: /es/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

El porcentaje de trabajo completado en todas las tareas.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## Ejemplos

Muestra cómo leer el porcentaje de trabajo completado del recurso.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// Mostrar el porcentaje de finalización del trabajo para todos los recursos
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


