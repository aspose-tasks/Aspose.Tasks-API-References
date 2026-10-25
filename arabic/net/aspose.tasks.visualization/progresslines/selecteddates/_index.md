---
title: "ProgressLines.SelectedDates"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ProgressLines. يحصل على قائمة التواريخ المختارة لعرض خطوط التقدم لها"
type: docs
weight: 190
url: /ar/net/aspose.tasks.visualization/progresslines/selecteddates/
---
## ProgressLines.SelectedDates property

يحصل على قائمة التواريخ المحددة لعرض خطوط التقدم لها.

```csharp
public List<DateTime> SelectedDates { get; }
```

## الأمثلة

يعرض كيفية العمل مع خطوط التقدم.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// لنُعرّف خط التقدم
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// حدد التاريخ لبدء عرض خطوط التقدم منه. لنحدد تاريخ حالة المشروع.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// حدد قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم من بداية تاريخ بدء المشروع
progressLines.BeginAtProjectStart = true;
// حدد تنسيق التاريخ (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />).
progressLines.DateFormat = DateLabel.DayDddd;
// حدد قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم عند التاريخ الحالي.
progressLines.DisplayAtCurrentDate = true;
// حدد قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم على فترات متكررة.
progressLines.DisplayAtRecurringIntervals = true;
// حدد قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم في التواريخ المحددة
progressLines.DisplaySelected = true;
// حدد قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم للخطة الأساسية أو الفعلية.
progressLines.IsBaselinePlan = false;
// حدد الخط المستخدم لتسمية خط التقدم.
progressLines.Font = new FontDescriptor("Arial", 10);
// حدد لون الخط لخط التقدم الحالي.
progressLines.LineColor = Color.Aquamarine;
// حدد نمط الخط لخط التقدم الحالي.
progressLines.LinePattern = LinePattern.Dashed;
// حدد لون الخط لخط التقدم الآخر.
progressLines.OtherLineColor = Color.Azure;
// حدد نمط الخط لخط التقدم الآخر.
progressLines.OtherLinePattern = LinePattern.Dotted;
// حدد لون النقطة التقدمية الأخرى.
progressLines.OtherProgressPointColor = Color.Red;
// حدد شكل نقطة التقدم لخط التقدم الآخر.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// حدد لون نقطة التقدم.
progressLines.ProgressPointColor = Color.Orange;
// ضبط شكل نقطة التقدم.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// ضبط الفاصل المتكرر.
progressLines.RecurringInterval = new RecurringInterval();
// ضبط الفاصل المتكرر.
progressLines.RecurringInterval.Interval = Interval.Daily;
// ضبط رقم اليوم اليومي
progressLines.RecurringInterval.DailyDayNumber = 1;
// ضبط قيمة تشير إلى ما إذا كان يجب إظهار التاريخ لكل سطر تقدم.
progressLines.ShowDate = true;

// دعنا نتحقق من خطوط التقدم
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [ProgressLines](../)
* namespace [Aspose.Tasks.Visualization](../../progresslines/)
* assembly [Aspose.Tasks](../../../)


