---
title: "فئة ProgressLines"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Visualization.ProgressLines. تمثل خطوط التقدم في عرض مخطط Gantt"
type: docs
weight: 3290
url: /ar/net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

يمثل خطوط التقدم في عرض مخطط جانت.

```csharp
public class ProgressLines
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ProgressLines](progresslines/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | الحصول أو تعيين التاريخ لعرض خطوط التقدم منه. |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | الحصول أو تعيين قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم من بداية تاريخ بدء المشروع. |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | الحصول أو تعيين تنسيق التاريخ ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | الحصول أو تعيين قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم في التاريخ الحالي. |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | الحصول أو تعيين قيمة تشير إلى ما إذا كان سيتم عرض خط التقدم على فترات متكررة. |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | الحصول أو تعيين قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم في التواريخ المحددة. |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | الحصول أو تعيين الخط المستخدم لتسمية خط التقدم. |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | الحصول أو تعيين قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم للخطة الأساسية أو الفعلية. |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | الحصول أو تعيين لون الخط لخط التقدم الحالي. |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | الحصول أو تعيين نمط الخط لخط التقدم الحالي. [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | الحصول أو تعيين لون الخط لخط التقدم الآخر. |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | الحصول أو تعيين نمط الخط لخط التقدم الآخر. |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | الحصول أو تعيين لون النقطة الأخرى للتقدم. |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | الحصول أو تعيين شكل نقطة التقدم لخط التقدم الآخر. |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | الحصول أو تعيين لون نقطة التقدم. |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | الحصول أو تعيين شكل نقطة التقدم. [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | الحصول أو تعيين الفاصل المتكرر. [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | يحصل على قائمة التواريخ المحددة لعرض خطوط التقدم لها. |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب عرض التاريخ لكل خط تقدم. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


