---
title: "PageInfo.Margins"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PageInfo. يحصل على نسخة من الفئة PageMargins التي تحدد هوامش الصفحة"
type: docs
weight: 50
url: /ar/net/aspose.tasks.visualization/pageinfo/margins/
---
## PageInfo.Margins property

يحصل على نسخة من الفئة [`PageMargins`](../../pagemargins/) التي تحدد هوامش الصفحة.

```csharp
public PageMargins Margins { get; }
```

## الأمثلة

يعرض كيفية العمل مع معلومات الصفحة في عرض MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// دعنا نعدّل العرض الافتراضي.
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// دعنا نعدّل الهوامش.
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// دعنا نُعدّل إعدادات الصفحة
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// دعنا نُعدّل إعدادات عرض الصفحة
// عيّن قيمة تشير إلى ما إذا كان يجب طباعة الملاحظات.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// العمل مع المشروع...
```

### انظر أيضًا

* class [PageMargins](../../pagemargins/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


