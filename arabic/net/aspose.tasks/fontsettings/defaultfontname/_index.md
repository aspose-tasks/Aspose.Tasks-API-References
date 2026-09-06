---
title: "FontSettings.DefaultFontName"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية FontSettings. تحصل أو تعين الخط الافتراضي أو الاحتياطي للعرض."
type: docs
weight: 20
url: /ar/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

يحصل أو يضبط الخط الافتراضي (أو الاحتياطي) للتصيير.

```csharp
public string DefaultFontName { get; set; }
```

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


