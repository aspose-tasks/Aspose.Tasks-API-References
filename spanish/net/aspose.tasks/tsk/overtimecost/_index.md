---
title: "Tsk.OvertimeCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El costo total de horas extra para una tarea de un recurso en todas las tareas asignadas o para una asignación de recurso"
type: docs
weight: 860
url: /es/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

El costo total de horas extra para una tarea, para un recurso en todas las tareas asignadas o para una asignación de recurso.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


