---
title: "RecurringInterval.MonthlyDay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية RecurringInterval. تحصل أو تعيين قيمة تشير إلى ما إذا كان يجب عرض خطوط التقدم الشهرية حسب اليوم"
type: docs
weight: 50
url: /ar/net/aspose.tasks.visualization/recurringinterval/monthlyday/
---
## RecurringInterval.MonthlyDay property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض خطوط التقدم الشهرية حسب اليوم.

```csharp
public bool MonthlyDay { get; set; }
```

## الأمثلة

يوضح كيفية العمل مع الفاصل المتكرر لخطوط التقدم.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// يسمح بقراءة خط التقدم
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// يسمح بإعادة تعريف الفاصل المتكرر
var newInterval = new RecurringInterval();

// تعيين قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم الشهرية حسب اليوم.
interval.MonthlyDay = true;
// تعيين رقم اليوم لخطوط التقدم الشهرية.
interval.MonthlyDayDayNumber = 1;
// تعيين رقم الشهر لخطوط التقدم الشهرية.
interval.MonthlyDayMonthNumber = 1;
// تعيين قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم حسب اليوم الأول أو الأخير المحدد مسبقًا.
interval.MonthlyFirstLast = true;
// تعيين نوع اليوم الأول أو الأخير لخطوط التقدم الشهرية.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// تعيين رقم الشهر لخطوط التقدم التي تُعرض حسب اليوم الأول أو الأخير المحدد مسبقًا.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### انظر أيضًا

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


