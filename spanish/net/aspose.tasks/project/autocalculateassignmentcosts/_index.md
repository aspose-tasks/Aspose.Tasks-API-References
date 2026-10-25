---
title: "Project.AutoCalculateAssignmentCosts"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene o establece si el costo de asignación y el costo restante deben calcularse automáticamente usando el trabajo de asignaciones y las tarifas de recursos"
type: docs
weight: 70
url: /es/net/aspose.tasks/project/autocalculateassignmentcosts/
---
## Project.AutoCalculateAssignmentCosts property

Obtiene o establece si el costo de asignación y el costo restante deben calcularse automáticamente usando el trabajo de la asignación y las tarifas de recursos.

```csharp
public bool AutoCalculateAssignmentCosts { get; set; }
```

## Ejemplos

Muestra cómo desactivar el cálculo automático de los costos de asignación y establecer los costos de asignación explícitamente.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("New task");
task.Duration = project.GetDuration(TimeSpan.FromHours(15), TimeUnitType.Day);
var resource = project.Resources.Add("Resource");
resource.StandardRate = 10m;

var assignment = project.ResourceAssignments.Add(task, resource);

assignment.Work = project.GetDuration(TimeSpan.FromHours(12), TimeUnitType.Day);
assignment.ActualWork = project.GetDuration(TimeSpan.FromHours(3), TimeUnitType.Day);

Console.WriteLine("Now assignment's cost are auto calculated:");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);

project.AutoCalculateAssignmentCosts = false;
assignment.ActualCost = 123;
assignment.RemainingCost = 456;
assignment.Cost = 555;

Console.WriteLine("Now auto calculation of assignment's cost is turned off.");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


