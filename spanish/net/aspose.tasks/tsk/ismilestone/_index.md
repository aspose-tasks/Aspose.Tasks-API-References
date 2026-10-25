---
title: "Tsk.IsMilestone"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea es un hito"
type: docs
weight: 630
url: /es/net/aspose.tasks/tsk/ismilestone/
---
## Tsk.IsMilestone field

Determina si una tarea es un hito.

```csharp
public static readonly Key<NullableBool, TaskKey> IsMilestone;
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


