---
title: "Task.RecurringInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene l'istanza della classe RecurringTaskInfo per l'attività che è un'attività ricorrente; se l'attività non è ricorrente restituisce null. Le informazioni per l'istanza di RecurringTaskInfo sono presenti solo nel formato file mpp"
type: docs
weight: 1030
url: /it/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

Ottiene l'istanza della classe [`RecurringTaskInfo`](../../recurringtaskinfo/) per l'attività che è un'attività ricorrente; se l'attività non è ricorrente restituisce null; le informazioni per l'istanza di [`RecurringTaskInfo`](../../recurringtaskinfo/) sono presenti solo nel formato file mpp.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## Esempi

Mostra come leggere le informazioni ricorrenti dell'attività.

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

### Vedi anche

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


