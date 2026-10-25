---
title: "SaveOptions.Timescale"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يحدد قيمة Timescale التي تُستخدم للتحكم في كيفية عرض المقياس الزمني إذا كان موجودًا عندما يتم حفظ المشروع بتنسيق رسومي."
type: docs
weight: 200
url: /ar/net/aspose.tasks.saving/saveoptions/timescale/
---
## SaveOptions.Timescale property

يحصل أو يحدد قيمة `Timescale` التي تُستخدم للتحكم في كيفية عرض المقياس الزمني (إذا كان موجودًا) عندما يتم حفظ المشروع بتنسيق رسومي.

```csharp
public Timescale Timescale { get; set; }
```

## الأمثلة

يوضح كيفية تعيين الفترة الزمنية الدنيا للعرض. القيمة الافتراضية هي <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// احفظ كصورة صفحة واحدة (Timescale.days بشكل افتراضي).
project.Save(OutDir + "NewProductDevDays_out.jpeg", new ImageSaveOptions(SaveFileFormat.Jpeg));

// احفظ كصورة صفحة واحدة (Timescale.ThirdsOfMonths).
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "NewProductDevThirdsOfMonths_out.jpeg", options);

// احفظ كصورة صفحة واحدة (Timescale.Months).
options.Timescale = Timescale.Months;
project.Save(OutDir + "NewProductDevMonths_out.jpeg", options);
```

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

يعرض كيفية عرض رؤية استخدام المهمة مع إعدادات مقياس الوقت المعرفة في إعدادات العرض.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// حدد SaveOptions وحدد أنه يجب استخدام إعدادات مقياس الزمن لـ TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
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

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


