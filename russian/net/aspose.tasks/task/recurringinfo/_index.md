---
title: "Task.RecurringInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Возвращает экземпляр класса RecurringTaskInfo для задачи, которая является повторяющейся; если задача не является повторяющейся, возвращает null. Информация об экземпляре RecurringTaskInfo присутствует только в формате файлов mpp."
type: docs
weight: 1030
url: /ru/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

Возвращает экземпляр класса [`RecurringTaskInfo`](../../recurringtaskinfo/) для задачи, которая является повторяющейся; если задача не является повторяющейся, возвращает null; Информация об экземпляре [`RecurringTaskInfo`](../../recurringtaskinfo/) присутствует только в формате файлов mpp.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## Примеры

Показывает, как читать информацию о повторяющихся задачах.

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

### См. также

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


