---
title: "Task.RecurringInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Task. Obtiene la instancia de la clase RecurringTaskInfo para la tarea que es una tarea recurrente; si la tarea no es recurrente, devuelve null. La información de la instancia de RecurringTaskInfo está presente solo en el formato de archivo mpp"
type: docs
weight: 1030
url: /es/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

Obtiene la instancia de la clase [`RecurringTaskInfo`](../../recurringtaskinfo/) para la tarea que es una tarea recurrente; si la tarea no es recurrente, devuelve null; La información de la instancia de [`RecurringTaskInfo`](../../recurringtaskinfo/) está presente solo en el formato de archivo mpp.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## Ejemplos

Muestra cómo leer la información recurrente de la tarea.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Recurrence Pattern: " + task.RecurringInfo.RecurrencePattern);
Console.WriteLine("Start Date: " + task.RecurringInfo.StartDate);
Console.WriteLine("End Date: " + task.RecurringInfo.EndDate);
Console.WriteLine("Duration: " + task.RecurringInfo.Duration);
Console.WriteLine("Occurrences: " + task.RecurringInfo.Occurrences);
Console.WriteLine("Weekly Days: " + task.RecurringInfo.WeeklyDays);
Console.WriteLine("WeeklyRepetitions: " + task.RecurringInfo.WeeklyRepetitions);
```

### Ver también

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


