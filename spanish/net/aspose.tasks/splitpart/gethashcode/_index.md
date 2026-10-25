---
title: "SplitPart.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método SplitPart. Devuelve un valor de código hash para la instancia de la clase SplitPart."
type: docs
weight: 40
url: /es/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

Devuelve un valor de código hash para la instancia de la clase [`SplitPart`](../).

```csharp
public override int GetHashCode()
```

### Valor devuelto

devuelve un valor de código hash para este objeto.

## Ejemplos

Muestra cómo obtener un código hash de una parte dividida.

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

// La igualdad de las partes divididas se verifica respecto al inicio, fin e índice de las partes divididas.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// El código hash de una parte dividida basado en el inicio, fin e índice de una parte dividida.
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### Ver también

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


