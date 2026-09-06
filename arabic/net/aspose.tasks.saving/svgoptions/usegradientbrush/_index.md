---
title: "SvgOptions.UseGradientBrush"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SvgOptions. تحدد ما إذا كان يجب استخدام فرشاة تدرج لوني عند عرض تخطيط المشروع. حاليًا لا يُدعم استخدام فرشاة التدرج للعرض إلى SVG"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/svgoptions/usegradientbrush/
---
## SvgOptions.UseGradientBrush property

يحدد ما إذا كان يجب استخدام فرشاة تدرجية عند عرض تخطيط المشروع. حاليًا لا يدعم استخدام الفرشاة التدرجية عند العرض إلى SVG.

```csharp
public override bool UseGradientBrush { get; set; }
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


