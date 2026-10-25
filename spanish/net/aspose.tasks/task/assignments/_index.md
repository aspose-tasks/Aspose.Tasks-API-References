---
title: "Task.Assignments"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Task. Obtiene una colección de asignaciones de recursos para este objeto"
type: docs
weight: 120
url: /es/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

Obtiene una colección de asignaciones de recursos para este objeto.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Ejemplos

Muestra cómo iterar sobre las asignaciones de la tarea.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // mostrar asignaciones de la tarea
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Ver también

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


