---
title: "Klasse RecurringTaskInfo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RecurringTaskInfo klasse. Vertegenwoordigt de details van een terugkerende taak in een project"
type: docs
weight: 1720
url: /nl/net/aspose.tasks/recurringtaskinfo/
---
## RecurringTaskInfo class

Stelt de details van een terugkerende taak in een project voor.

```csharp
public class RecurringTaskInfo
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DailyRepetitions](../../aspose.tasks/recurringtaskinfo/dailyrepetitions/) { get; set; } | Haalt het aantal herhalingen op of stelt dit in voor het dagelijkse terugkeerpatroon. |
| [DailyUseWorkdays](../../aspose.tasks/recurringtaskinfo/dailyuseworkdays/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of werkdagen moeten worden gebruikt voor het dagelijkse terugkeerpatroon. |
| [Duration](../../aspose.tasks/recurringtaskinfo/duration/) { get; set; } | Haalt de duur op of stelt deze in voor één voorkomen van de terugkerende taak. de instantie van de [`Duration`](./duration/) klasse. |
| [EndDate](../../aspose.tasks/recurringtaskinfo/enddate/) { get; set; } | Haalt de datum op of stelt deze in waarop de voorkomen moeten eindigen. |
| [MonthlyDay](../../aspose.tasks/recurringtaskinfo/monthlyday/) { get; set; } | Haalt het aantal dagen op of stelt dit in voor het maandelijkse terugkeerpatroon. |
| [MonthlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyordinalday/) { get; set; } | Haalt een dag op of stelt deze in voor het maandelijkse terugkeerpatroon bij gebruik van een ordinale dag. Kan een van de waarden van de DayOfWeek-enumeratie zijn. |
| [MonthlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/monthlyordinalnumber/) { get; set; } | Haalt een ordinaal getal op of stelt dit in voor het maandelijkse terugkeerpatroon. Kan een van de waarden van de [`OrdinalNumber`](../ordinalnumber/) enumeratie zijn. |
| [MonthlyOrdinalRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyordinalrepetitions/) { get; set; } | Haalt het aantal herhalingen op of stelt dit in voor het maandelijkse terugkeerpatroon bij gebruik van een ordinale dag. |
| [MonthlyRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyrepetitions/) { get; set; } | Haalt het aantal herhalingen op of stelt dit in voor het maandelijkse terugkeerpatroon. |
| [MonthlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyuseordinalday/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of een ordinale dag moet worden gebruikt voor het maandelijkse terugkeerpatroon. |
| [Occurrences](../../aspose.tasks/recurringtaskinfo/occurrences/) { get; set; } | Haalt het aantal voorkomen op of stelt dit in van de terugkerende taak. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskinfo/recurrencepattern/) { get; set; } | Haalt een terugkeerpatroon op of stelt dit in voor de terugkerende taak. Kan een van de waarden van de [`RecurrencePattern`](./recurrencepattern/) enumeratie zijn. |
| [StartDate](../../aspose.tasks/recurringtaskinfo/startdate/) { get; set; } | Haalt de datum op of stelt deze in waarop de voorkomen moeten beginnen. |
| [Task](../../aspose.tasks/recurringtaskinfo/task/) { get; } | Haalt de bovenliggende taak op van deze instantie van de `RecurringTaskInfo` klasse. |
| [UseEndDate](../../aspose.tasks/recurringtaskinfo/useenddate/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of de einddatum of een aantal herhalingen moet worden gebruikt voor de terugkerende taak. |
| [WeeklyDays](../../aspose.tasks/recurringtaskinfo/weeklydays/) { get; set; } | Haalt een collectie van dagen op of stelt deze in die worden gebruikt in het wekelijkse herhalingspatroon. |
| [WeeklyRepetitions](../../aspose.tasks/recurringtaskinfo/weeklyrepetitions/) { get; set; } | Haalt een aantal herhalingen op of stelt dit in voor het wekelijkse herhalingspatroon. |
| [YearlyDate](../../aspose.tasks/recurringtaskinfo/yearlydate/) { get; set; } | Haalt een datum op of stelt deze in voor het jaarlijkse herhalingspatroon. |
| [YearlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyordinalday/) { get; set; } | Haalt een weekdag op of stelt deze in van het jaarlijkse herhalingspatroon bij gebruik van een ordinale dag. Kan een van de waarden van de DayOfWeek‑enumeratie zijn. |
| [YearlyOrdinalMonth](../../aspose.tasks/recurringtaskinfo/yearlyordinalmonth/) { get; set; } | Haalt een maand op of stelt deze in van het jaarlijkse herhalingspatroon bij gebruik van een ordinale dag. Kan een van de waarden van de [`Month`](../month/)‑enumeratie zijn. |
| [YearlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/yearlyordinalnumber/) { get; set; } | Haalt een ordinaal getal op of stelt dit in van het jaarlijkse herhalingspatroon. Kan een van de waarden van de [`OrdinalNumber`](../ordinalnumber/)‑enumeratie zijn. |
| [YearlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyuseordinalday/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of een ordinale dag moet worden gebruikt voor het jaarlijkse herhalingspatroon. |

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


