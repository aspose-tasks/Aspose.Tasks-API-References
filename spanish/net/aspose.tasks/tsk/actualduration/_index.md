---
title: "Tsk.ActualDuration"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El período de tiempo de trabajo real para una tarea basado en la duración programada y el trabajo restante actual o el porcentaje completado."
type: docs
weight: 30
url: /es/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

El período de tiempo de trabajo real para una tarea, basado en la duración programada y el trabajo restante actual o el porcentaje completado.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


