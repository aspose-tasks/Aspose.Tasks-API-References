---
title: "Tsk.BCWS"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Los costos acumulados de la línea base por fase de tiempo hasta la fecha de estado o la fecha actual"
type: docs
weight: 130
url: /es/net/aspose.tasks/tsk/bcws/
---
## Tsk.BCWS field

Los costos acumulados de línea base faseados en el tiempo hasta la fecha de estado o la fecha de hoy.

```csharp
public static readonly Key<double, TaskKey> BCWS;
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


