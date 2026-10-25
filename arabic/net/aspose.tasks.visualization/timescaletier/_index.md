---
title: "الفئة TimescaleTier"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.TimescaleTier. تمثل طبقة واحدة من مقياس الوقت في مخطط جانت"
type: docs
weight: 3450
url: /ar/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

يمثل مستوى واحد من مقياس الوقت في مخطط جانت.

```csharp
public sealed class TimescaleTier
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | ينشئ مثيلاً جديداً من الفئة `TimescaleTier`. |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | ينشئ مثيلاً جديداً من الفئة `TimescaleTier`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | يحصل أو يضبط طريقة محاذاة التسميات داخل كل فترة زمنية للطبقة ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | يحصل أو يضبط الفاصل الزمني لوحدة الوقت الذي تُظهر فيه التسميات للطبقة. القيمة الافتراضية هي 1. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | يحصل أو يضبط دالة رد الاتصال لمعالجة رسم علامة التاريخ في هذه الطبقة. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | يحصل أو يضبط تسمية التاريخ [`DateLabel`](../datelabel/) للطبقة الزمنية. |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | يحصل أو يضبط العلامة التي تحدد ما إذا كان يجب عرض تسميات التاريخ على كل صفحة عندما تمتد فترة زمنية على عدة صفحات. إذا كانت القيمة 'true'، عندما تمتد الفترة الزمنية على عدة صفحات، تُعرض تسميات التاريخ للفترة على كل صفحة. إذا كانت القيمة 'false'، تُعرض تسمية التاريخ مرة واحدة فقط وفقاً لقيمة خاصية [`Alignment`](./alignment/). |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب إظهار علامات الفواصل التي تفصل الفترات الزمنية في الطبقة. |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | يحصل أو يضبط وحدة مقياس الوقت [`TimescaleUnit`](../timescaleunit/) للطبقة الزمنية. القيمة الافتراضية هي [`Days`](../timescaleunit/). |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب اعتماد تسميات الطبقة على السنة المالية. |

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


