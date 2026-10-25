---
title: "GanttChartView.TopTimescaleTier"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GanttChartView. يحصل أو يعيّن إعدادات الطبقة العلوية لمقياس الوقت للعرض. TimescaleTier"
type: docs
weight: 190
url: /ar/net/aspose.tasks/ganttchartview/toptimescaletier/
---
## GanttChartView.TopTimescaleTier property

يحصل أو يضبط إعدادات مستوى الوقت العلوي للعرض. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
```

## الأمثلة

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

يعرض كيفية تخصيص تسميات طبقة مقياس الوقت.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// إضافة روابط المهام
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// ضبط طبقات مقياس الوقت

// ضبط الطبقة العليا
// ضبط الطبقة العليا لمقياس الوقت في عرض مخطط جانت.
view.MiddleTimescaleTier = new TimescaleTier();
// ضبط وحدة مقياس الوقت <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> للطبقة الزمنية.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// ضبط الفاصل الزمني لوحدة الوقت الذي تُظهر فيه التسميات للطبقة.
view.MiddleTimescaleTier.Count = 1;
// ضبط تسمية التاريخ <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> للطبقة الزمنية.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// ضبط طريقة محاذاة التسميات داخل كل فترة زمنية للطبقة (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// تعيين قيمة تشير إلى ما إذا كان يجب إظهار علامات الفواصل التي تفصل الفترات الزمنية في المستوى.
view.MiddleTimescaleTier.ShowTicks = true;
// تعيين قيمة تشير إلى ما إذا كان يجب أن تستند تسميات المستوى إلى السنة المالية.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// تمت الإضافة لتحسين التصور.
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// تخصيص تواريخ المستوى الأوسط.
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// استخدم خيار 'Timescale.DefinedInView' لتصوير المقاييس الزمنية باستخدام إعدادات المقاييس الزمنية المعرفة في العرض (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### انظر أيضًا

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


