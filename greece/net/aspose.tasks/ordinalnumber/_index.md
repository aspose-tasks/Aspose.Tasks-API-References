---
title: "Απαρίθμηση OrdinalNumber"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.OrdinalNumber. Αντιπροσωπεύει έναν αριθμό σειράς στην περίπτωση της κλάσης RecurringTaskInfo"
type: docs
weight: 1140
url: /el/net/aspose.tasks/ordinalnumber/
---
## OrdinalNumber enumeration

Αντιπροσωπεύει έναν αριθμό σειράς στην περίπτωση της κλάσης [`RecurringTaskInfo`](../recurringtaskinfo/).

```csharp
public enum OrdinalNumber
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| First | `1` | Το πρώτο στοιχείο. |
| Second | `2` | Το δεύτερο στοιχείο. |
| Third | `3` | Το τρίτο στοιχείο. |
| Fourth | `4` | Το τέταρτο στοιχείο. |
| Last | `5` | Το τελευταίο στοιχείο. |

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε τις επαναλαμβανόμενες πληροφορίες των εργασιών.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// διαβάστε τις επαναλαμβανόμενες πληροφορίες των εργασιών
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    var info = task.RecurringInfo;
    if (info == null)
    {
        continue;
    }

    Console.WriteLine("Start Date: " + info.StartDate);
    Console.WriteLine("Duration: " + info.Duration);
    Console.WriteLine("End Date: " + info.EndDate);
    Console.WriteLine("Daily Repetitions: " + info.DailyRepetitions);
    Console.WriteLine("Daily Use Workdays: " + info.DailyUseWorkdays);
    Console.WriteLine("Monthly Day: " + info.MonthlyDay);
    Console.WriteLine("Monthly Ordinal Day: " + info.MonthlyOrdinalDay);
    Console.WriteLine("Monthly Ordinal Number: " + info.MonthlyOrdinalNumber);
    Console.WriteLine("Monthly Ordinal Repetitions: " + info.MonthlyOrdinalRepetitions);
    Console.WriteLine("Monthly Repetitions: " + info.MonthlyRepetitions);
    Console.WriteLine("Monthly Use Ordinal Day: " + info.MonthlyUseOrdinalDay);
    Console.WriteLine("Occurrences: " + info.Occurrences);
    Console.WriteLine("Recurrence Pattern: " + info.RecurrencePattern);
    Console.WriteLine("Parent Task: " + info.Task.Get(Tsk.Name));
    Console.WriteLine("Use End Date: " + info.UseEndDate);
    Console.WriteLine("Weekly Days: " + info.WeeklyDays);
    Console.WriteLine("Weekly Repetitions: " + info.WeeklyRepetitions);
    Console.WriteLine("Yearly Date: " + info.YearlyDate);
    Console.WriteLine("Yearly Ordinal Day: " + info.YearlyOrdinalDay);
    Console.WriteLine("Yearly Ordinal Month: " + info.YearlyOrdinalMonth);
    Console.WriteLine("Yearly Ordinal Number: " + info.YearlyOrdinalNumber);
    Console.WriteLine("Yearly Use Ordinal Day: " + info.YearlyUseOrdinalDay);
    Console.WriteLine();
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


