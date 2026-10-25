---
title: "تعداد Timescale"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.Timescale. يحدد الخيارات التي توضح كيفية عرض مقياس الزمن في عروض مخطط جانت لاستخدام المهام أو استخدام الموارد عندما يتم تصدير المشروع إلى تنسيق رسومي."
type: docs
weight: 3430
url: /ar/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

يحدد الخيارات التي تحدد كيفية عرض مقياس الوقت في مخطط جانت أو عرض استخدام المهمة أو عرض استخدام الموارد عندما يتم تصدير المشروع إلى تنسيق رسومي.

```csharp
public enum Timescale
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DefinedInView | `0` | استخدم إعدادات مقياس الزمن المعرفة في خصائص عرض المشروع: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/)، [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/)، [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). صالحة للتنسيقات التي تحتوي على بيانات العرض. على سبيل المثال، المشاريع التي تُقرأ من تنسيق MPP. |
| Days | `1` | مقياس زمن مسبق التعريف ذو مستويين حيث الحد الأدنى للتفصيل هو يوم واحد. |
| ThirdsOfMonths | `10` | مقياس زمن مسبق التعريف ذو مستويين حيث مستوى التفصيل هو ثلث الشهر. |
| Months | `30` | مقياس زمن مسبق التعريف ذو مستويين حيث الحد الأدنى للتفصيل هو شهر واحد. |

## الأمثلة

يوضح كيفية حفظ المشروع كملف SVG.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // حدد <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> الذي سيتم حفظ المستند به
                            PresentationFormat = PresentationFormat.GanttChart,

                            // حدد قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف لتناسب محتواه.
                            FitContent = true,

                            // حدد الحد الأدنى للفترة الزمنية للعرض. القيمة الافتراضية هي <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // يحدد ما إذا كان يجب استخدام فرشاة تدرجية عند عرض تخطيط المشروع
                            // حاليًا لا يدعم استخدام الفرشاة التدرجية عند العرض إلى SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


