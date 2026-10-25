---
title: "Tsk.IsCritical"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea está en la ruta crítica"
type: docs
weight: 560
url: /es/net/aspose.tasks/tsk/iscritical/
---
## Tsk.IsCritical field

Determina si una tarea está en la ruta crítica.

```csharp
public static readonly Key<NullableBool, TaskKey> IsCritical;
```

## Ejemplos

Muestra cómo encontrar tareas críticas y/o basadas en esfuerzo.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizar todas las tareas recopiladas
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


