---
title: "تعداد TimescaleUnit"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.TimescaleUnit. يحدد وحدة الوقت لأي مستوى من مقياس الزمن في مخطط جانت أو أي عرض زمني مرحلي آخر."
type: docs
weight: 3460
url: /ar/net/aspose.tasks.visualization/timescaleunit/
---
## TimescaleUnit enumeration

يحدد وحدة الوقت لأي طبقة من مقياس الوقت في مخطط جانت أو أي عرض زمني مرحلي آخر.

```csharp
public enum TimescaleUnit
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `-1` | يشير إلى لا شيء. مستوى مقياس الزمن مخفي. |
| Minutes | `0` | يشير إلى وحدة مقياس الزمن بالدقائق. |
| Hours | `1` | يشير إلى وحدة مقياس الزمن بالساعات. |
| Days | `2` | يشير إلى وحدة مقياس الزمن بالأيام. |
| Weeks | `3` | يشير إلى وحدة مقياس الزمن بالأسابيع. |
| ThirdsOfMonths | `4` | يشير إلى وحدة مقياس الزمن بأثلاث الشهور. |
| Months | `5` | يشير إلى وحدة مقياس الزمن بالشهور. |
| Quarters | `6` | يشير إلى وحدة مقياس الزمن بأرباع السنوات. |
| HalfYears | `7` | يشير إلى وحدة مقياس الزمن بنصف السنة. |
| Years | `8` | يشير إلى وحدة مقياس الزمن بالسنوات. |

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


