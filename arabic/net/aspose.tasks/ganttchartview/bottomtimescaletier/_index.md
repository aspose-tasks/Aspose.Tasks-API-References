---
title: "GanttChartView.BottomTimescaleTier"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GanttChartView. يحصل أو يعيّن إعدادات الطبقة السفلية لمقياس الوقت للعرض. TimescaleTier"
type: docs
weight: 60
url: /ar/net/aspose.tasks/ganttchartview/bottomtimescaletier/
---
## GanttChartView.BottomTimescaleTier property

يحصل أو يضبط إعدادات مستوى الوقت السفلي للعرض. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/)

```csharp
public TimescaleTier BottomTimescaleTier { get; set; }
```

## الأمثلة

يوضح كيفية العمل مع مستويات مقياس الوقت من خلال خيارات الحفظ.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

GanttChartView ganttChartView = (GanttChartView) project.Views.ToList()[0];

// ضبط مستويات مقياس الوقت في عرض مخطط جانت
ganttChartView.MiddleTimescaleTier.Unit = TimescaleUnit.Months;
ganttChartView.MiddleTimescaleTier.Count = 1;
ganttChartView.MiddleTimescaleTier.Label = DateLabel.MonthMmmm;

ganttChartView.BottomTimescaleTier.Unit = TimescaleUnit.Days;
ganttChartView.BottomTimescaleTier.Count = 1;
ganttChartView.BottomTimescaleTier.Label = DateLabel.DayDddDd;

// ...
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    Timescale = Timescale.DefinedInView
};

// ...

// حفظ المشروع كصورة
project.Save(OutDir + "WorkWithTimescaleTier_out.png", options);
```

يوضح كيفية تعديل مستويات مقياس الوقت.

```csharp
var project = new Project();

// تهيئة عرض مخطط جانت
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// تعيين عدد مقياس الوقت
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// إضافة عرض مخطط جانت إلى المشروع
project.Views.Add(view);

// إضافة بعض بيانات الاختبار إلى المشروع
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// استخدم خيار 'Timescale.DefinedInView' لتصيير مقاييس الوقت باستخدام إعدادات مقياس الوقت التي قمنا بتعيينها (view.TopTimescaleTier، view.MiddleTimescaleTier، view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### انظر أيضًا

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


