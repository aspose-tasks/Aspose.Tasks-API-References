---
title: "TaskBaselineCollection.Remove"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de TaskBaselineCollection. Elimina la línea base de esta colección"
type: docs
weight: 50
url: /es/net/aspose.tasks/taskbaselinecollection/remove/
---
## TaskBaselineCollection.Remove method

Elimina la línea base de esta colección.

```csharp
public bool Remove(TaskBaseline item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | TaskBaseline | El elemento a eliminar. |

### Valor devuelto

true si el elemento se ha eliminado correctamente; de lo contrario, false

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

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


