---
title: "FontSettings.UseProjectDefaultFont"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية FontSettings. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب استخدام الخط الافتراضي للعرض."
type: docs
weight: 40
url: /ar/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب استخدام الخط الافتراضي للتصيير.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## ملاحظات

عند كون القيمة False وتحديد DefaultFontName، سيستخدم محرك العرض الخط المحدد بواسطة DefaultFontName كخط احتياطي. وإلا يتم استخدام خط 'Arial' (إذا كان مثبتًا) أو خطوط 'Generic Sans Serif' كخط احتياطي. يُستخدم الخط الاحتياطي أثناء عرض مشروع العرض عندما يشير نمط النص إلى خط غير مثبت على نظام التشغيل الحالي. للحصول على تحكم أكبر في حل الخطوط يمكنك استخدام استدعاء [`FontResolveCallback`](../fontresolvecallback/).

## الأمثلة

يوضح كيفية تعيين خط مخصص سيُستخدم لطباعة ملف PDF الناتج.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### انظر أيضًا

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


