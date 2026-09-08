---
title: "Enum OrdinalNumber"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OrdinalNumber enum. Vertegenwoordigt een ordinaal getal in de instantie van de RecurringTaskInfo klasse"
type: docs
weight: 1140
url: /nl/net/aspose.tasks/ordinalnumber/
---
## OrdinalNumber enumeration

Vertegenwoordigt een ordinaal getal in de instantie van de [`RecurringTaskInfo`](../recurringtaskinfo/) klasse.

```csharp
public enum OrdinalNumber
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| First | `1` | Het eerste element. |
| Second | `2` | Het tweede element. |
| Third | `3` | Het derde element. |
| Fourth | `4` | Het vierde element. |
| Last | `5` | Het laatste element. |

## Voorbeelden

Toont hoe de terugkerende informatie van taken kan worden gelezen.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// lees terugkerende informatie van taken
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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


