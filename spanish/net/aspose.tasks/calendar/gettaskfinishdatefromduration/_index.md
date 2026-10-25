---
title: "Calendar.GetTaskFinishDateFromDuration"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Calcula la fecha y hora de finalización de la tarea a partir de sus partes de fecha de inicio y la duración del trabajo"
type: docs
weight: 210
url: /es/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio, sus partes divididas y la duración del trabajo.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarea | Tarea | La tarea para la que se calcula la fecha de finalización. |
| duración | TimeSpan | La duración a calcular. |

### Valor devuelto

Fecha de finalización de la tarea para la fecha de inicio y duración dadas.

## Observaciones

Devuelve DateTime.MinValue si la tarea es resumen, nula o su fecha de inicio no está establecida.

## Ejemplos

Muestra cómo calcular la fecha de finalización de una tarea mediante una duración personalizada.

```csharp
var project = new Project(DataDir + "SplitTaskFinishDate.mpp");

// Buscar una tarea dividida
var task = project.RootTask.Children.GetByUid(4);

// Buscar el calendario del proyecto
var calendar = project.Get(Prj.Calendar);

// Calcular la fecha de finalización de la tarea con diferentes duraciones
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 8 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(8, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 16 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(16, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 24 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(24, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 28 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(28, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 32 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(32, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 46 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(46, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 61 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(61, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 75 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(75, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 80 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(80, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 120 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(120, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 150 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(150, 0, 0)));
```

### Ver también

* class [Task](../../task/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


