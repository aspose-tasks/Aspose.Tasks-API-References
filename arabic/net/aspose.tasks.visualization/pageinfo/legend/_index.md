---
title: "PageInfo.Legend"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PageInfo. تحصل أو تعين نسخة من فئة PageLegend التي تحدد خيارات عرض أسطورة الصفحة"
type: docs
weight: 40
url: /ar/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

تحصل أو تعين نسخة من الفئة [`PageLegend`](../../pagelegend/) التي تحدد خيارات عرض أسطورة الصفحة.

```csharp
public PageLegend Legend { get; set; }
```

## ملاحظات

حاليًا ينطبق فقط على عروض مخطط جانت.

## الأمثلة

يعرض كيفية العمل مع معلومات أسطورة الصفحة.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// دعنا نقرأ معلومات أسطورة الصفحة
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// كما يُدعم تعديل الأسطورة
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

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

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


