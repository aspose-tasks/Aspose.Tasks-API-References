---
title: "GanttChartView.Gridlines"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GanttChartView. يحصل أو يعيّن قائمة من خطوط الشبكة لعرض مخطط جانت."
type: docs
weight: 80
url: /ar/net/aspose.tasks/ganttchartview/gridlines/
---
## GanttChartView.Gridlines property

يحصل أو يعيّن قائمة من `Gridlines` لعرض مخطط جانت.

```csharp
public List<Gridlines> Gridlines { get; set; }
```

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

* class [Gridlines](../../../aspose.tasks.visualization/gridlines/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


