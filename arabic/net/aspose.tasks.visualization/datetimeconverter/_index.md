---
title: "المندوب DateTimeConverter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "يمثل طريقة محول لتحويل التاريخ إلى سلسلة في مستويات مقياس الوقت في العرض"
type: docs
weight: 2990
url: /ar/net/aspose.tasks.visualization/datetimeconverter/
---
## DateTimeConverter delegate

يمثل طريقة محول لتحويل التاريخ إلى سلسلة في مستويات مقياس الوقت في العرض.

```csharp
public delegate string DateTimeConverter(DateTime date);
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| التاريخ | DateTime | مثيل فئة DateTime للتحويل إلى سلسلة. |

### قيمة الإرجاع

تمثيل السلسلة للتاريخ المحدد.

## الأمثلة

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


