---
title: "Project.RecalculateResourceStartFinish"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Project. Recalcula el inicio y fin de los recursos"
type: docs
weight: 1170
url: /es/net/aspose.tasks/project/recalculateresourcestartfinish/
---
## Project.RecalculateResourceStartFinish method

Recalcula el inicio y fin de los recursos.

```csharp
public void RecalculateResourceStartFinish()
```

## Ejemplos

Muestra cómo recalcular las fechas de inicio/fin de los recursos.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 26, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1d, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 3, 26, 17, 0, 0));

var resource = project.Resources.Add("Res1");
resource.Set(Rsc.Start, new DateTime(2020, 3, 26, 8, 0, 0));
resource.Set(Rsc.Finish, new DateTime(2020, 3, 26, 17, 0, 0));

var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 3, 25, 8, 0, 0));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 3, 27, 8, 0, 0));

Console.WriteLine("Resource Start (before): " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Finish (before): " + resource.Get(Rsc.Finish));

// Recalcula el inicio y fin de los recursos
project.RecalculateResourceStartFinish();

Console.WriteLine("Resource Start (after): " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Finish (after): " + resource.Get(Rsc.Finish));
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


