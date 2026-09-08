---
title: "Task.RecurringInfo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task-eigenschap. Haalt de instantie van de klasse RecurringTaskInfo op voor de taak die een terugkerende taak is; als de taak geen terugkerende taak is, wordt null geretourneerd. De informatie voor de instantie van RecurringTaskInfo is alleen aanwezig in het mpp-bestandsformaat."
type: docs
weight: 1030
url: /nl/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

Haalt de instantie van de klasse [`RecurringTaskInfo`](../../recurringtaskinfo/) op voor de taak die een terugkerende taak is; als de taak geen terugkerende taak is, wordt null geretourneerd; De informatie voor de instantie van [`RecurringTaskInfo`](../../recurringtaskinfo/) is alleen aanwezig in het mpp-bestandsformaat.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## Voorbeelden

Toont hoe de terugkerende informatie van een taak te lezen is.

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

### Zie ook

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


