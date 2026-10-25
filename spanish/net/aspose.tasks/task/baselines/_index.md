---
title: "Task.Baselines"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Task. Obtiene o establece la colección de valores de línea base de la tarea"
type: docs
weight: 130
url: /es/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

Obtiene o establece la colección de valores de línea base de la tarea.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## Ejemplos

Muestra cómo leer las líneas base de la tarea.

```csharp
var project = new Project();

// establecer una línea base
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Mostrar duración de la línea base de la tarea
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### Ver también

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


