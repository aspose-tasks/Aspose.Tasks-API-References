---
title: "ResourceAssignment.ToString"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceAssignment. Devuelve una representación corta en forma de cadena de la instancia de la clase ResourceAssignment. Los detalles exactos de la representación no están especificados y pueden cambiar"
type: docs
weight: 790
url: /es/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

Devuelve una representación corta en forma de cadena de la instancia de la clase [`ResourceAssignment`](../). Los detalles exactos de la representación no están especificados y pueden cambiar.

```csharp
public override string ToString()
```

### Valor devuelto

cadena corta que representa el objeto de asignación.

## Ejemplos

Muestra cómo imprimir información de asignación común.

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

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


