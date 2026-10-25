---
title: "TaskBaselineCollection.Count"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TaskBaselineCollection. Obtiene el número de objetos contenidos en este objeto TaskBaselineCollection."
type: docs
weight: 10
url: /es/net/aspose.tasks/taskbaselinecollection/count/
---
## TaskBaselineCollection.Count property

Obtiene el número de objetos contenidos en este objeto TaskBaselineCollection.

```csharp
public int Count { get; }
```

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

* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


