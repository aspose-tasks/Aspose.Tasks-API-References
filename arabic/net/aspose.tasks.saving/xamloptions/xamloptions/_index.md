---
title: "XamlOptions.XamlOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ XamlOptions. يهيئ مثيلاً جديداً من الفئة XamlOptions التي يمكن استخدامها لحفظ المشروع بتنسيق XAML"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

يهيئ مثيلاً جديداً من الفئة [`XamlOptions`](../) التي يمكن استخدامها لحفظ المشروع بتنسيق XAML.

```csharp
public XamlOptions()
```

## الأمثلة

يعرض كيفية حفظ مشروع بتنسيق XAML باستخدام خيارات الحفظ.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### انظر أيضًا

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


