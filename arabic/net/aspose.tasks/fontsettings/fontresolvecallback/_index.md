---
title: "FontSettings.FontResolveCallback"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية FontSettings. تحصل أو تعين رد اتصال يمكن استخدامه لتخصيص الخطوط التي تم حلها."
type: docs
weight: 30
url: /ar/net/aspose.tasks/fontsettings/fontresolvecallback/
---
## FontSettings.FontResolveCallback property

يحصل أو يضبط رد نداء يمكن استخدامه لتخصيص الخطوط التي تم حلها.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

## الأمثلة

يوضح كيفية تعيين رد اتصال حل الخط المخصص لتنفيذ كود معرف من قبل المستخدم لتعيين خط احتياطي أو لاستبدال الخط المحدد.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

options.FontSettings.FontResolveCallback = delegate(FontResolveEventArgs args)
{
    if (args.RequestedFontName != args.ResolvedFontName)
    {
        // يبدو أنه لا يمكن العثور على الخط المحدد وتم تعيين الخط الاحتياطي.
        // يمكننا تجاوز الخط الاحتياطي.
        args.ResolvedFontName = "Arial";
    }

    // أو ببساطة استبدال الخط المحدد:
    if (args.RequestedFontName == "Comic Sans MS")
    {
        args.ResolvedFontName = "Arial";
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### انظر أيضًا

* delegate [FontResolveCallbackDelegate](../../fontresolvecallbackdelegate/)
* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


