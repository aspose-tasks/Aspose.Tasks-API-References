---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية HtmlSaveOptions. يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم استخدام فرشاة التدرج عند عرض تخطيط المشروع. حالياً لا يُدعم استخدام فرشاة التدرج عند العرض إلى HTML"
type: docs
weight: 160
url: /ar/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان سيتم استخدام فرشاة تدرجية عند عرض تخطيط المشروع. حاليًا لا يُدعم استخدام الفرشاة التدرجية عند العرض إلى HTML.

```csharp
public override bool UseGradientBrush { get; set; }
```

## الأمثلة

يوضح كيفية تعيين خط مخصص سيُستخدم لتصدير المشروع في ملف HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


