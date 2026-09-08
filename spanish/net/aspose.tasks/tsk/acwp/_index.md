---
title: "Tsk.ACWP"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Costos incurridos por el trabajo ya realizado en una tarea hasta la fecha de estado del proyecto o la fecha de hoy."
type: docs
weight: 110
url: /es/net/aspose.tasks/tsk/acwp/
---
## Tsk.ACWP field

Costos incurridos por el trabajo ya realizado en una tarea, hasta la fecha de estado del proyecto o la fecha de hoy.

```csharp
public static readonly Key<double, TaskKey> ACWP;
```

## Ejemplos

Muestra cómo leer los valores de costo de la tarea.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


