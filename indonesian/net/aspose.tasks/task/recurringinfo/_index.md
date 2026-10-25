---
title: "Task.RecurringInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan instance kelas RecurringTaskInfo untuk tugas yang merupakan tugas berulang; jika tugas bukan tugas berulang maka mengembalikan null. Info untuk instance RecurringTaskInfo hanya terdapat dalam format file mpp."
type: docs
weight: 1030
url: /id/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

Memperoleh instance kelas [`RecurringTaskInfo`](../../recurringtaskinfo/) untuk tugas yang merupakan tugas berulang; jika tugas bukan tugas berulang maka mengembalikan null; Informasi untuk instance [`RecurringTaskInfo`](../../recurringtaskinfo/) hanya tersedia dalam format file mpp.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## Contoh

Menampilkan cara membaca info berulang tugas.

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

### Lihat Juga

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


