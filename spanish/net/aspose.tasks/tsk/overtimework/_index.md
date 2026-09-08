---
title: "Tsk.OvertimeWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La cantidad de horas extra programadas para ser realizadas por todos los recursos asignados a una tarea."
type: docs
weight: 870
url: /es/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

La cantidad de horas extra programada para ser realizada por todos los recursos asignados a una tarea.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## Ejemplos

Muestra cómo leer las horas extra de la tarea.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// Leer horas extra y porcentaje de finalización de tareas
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // Establecer porcentaje completado
    task.Set(Tsk.PercentComplete, 100);
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


