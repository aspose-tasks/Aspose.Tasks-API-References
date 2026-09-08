---
title: "Resource.Baselines"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Resource. Obtiene una instancia de BaselineCollection para este objeto. Los valores de referencia para un recurso"
type: docs
weight: 160
url: /es/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

Obtiene una instancia de BaselineCollection para este objeto. Los valores de línea base para un recurso.

```csharp
public BaselineCollection Baselines { get; }
```

## Ejemplos

Muestra cómo leer las líneas base del recurso.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### Ver también

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


