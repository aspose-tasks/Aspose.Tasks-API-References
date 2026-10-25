---
title: "Clase TaskBaselineCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TaskBaselineCollection. Representa una colección de objetos TaskBaseline"
type: docs
weight: 2380
url: /es/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

Representa una colección de objetos [`TaskBaseline`](../taskbaseline/).

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | Obtiene el número de objetos contenidos en este objeto TaskBaselineCollection. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | Esta es la implementación de referencia del método Add de ICollection, que solo lanza NotSupportedException |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | Elimina la línea base de esta colección. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | Convierte el objeto TaskBaselineCollection en una lista de objetos [`TaskBaseline`](../taskbaseline/). |

## Ejemplos

Muestra cómo trabajar con colecciones de líneas base de tareas.

```csharp
var project = new Project();

// crear líneas base del proyecto
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// imprimir líneas base de tareas
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// lets clear all baselines
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### Ver también

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


