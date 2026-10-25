---
title: "Task.RecurringInfo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Tekrarlayan bir görev olan görev için RecurringTaskInfo sınıfının örneğini alır; görev tekrarlayan bir görev değilse null döndürür. RecurringTaskInfo örneğiyle ilgili bilgi yalnızca mpp dosya formatında bulunur."
type: docs
weight: 1030
url: /tr/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

Görev için tekrarlayan bir görev olan [`RecurringTaskInfo`](../../recurringtaskinfo/) sınıfının örneğini alır; görev tekrarlayan bir görev değilse null döndürür; [`RecurringTaskInfo`](../../recurringtaskinfo/) örneğiyle ilgili bilgi yalnızca mpp dosya formatında bulunur.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## Örnekler

Görev'in yinelenen bilgilerini nasıl okuyacağınızı gösterir.

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

### Ayrıca Bakınız

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


