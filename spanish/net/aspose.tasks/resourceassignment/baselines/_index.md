---
title: "ResourceAssignment.Baselines"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ResourceAssignment propiedad. Obtiene el objeto AssignmentBaselineCollection. La colección de valores de línea base asociados a una asignación"
type: docs
weight: 120
url: /es/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

Obtiene el objeto AssignmentBaselineCollection. La colección de valores de línea base asociados a una asignación.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## Ejemplos

Muestra cómo obtener acceso a las líneas base de la asignación.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

project.SetBaseline(BaselineType.Baseline);

foreach (var assignmentBaseline in resourceAssignment.Baselines)
{
    Console.WriteLine("Baseline Start: {0}", assignmentBaseline.Start);
    Console.WriteLine("Baseline Finish: {0}", assignmentBaseline.Finish);
}
```

### Ver también

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


