---
title: "Duration.TimeUnit"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Duration. Obtiene el tipo de unidad de tiempo para este objeto. El tipo de unidad de tiempo de esta instancia Duration."
type: docs
weight: 50
url: /es/net/aspose.tasks/duration/timeunit/
---
## Duration.TimeUnit property

Obtiene el tipo de unidad de tiempo para este objeto. El tipo de unidad de tiempo de esta instancia Duration.

```csharp
public TimeUnitType TimeUnit { get; }
```

## Ejemplos

Muestra cómo actualizar una duración de tareas.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// obtener una tarea
var task1 = project.RootTask.Children.GetById(1);

// actualizar la duración de la tarea
var duration1 = task1.Get(Tsk.Duration);

// agregar un día a la tarea 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// establecer una nueva duración a la tarea
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// obtener otra tarea
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// cambiar la duración usando el tipo de unidad de tiempo actual
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// establecer una nueva duración a la tarea
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Ver también

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


