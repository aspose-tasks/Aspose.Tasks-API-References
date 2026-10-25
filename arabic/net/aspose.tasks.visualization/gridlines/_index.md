---
title: "فئة Gridlines"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Visualization.Gridlines. تمثل خطوط الشبكة التي تظهر في عرض GanttChart."
type: docs
weight: 3120
url: /ar/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

يمثل خطوط الشبكة التي تظهر في عرض مخطط جانت.

```csharp
public class Gridlines
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Gridlines](gridlines/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | يحصل أو يعيّن الرقم من 0 إلى 99 الذي يحدد الفاصل بين خطوط الشبكة. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | يحصل أو يعيّن لون خطوط الشبكة الثانوية. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | يحصل أو يضبط نمط الخط لخطوط الشبكة الثانوية. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | يحصل أو يضبط لون خطوط الشبكة العادية. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | يحصل أو يضبط نمط الخط لخطوط الشبكة العادية. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | يحصل أو يضبط نوع خط الشبكة. |

## الأمثلة

يعرض كيفية العمل مع خطوط الشبكة.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// يسمح بضبط أول خط شبكة في العرض
var gridlines = view.Gridlines[0];
// اضبط الرقم من 0 إلى 99 الذي يحدد الفاصل بين خطوط الشبكة.
gridlines.Interval = 2;
// اضبط لون خطوط الشبكة الثانوية.
gridlines.IntervalColor = Color.Red;
// اضبط نمط الخط لخطوط الشبكة الثانوية
gridlines.IntervalPattern = LinePattern.Solid;
// اضبط لون خطوط الشبكة العادية
gridlines.NormalColor = Color.Blue;
// اضبط نمط الخط لخطوط الشبكة العادية
gridlines.NormalPattern = LinePattern.CloseDot;
// اضبط نوع خط الشبكة
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


