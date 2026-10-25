---
title: "BaselineCollection.Count"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de BaselineCollection. Obtiene el número de objetos contenidos en este objeto BaselineCollection"
type: docs
weight: 10
url: /es/net/aspose.tasks/baselinecollection/count/
---
## BaselineCollection.Count property

Obtiene el número de objetos contenidos en este objeto BaselineCollection.

```csharp
public int Count { get; }
```

## Ejemplos

Muestra cómo trabajar con colecciones de baseline.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// leer información de baseline
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### Ver también

* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


