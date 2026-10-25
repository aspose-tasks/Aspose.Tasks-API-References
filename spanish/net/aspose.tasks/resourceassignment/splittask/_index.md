---
title: "ResourceAssignment.SplitTask"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceAssignment. Divide la tarea en dos partes"
type: docs
weight: 770
url: /es/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Divide la tarea en dos partes.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | El comienzo de la interrupción del trabajo en la que basar la división. |
| finalizar | DateTime | El final de la interrupción del trabajo en la que basar la división. |
| calendario | Calendar | El calendario en el que basar la división. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | Lanza una excepción cuando la fecha de inicio es menor que la fecha de inicio de la asignación. |
| ArgumentOutOfRangeException | Lanza una excepción cuando la fecha de finalización es mayor que la fecha de finalización de la asignación. |

## Ejemplos

Muestra cómo agregar una división a una tarea.

```csharp
var project = new Project();

// Obtener un calendario estándar
var calendar = project.Get(Prj.Calendar);

// Establecer la configuración del calendario del proyecto
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// Agregar una nueva tarea a la tarea raíz
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// Crear una nueva asignación de recurso y generar datos por fases de tiempo
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// Dividir la tarea en 3 partes.
// Proporcionar argumentos de fecha de inicio y fecha de finalización al método SplitTask que se utilizarán para la división
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### Ver también

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


