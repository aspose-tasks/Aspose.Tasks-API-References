---
title: "Task.RecurringInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει το αντικείμενο της κλάσης RecurringTaskInfo για την εργασία που είναι επαναλαμβανόμενη εργασία· εάν η εργασία δεν είναι επαναλαμβανόμενη, τότε επιστρέφει null. Οι πληροφορίες για το αντικείμενο της RecurringTaskInfo είναι διαθέσιμες μόνο σε μορφή αρχείου mpp."
type: docs
weight: 1030
url: /el/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

Λαμβάνει το αντικείμενο της κλάσης [`RecurringTaskInfo`](../../recurringtaskinfo/) για την εργασία που είναι επαναλαμβανόμενη εργασία· εάν η εργασία δεν είναι επαναλαμβανόμενη, τότε επιστρέφει null· Οι πληροφορίες για το αντικείμενο της [`RecurringTaskInfo`](../../recurringtaskinfo/) είναι διαθέσιμες μόνο σε μορφή αρχείου mpp.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις επαναλαμβανόμενες πληροφορίες της εργασίας.

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

### Δείτε επίσης

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


