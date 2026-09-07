---
title: "एन्यूम OrdinalNumber"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.OrdinalNumber एन्यूम। यह RecurringTaskInfo क्लास के उदाहरण में एक क्रमांक दर्शाता है"
type: docs
weight: 1140
url: /hi/net/aspose.tasks/ordinalnumber/
---
## OrdinalNumber enumeration

एक क्रमांक को दर्शाता है जो [`RecurringTaskInfo`](../recurringtaskinfo/) क्लास के उदाहरण में है।

```csharp
public enum OrdinalNumber
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| First | `1` | पहला तत्व। |
| Second | `2` | दूसरा तत्व। |
| Third | `3` | तीसरा तत्व। |
| Fourth | `4` | चौथा तत्व। |
| Last | `5` | अंतिम तत्व। |

## उदाहरण

कार्य की पुनरावर्ती जानकारी को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// कार्य की पुनरावर्ती जानकारी पढ़ें
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

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


