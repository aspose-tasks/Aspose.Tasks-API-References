---
title: "Tsk.Calendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El calendario de la tarea"
type: docs
weight: 160
url: /es/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

El calendario de la tarea.

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## Ejemplos

Muestra cómo leer/escribir calendarios de tareas.

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// Crear calendario y asignarlo a la tarea
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizar todos los hijos recursivos
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


