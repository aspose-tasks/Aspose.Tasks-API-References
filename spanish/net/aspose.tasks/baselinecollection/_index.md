---
title: "Clase BaselineCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.BaselineCollection. Representa una colección de objetos Baseline"
type: docs
weight: 120
url: /es/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

Representa una colección de objetos [`Baseline`](../baseline/).

```csharp
public class BaselineCollection : IList<Baseline>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | Obtiene el número de objetos contenidos en este objeto BaselineCollection. |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | Obtiene el [`Resource`](../resource/) padre de esta colección. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | Esta es la implementación de referencia del método Add de ICollection, que solo lanza NotSupportedException |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | Elimina la línea base de esta colección. |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | Convierte el objeto BaselineCollection en una lista de objetos [`Baseline`](../baseline/). |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


