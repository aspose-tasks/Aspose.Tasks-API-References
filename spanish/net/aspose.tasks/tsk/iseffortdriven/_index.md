---
title: "Tsk.IsEffortDriven"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si la programación de la tarea es programación basada en esfuerzo"
type: docs
weight: 570
url: /es/net/aspose.tasks/tsk/iseffortdriven/
---
## Tsk.IsEffortDriven field

Determina si la programación de la tarea es una programación basada en el esfuerzo.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEffortDriven;
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


