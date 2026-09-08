---
title: "Clase SplitPart"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.SplitPart. Representa una porción de tarea. SplitPart es un miembro de la colección SplitParts de tareas."
type: docs
weight: 2290
url: /es/net/aspose.tasks/splitpart/
---
## SplitPart class

Representa una porción de tarea. SplitPart es un miembro de la colección SplitParts de la tarea.

```csharp
public class SplitPart
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Finish](../../aspose.tasks/splitpart/finish/) { get; } | Obtiene la fecha de finalización de un SplitPart. |
| [Start](../../aspose.tasks/splitpart/start/) { get; } | Obtiene la fecha de inicio de un SplitPart. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.tasks/splitpart/equals/)(object) | Compara dos partes divididas. |
| override [GetHashCode](../../aspose.tasks/splitpart/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase `SplitPart`. |

## Ejemplos

Muestra cómo trabajar con partes divididas de una tarea dividida.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// debe generar primero los datos faseados de asignación de recursos
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// dividir la tarea.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// iterar sobre partes divididas
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


