---
title: "SvgOptions.SvgOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ SvgOptions. يهيئ مثيلاً جديداً لفئة SvgOptions يمكن استخدامها لحفظ المشروع بصيغة SVG"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/svgoptions/svgoptions/
---
## SvgOptions constructor

يهيئ مثيلاً جديداً لفئة [`SvgOptions`](../) يمكن استخدامها لحفظ المشروع بصيغة SVG.

```csharp
public SvgOptions()
```

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

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


