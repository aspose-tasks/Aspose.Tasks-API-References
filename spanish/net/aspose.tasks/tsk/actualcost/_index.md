---
title: "Tsk.ActualCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Costos incurridos por el trabajo ya realizado por los recursos en sus tareas junto con cualquier otro costo registrado asociado a la tarea"
type: docs
weight: 20
url: /es/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

Costos incurridos por el trabajo ya realizado por los recursos en sus tareas, junto con cualquier otro costo registrado asociado a la tarea.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
```

## Ejemplos

Muestra cómo leer las propiedades reales de la tarea.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizar todas las tareas recopiladas
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


