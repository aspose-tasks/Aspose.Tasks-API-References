---
title: "Tsk.IsEstimated"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea está estimada"
type: docs
weight: 580
url: /es/net/aspose.tasks/tsk/isestimated/
---
## Tsk.IsEstimated field

Determina si una tarea está estimada.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEstimated;
```

## Ejemplos

Muestra cómo encontrar tareas estimadas y/o hitos.

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// Iterar sobre las tareas recopiladas
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


