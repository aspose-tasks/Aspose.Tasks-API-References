---
title: "الفئة RecurringInterval"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.RecurringInterval. تمثل الفواصل المتكررة المستخدمة في خطوط التقدم في عرض مخطط جانت."
type: docs
weight: 3310
url: /ar/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

يمثل الفواصل المتكررة المستخدمة في خطوط التقدم في عرض مخطط جانت.

```csharp
public class RecurringInterval
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | يحصل أو يعيّن رقم اليوم اليومي. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان اليوم يوم عمل لخطوط التقدم اليومية. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | يحصل أو يعيّن الفاصل المتكرر. يمكن أن يكون أي قيمة من نوع [`Interval`](./interval/). |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض خطوط التقدم الشهرية حسب اليوم. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | يحصل أو يعيّن رقم اليوم لخطوط التقدم الشهرية. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | يحصل أو يعيّن رقم الشهر لخطوط التقدم الشهرية. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض خطوط التقدم وفقًا لأول يوم أو آخر يوم محدد مسبقًا. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | يحصل أو يعيّن نوع اليوم الأول أو الأخير لخطوط التقدم الشهرية. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | يحصل أو يعيّن رقم الشهر لخطوط التقدم، التي تُعرض وفقًا لأول يوم أو آخر يوم محدد مسبقًا. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | يحصل على قائمة بالأيام لخطوط التقدم الأسبوعية. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | يحصل أو يعيّن رقم الأسبوع لخطوط التقدم الأسبوعية. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


