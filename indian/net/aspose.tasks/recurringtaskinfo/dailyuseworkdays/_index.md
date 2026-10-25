---
title: "RecurringTaskInfo.DailyUseWorkdays"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RecurringTaskInfo प्रॉपर्टी। मान प्राप्त करता है या सेट करता है जो दर्शाता है कि दैनिक पुनरावृत्ति पैटर्न के लिए कार्यदिवसों का उपयोग करना है या नहीं।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/recurringtaskinfo/dailyuseworkdays/
---
## RecurringTaskInfo.DailyUseWorkdays property

दैनिक आवृत्ति पैटर्न के लिए कार्यदिवसों का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool DailyUseWorkdays { get; set; }
```

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

* class [RecurringTaskInfo](../)
* namespace [Aspose.Tasks](../../recurringtaskinfo/)
* assembly [Aspose.Tasks](../../../)


